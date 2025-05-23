##  Title

Neurodynamic Analysis-Driven Coupled Neural P Systems for Multi-Focus Image Fusion



## Abstract

Multi-focus image fusion (MFIF) is a crucial technique in image processing, with a key challenge being the generation of decision maps with precise boundaries. However, traditional methods based on heuristic rules and deep learning methods with black-box mechanisms are difficult to generate high-quality decision maps. To overcome this challenge, we introduce neurodynamic analysis-driven coupled neural P systems, which are third-generation neural computation models inspired by spiking mechanisms, to enhance the accuracy of decision maps. Specifically, we first conducted an in-depth analysis of the neural dynamics of the model to identify the constraints between the network parameters and the input signals. This solid analysis avoids abnormal continuous firing of neurons and ensures the model accurately distinguishes between focused and unfocused regions, generating high-quality decision maps for the MFIF task. Based on this, we then propose a novel approach for MFIF based on neurodynamic-driven coupled neural P systems, called NDCNPFuse. Unlike current ideas of decision map generation, NDCNPFuse distinguishes between focused and unfocused regions by mapping the source image into interpretable spike matrices. By comparing the number of spikes, an accurate decision map can be generated directly without any post-processing. Experimental results on three datasets show that our method outperforms 15 state-of-the-art MFIF methods in visual and quantitative performance. Moreover, NDCNPFuse is able to significantly improve the performance of downstream tasks such as salient object detection. The code for NDCNPFuse is available at https://github.com/MorvanLi/MFIF-NDCNPFuse.

## Comparison Methods

We also give all the comparative experimental SOTA methods in this paper:

- Traditional methods
  - [PA-DCPCNN](https://github.com/Chinmaya-Panigrahy/Fractal-dimension-based-parameter-adaptive-dual-channel-PCNN-for-multi-focus-image-fusion)
  - [NSCT-CNP](https://github.com/MorvanLi)
- Deep learning methods
	- [DRPL](https://github.com/sasky1/DRPL)
	- [CU-Net](https://github.com/cindydeng1991/TPAMI-CU-Net)
	- [SDNet](https://github.com/HaoZhang1018/SDNet)
	- [DRPL](https://github.com/sasky1/DRPL)
	- [DRL-FPD](https://github.com/yuliu316316/DRL-FPD-MFIF)
	- [GACN](https://github.com/Keep-Passion/GACN)
	- [U2Fusion](https://github.com/hanna-xu/U2Fusion)
	- [SwinFusion](https://github.com/Linfeng-Tang/SwinFusion)
	- [ZMFF](https://github.com/junjun-jiang/ZMFF)
	- [MUFusion](https://github.com/AWCXV/MUFusion)
	- [DeepM2CDL](https://github.com/JingyiXu404/TPAMI-DeepM2CDL)
	- [MGDN](https://github.com/Guanys-dar/MGDN)
	- [DB-MFIF](https://github.com/Zancelot/DB-MFIF)
	- [TC-MoA](https://github.com/YangSun22/TC-MoA)

## Implementation Details
The traditional methods run on an Intel(R) Core(TM) i5-13400 CPU, and the DL methods run on a single Nvidia A100 GPU. We set the coupling radius $r$ of PACNPFuse to be 16 and the number of iterations $t$ to be 110.



## Note
We did not upload the experimental results data of all the comparison methods because they were too large. If any researcher needs the results of these comparison methods, please contact me via email: morvanli@stu.xjtu.edu.cn.
