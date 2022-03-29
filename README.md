# Clinical Decision Support System using Deep Learning

The goal of this project is to create a deep learning model that aids clinical decision making, focusing on aiding the process of differential diagnosis. Given a chest X-Ray, the deep learning model will output similar chest x-rays that have distinct medical reports. This will provide the doctor with distinct diagnoses that could apply to the input. I am currently working on the Computer Vision Section of this project, building a Variational Auto-Encoder. The project is done in collaboration with Third Eye Intelligence. The project is done in collaboration with Third Eye Intelligence, and as part of our Y3 Group Project as Computational Bioengineering students at Imperial College London.

This specific repo relates to the Computer Vision section of the project, with the initial goal of creating an AutoEncoder.

## Linear Auto-Encoder

So far, this autoencoder has only been trained first on 3% of the data, and then on 40% of the data (both times 1 epoch only) due to CPU constraints. The results can be compared below.

<img width="292" alt="Screenshot 2022-02-10 at 22 47 34" src="https://user-images.githubusercontent.com/78087643/153510464-4faa9122-7870-48d8-b542-3d6652b12e37.png">.

For 3% of data.

<img width="278" alt="Screenshot 2022-02-10 at 22 47 40" src="https://user-images.githubusercontent.com/78087643/153510487-a735e056-2264-412b-bf47-95b34feccb7c.png">
 
For 40% of data.

 ## Convolutional Auto-Encoder
 
 The results for the convolutional AE are incredibly better. The following image was obtained after only 3 epochs on 15% of the data.
 
 <img width="270" alt="Screenshot 2022-02-24 at 15 19 31" src="https://user-images.githubusercontent.com/78087643/155575927-b884bb1f-50e4-4df2-b05e-80b244282835.png">
 
The CNN has 2 convolutional layers + 1 Pooling Layer + 2 Transposed Convolutional Layers (Decoder).

## Deeper Convolutional Auto-Encoder

This CNN has 4 convolutional layers(intercalated with 4 Pooling Layers), followed by 3 Linear Fully connected Layers. The decoder part is a mirror of this, with 3 linear fully connected layers, followed by 4 Transposed Convolutional Layers.

 
