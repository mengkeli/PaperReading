##Deeplearning4j parameter tuning##

- by MengkeLi

1. 读入训练数据，处理成一个DataIterator
2. 构建Deepface的网络
3. 迭代训练，输出预测结果
4. 调参和优化

#### DataIterator
---
自己定义一个DataIterator

```
public class LfwDataIterator implements DataSetIterator{
    batchNum //每批次的训练数据组数
    
    public boolean loadData(){}
    private void resetDataRecord(){} //重置训练批次列表
    public List<DailyData> readDataFromFile(String fileName) throws IOException{}
}
```
> LfwDataIterator实现了DataIterator接口，需要实现几个方法，例如hasNext、next、reset...用来进行每一批次DataSet的获取。loadData和readDataFromFile用来获取数据，并保存在一个DailyData类型的List中，每次调用next方法时，就会从List取出当前需要的数据，并构造成DataSet，返回给调用者

#### 构建网络

```
public static MultiLayerNetwork getNetModel(int In, int Out){
    MultilayerConfiguration conf = new NeuralNetConfiguration.Builder() // 配置一系列参数
    
    MultiLayerNetwork net = new MultiLayerNetwork(conf); // 传入参数
    net.init();
    new.setListeners(new ScoreIterationListener(1));
    
    return net;  
}
```
> 这段代码中有很多参数可以进行调整来寻找最优的拟合效果或调整训练速率，比如隐含层单元数目、激活函数、学习速率、正则化因子……构造好网络后加入一个ScoreIterationListener来监听每次迭代训练后的得分。

#### 迭代训练
设置迭代次数Epochs为100，表示用整个数据及反复训练100次

程序主函数
```
    public static void main(String[] args) {
        String inputFile = StockRnnPredict.class.getClassLoader().getResource("stock/sh000001.csv").getPath();
        int batchSize = 1;
        int exampleLength = 30;
        //初始化深度神经网络
        StockDataIterator iterator = new StockDataIterator();
        iterator.loadData(inputFile,batchSize,exampleLength);

        MultiLayerNetwork net = getNetModel(IN_NUM,OUT_NUM);
        train(net, iterator);
    }
```

