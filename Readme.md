# Medical Diagnosis of Malaria and Pneumonia using SNN

Self Normalizing Neural Networks are used for diagnosing malaria and pneumonia and compared with the Inception model's performance.
SNN performs same as Inception, with very low computing time at low learning rate for malaria and pneumonia.
SNN outperformed Inception at a higher learning rate for pneumonia. 

SNN is a model inspired from ResNet. SNN uses the skip connection like ResNet and adds the tensor outputs of both the connections together.
SNN employs both short and long skip connections, as a result of which convergence is better and faster. 

Both connections are used because the spatial information lost along is recovered using long skip connections. Similarly the spatial information lost due to long skip connections are obtained using the short skip connections. 


## SNN architecture


![](images/SNN_architecture.png)


## Pneumonia
The dataset is publicly available in https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia


### Time taken by different models for training pneumonia
![](images/pneu_training_time.png)

SNN model is able to train faster than other models, because it's capable of training with images of smaller size, thus the number of convolutions operations to be performed is less, speeding the training process. 

x axis represents epochs and y axis presents training time in seconds

### Training accuracy of different models for pneumonia
![](images/training_accuracy_pneumonia.png)

x axis represents epochs and y axis presents training time in seconds

### Validation accuracy of different models for pneumonia
![](images/validation_accuracy_pneu.png)

x axis represents epochs and y axis presents training time in seconds

### Inception vs SNN with initial learning rate = 1e-2
![](images/higher_learning_rate.png)


## Malaria

The dataset is publicly available in https://lhncbc.nlm.nih.gov/publication/pub9932

### SNN v Inception performance on malaria
![](images/performance_malaria.png)

