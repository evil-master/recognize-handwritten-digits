�ȼ��� MNIST ����
```
>>> import mnist_loader
>>> training_data, validation_data, test_data = mnist_loader.load_data_wrapper()
```

�ڼ�����MNIST����֮�����ǽ�����һ����30�����ز���Ԫ��Network��
```
>>> import network
>>> net = network.Network([784, 30, 10])
```

��󣬽�ʹ������ݶ��½�����MNIST training_dataѧϰ����30�ε����ڣ�С�������ݴ�СΪ10��ѧϰ���ʦ�=3.0��
```
>>> net.SGD(training_data, 30, 10, 3.0, test_data=test_data)
```