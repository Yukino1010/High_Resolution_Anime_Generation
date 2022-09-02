# High_Resolution_Anime_Generation

<p align="center">
<img width="400px" src="https://github.com/Yukino1010/High_Resolution_Anime_Generation/blob/master/result/final_1.jpg?raw=true" >
<img width="400px" src="https://github.com/Yukino1010/High_Resolution_Anime_Generation/blob/master/result/final_3.jpg?raw=true">
</p>

<p align="center">
<img width="400px" src="https://github.com/Yukino1010/High_Resolution_Anime_Generation/blob/master/result/final_2.jpg?raw=true" >
<img width="400px" src="https://github.com/Yukino1010/High_Resolution_Anime_Generation/blob/master/result/final_5.jpg?raw=true">
</p>


## Introduce
This is an implimentation of PGGAN (Progressive Growing of GANs for Improved Quality, Stability, and Variation). PGGAN can generate high resolution image by training each resolution from low to high independently, with a fade-in structure to maintain the robustness in both generator and discriminator.


## Network Structure
To make the implimentation simpler, we replace the pixel normalization with batch normalization whlie didn't apply equalized learning rate in the model.
Besides, we use wasserstein distance as the loss function with the critic 5.
## Hyperparameters

- START_IMG_SIZE = 16
- N_CRITIC = 5
- EPOCH_TRAN_REV = 40
- EPOCHS = 200
- Z_DIM = 512
- LAMBDA = 10
- BATCH_SIZE = 16
- TOTAL_ITER = 2500

## Data

## Result
<p align="center">
<img width="400px" src="https://github.com/Yukino1010/High_Resolution_Anime_Generation/blob/master/result/rev16.jpg?raw=true" >
<img width="400px" src="https://github.com/Yukino1010/High_Resolution_Anime_Generation/blob/master/result/rev32.jpg?raw=true">
</p>

<p align="center">
16 resolution and 32 resolution
</p>

<p align="center">
<img width="400px" src="https://github.com/Yukino1010/High_Resolution_Anime_Generation/blob/master/result/rev64.jpg?raw=true" >
<img width="400px" src="https://github.com/Yukino1010/High_Resolution_Anime_Generation/blob/master/result/rev128.jpg?raw=true">
</p>

<p align="center">
64 resolution and 128 resolution
</p>


## References
