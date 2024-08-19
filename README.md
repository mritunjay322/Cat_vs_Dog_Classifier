# Cat_vs_Dog_Classifier
# Problem statement :

In this Section i have  implementied Convolution Neural Network(CNN) Classifier for Classifying dog and cat images.I have used the transfer learning concept to get the better accuracy.I use the pre-trained Xception model without the top (classification) layer . I add classification layer as per our problem the train the model on my custom Dataset.

# Xception is a deep convolutional neural network architecture introduced by François Chollet in 2017. It is trained on the ImageNet dataset, which contains over 1.2 million labeled images across 1,000 different classes. The Xception model is characterized by its depth and efficiency, employing a series of depthwise separable convolutions that reduce the number of parameters while maintaining performance. This architecture is inspired by the inception module but replaces standard convolutions with depthwise separable convolutions, resulting in improved efficiency and performance. Xception has demonstrated strong performance in various computer vision tasks, including image classification, object detection, and segmentation.

# Model Summary-This is the model summary that i used to train the dataset:

Model: "sequential"
Layer (type)                Output Shape              Param #   

=================================================================

 xception (Functional)       (None, 7, 7, 2048)        20861480  
                                                                 
 average_pooling2d (AverageP  (None, 3, 3, 2048)       0         

 ooling2D)                                                       
                                                               
 flatten (Flatten)           (None, 18432)             0         
                                                               
 dense (Dense)               (None, 220)               4055260   
                                                               
 dense_1 (Dense)             (None, 1)                 221       
                                                               
=================================================================

Total params: 24,916,961

Trainable params: 4,055,481

# Model Accuracy: Below is the model accuracy that i was able to achieve.

Test Loss: 0.045325081795454025

Test Accuracy: 0.9862499833106995

Lastly, I run my model on random images of cat and dog from internet.Below are the results:-

1/1 [==============================] - 0s 50ms/step

![image](https://github.com/user-attachments/assets/038e3cb9-25cc-495c-9749-dd6c29a7bb16)

/1 [==============================] - 0s 31ms/step

![image](https://github.com/user-attachments/assets/91e52f84-7186-4120-a1cc-4460581ad65f)

1/1 [==============================] - 0s 35ms/step

![image](https://github.com/user-attachments/assets/4fc7db8b-5fdb-49ce-a6e2-9b7b68161625)





