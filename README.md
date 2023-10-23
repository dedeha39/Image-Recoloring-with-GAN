# Image Recoloring with Generative Adversarial Networks (GANs)

## Overview

This repository contains the implementation of a deep learning model for image recoloring using Generative Adversarial Networks (GANs). The project aims to generate realistic color images from grayscale input images. Two different GAN architectures, namely Vanilla GAN and Wasserstein GAN (WGAN), were implemented and compared for their effectiveness in image recoloring.

## Key Features

- **Vanilla GAN and WGAN:** Implemented both Vanilla GAN and Wasserstein GAN models for image recoloring.
- **U-Net Architecture:** Utilized U-Net architecture for the generator network, allowing efficient upsampling and downsampling of images.
- **PatchGAN Discriminator:** Implemented PatchGAN discriminator for local patch-level classification of images.
- **Datasets:** Used COCO and ImageNet datasets for training and testing the models.
- **Evaluation Metrics:** Evaluated model performance using Frechet Inception Distance (FID), Peak Signal-to-Noise Ratio (PSNR), and Structural Similarity Index (SSIM).

## Model Architectures

- **Vanilla GAN:** Vanilla GAN architecture was used with a combination of L1 and adversarial (GAN) loss functions for training the model.
- **Wasserstein GAN (WGAN):** Implemented Wasserstein GAN with Wasserstein distance as the loss function, ensuring stable training and improved gradients.

## Results

- **Vanilla GAN:** Achieved superior results in terms of FID, PSNR, SSIM, and visual quality for both COCO and ImageNet datasets.
- **Wasserstein GAN (WGAN):** Although acceptable, the results were not as impressive as Vanilla GAN, especially for the ImageNet dataset.

## Usage

1. Clone the repository: `git clone https://github.com/username/image-recoloring-gan.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Train the model: `python train.py --dataset coco --gan_type vanilla`
4. Generate recolored images: `python generate.py --input_path input_images/ --output_path output_images/`

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## References

[1] Y. Pang, J. Lin, T. Qin, and Z. Chen, “Image-to-image translation: Methods and applications,” IEEE Transactions on Multimedia, vol. 24, pp. 3859–3881, 2022.
[2] I. Zeger, S. Grgic, J. Vukovic, and G. Sisul, “Grayscale image col- orization methods: Overview and evaluation,” IEEE Access, vol. 9, pp. 113326–113346, 2021.
[3] M. S. Khan, Y. Gotoh, and N. Nida, “Medical image colorization for better visualization and segmentation,” pp. 571–580, 07 2017.
[4] P. Isola, J.-Y. Zhu, T. Zhou, and A. A. Efros, “Image-to-image translation with conditional adversarial networks,” 11 2016.
[5] J. Brownlee, “How to implement pix2pix gan models from scratch with keras,” 07 2019.
[6] M. Heusel, H. Ramsauer, T. Unterthiner, B. Nessler, and S. Hochreiter, “Gans trained by a two time-scale update rule converge to a local nash equilibrium,” 06 2017.
[7] M. Lucic, K. Kurach, M. Michalski, S. Gelly, and O. Bousquet, “Are gans created equal? a large-scale study,” arxiv.org, 11 2017.
[8] C. Ballester, A. Bugeau, H. Carrillo, M. Cl ˜A©ment, R. Giraud, L. Raad, and P. Vitoria, “Analysis of different losses for deep learning image colorization,” 05 2022.
[9] O. Ronneberger, P. Fischer, and T. Brox, “U-net: Convolutional networks for biomedical image segmentation,” 2015.
[10] U. Demir and G. Unal, “Patch-based image inpainting with generative adversarial networks,” 03 2018.
[11] C. M. Ward, J. Harguess, B. Crabb, and S. Parameswaran, “Image quality assessment for determining efficacy and limitations of super- resolution convolutional neural network (srcnn),” 09 2017.
[12] M. Arjovsky, S. Chintala, and L. Bottou, “Wasserstein gan,” 2017.
[13] N. S. , G. Hinton and K. Swersky, “”neural networks for machine learning lecture 6a overview of mini-batch gradient descent”,” 07 2012.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
