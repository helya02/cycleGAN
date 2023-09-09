# cycleGAN
CycleGAN, short for Cycle-Consistent Generative Adversarial Network, is a deep learning model used for image-to-image translation tasks. It was first introduced by Jun-Yan Zhu et al. in 2017.  
 
CycleGAN aims to learn a mapping between two different domains (e.g., horses and zebras) without requiring paired examples for training. This means that it can learn to translate images from one domain to another even if there is no direct correspondence between the images in the training set. 
 
The key idea behind CycleGAN is to introduce cycle consistency. It assumes that if an image from domain A is translated to domain B and then translated back to domain A, it should be similar to the original image. Similarly, if an image from domain B is translated to domain A and then back to domain B, it should also be similar to the original image. By enforcing this cycle consistency, CycleGAN can learn to perform image translation without explicitly paired training data. 
 
The model consists of two generators and two discriminators. The generators learn to translate images from one domain to another, while the discriminators try to distinguish between the translated images and real images from the target domain. The generators and discriminators are trained in an adversarial manner, where they compete against each other to improve their performance. I used the U-Net model as the generator of cycleGAN.
 
CycleGAN has been successfully applied to various image-to-image translation tasks, such as style transfer, object transfiguration, and even domain adaptation. It has shown promising results in generating realistic and high-quality translations between different visual domains.
