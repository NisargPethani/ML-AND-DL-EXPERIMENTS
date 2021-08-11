# AUTOENCODER

Implemented a fully functioning under complete autoencoder for feature learning.

## Tasks

- Use the MNIST dataset for all the experiments. Use a 70:30 data split.

    1. Load the dataset using “ torchvision.datasets” library, preprocess the dataset using “torch. vision.transforms” library and finally create a train loader and test loader of some batch size using “torch.utils.data” library.
    
    2. Create an autoencoder class with decoder and encoder architecture and a hidden neuron representation.

    3. Initialise an optimizer using “torch.optim” library and you can also use a learning rate scheduler using “torch.optim.lr_scheduler” library.

    4. Write a training loop over epochs and over the batches of the train set and calculate the average loss between thereconstructed image and the input image.

    5. Write a testing loop over the batches of the test set and calculate the loss between the reconstructed image and the input image.

    6. You can save the best performing model using “torch.save”. 
    
- Report the test reconstruction loss and plot the train loss vs epochs for the following cases :

    1. Perform the experiment using different optimizers 
        - Adam
        - RMSProp
        - SGD with momentum
        - SGD without momentum.

    2. Plot the test reconstruction loss vs hidden neurons for all the above optimizers.

    3. Perform PCA reconstruction and compare with the Autoencoder reconstruction using test reconstruction loss (you can use inbuilt PCA).