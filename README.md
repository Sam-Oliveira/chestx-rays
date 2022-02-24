# Cyclic Joint Representations for Diagnostic Images and Text (Deep Learning)

Medical image analysis has taken huge steps forward due to the emergence of practical machine learning algorithms based around the use of deep networks. However, the standard pipeline of medical image analysis involves a tedious process of human interpretation, sometimes with segmentation. Simple labelling is usually done, and this is fine, but does not scale well. Nor is it necessarily sustainable: when new imaging methods come along, one has to start from scratch again. The aim of this project is to generalise the principle of cycle-consistent training to provide a learning signal that can aid or regularise the learning of joint image/text representations. The project is done in collaboration with Third Eye Intelligence, and as part of our Y3 Group Project as Computational Bioengineering students at Imperial College London.

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

 
