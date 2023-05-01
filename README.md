# U-Net-Image-Segmentation-in-Keras-Pet-Example-

![image](https://user-images.githubusercontent.com/71633926/235498107-6d05c260-51b8-48e7-9fd2-7bcd794f1c6f.png)

<h2>U-Net Image Segmentation</h2>
U-Net is a popular convolutional neural network (CNN) architecture for image segmentation tasks. The U-Net architecture was first proposed by Ronneberger et al. in their paper titled "U-Net: Convolutional Networks for Biomedical Image Segmentation". Since then, it has been widely used in various image segmentation applications, such as medical image analysis, object detection, and scene segmentation.

<h2>Architecture</h2>
The U-Net architecture consists of two parts: the contracting path and the expansive path. The contracting path is a traditional convolutional neural network that reduces the spatial resolution of the input image and increases the number of channels. The expansive path is a series of up-convolutions that increase the spatial resolution of the image and decrease the number of channels. The expansive path is then concatenated with the corresponding layer from the contracting path to produce the final segmentation map.

<h2>U-Net Architecture</h2>

The contracting path is composed of several convolutional layers, each followed by a rectified linear unit (ReLU) activation function and a max-pooling layer. The number of channels is doubled at each max-pooling layer, resulting in a high-level feature representation with a reduced spatial resolution. The expansive path is composed of several up-convolutional layers, each followed by a convolutional layer with a ReLU activation function. The up-convolutional layers double the spatial resolution of the input, while the convolutional layers reduce the number of channels. The final layer of the U-Net architecture uses a softmax activation function to produce a probability map of the segmentation classes.

<h2>Loss Function</h2>
The loss function used in U-Net image segmentation is usually the binary cross-entropy loss or the dice loss. The binary cross-entropy loss is defined as:

<h2>Binary Cross-Entropy Loss</h2>

where y is the ground-truth segmentation map and p is the predicted probability map. The dice loss is defined as:

<h2>Dice Loss</h2>

where y is the ground-truth segmentation map, p is the predicted probability map, and w is a weight parameter that balances the contribution of false positives and false negatives.

<h2>Training</h2>
U-Net image segmentation is trained using backpropagation and stochastic gradient descent (SGD). The training process involves minimizing the loss function with respect to the model parameters. The training data consists of input images and corresponding ground-truth segmentation maps. During training, the input images are fed to the model, and the output segmentation maps are compared to the ground-truth segmentation maps using the loss function. The gradients of the loss function with respect to the model parameters are then computed using backpropagation, and the parameters are updated using SGD.

![image](https://user-images.githubusercontent.com/71633926/235498266-319442be-c1f7-4270-bee3-615b3c7f4a18.png)



<h2>References<h2>
<i>
Ronneberger, Olaf, et al. "U-Net: Convolutional Networks for Biomedical Image Segmentation." International Conference on Medical Image Computing and Computer-Assisted Intervention. Springer, Cham, 2015, pp. 234-241.</i>


