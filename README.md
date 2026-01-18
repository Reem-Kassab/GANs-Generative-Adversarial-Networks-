# 👟 Footwear Generation using GANs

## 📝 Description
This project explores the capabilities of **Generative Adversarial Networks (GANs)** in the domain of Computer Vision. The primary goal is to generate new, synthetic images of footwear that closely resemble real-world samples.

The model was trained on the **Footwear Dataset** sourced from Kaggle. It consists of a **Generator** (which creates images) and a **Discriminator** (which tries to distinguish real images from fake ones), training together in a zero-sum game until the generator produces realistic outputs.

## 🚀 Key Features
* **Generative Model:** Implements a GAN architecture (e.g., DCGAN) to synthesize images.
* **Custom Dataset:** Trained on a diverse collection of footwear images.
* **Progressive Training:** Visualizes the improvement of generated images over epochs, moving from random noise to recognizable shapes.
* **Loss Visualization:** Tracks Generator and Discriminator losses to ensure stable training.

## 🛠️ Technologies Used
* **Deep Learning Framework:** TensorFlow
* **Language:** Python
* **Libraries:** Matplotlib, NumPy
* **Dataset:** [Kaggle Footwear Dataset](https://www.kaggle.com/datasets/adityakadam1/footwear/data)


## 💻 How it Works
1.  **Preprocessing:** Images are resized and normalized (e.g., to range [-1, 1]).
2.  **Architecture:**
    * **Generator:** Takes a random noise vector (latent space) and upsamples it to generate an image.
    * **Discriminator:** A classifier that attempts to distinguish between real images from the dataset and fake images from the Generator.
3.  **Training:** Both networks are updated iteratively. The Generator gets better at fooling the Discriminator, while the Discriminator gets better at spotting fakes.

## 🏃‍♀️ How to Run
1.  Clone the repository.
2.  Install dependencies:
    ```bash
    pip install torch torchvision matplotlib numpy
    ```
