# Medium . Permeation
## SARS-COV-2 Painting Creation by Generative Model
[Paper](https://arxiv.org/abs/2304.11354) | [Project Page](https://yfyangd.github.io/CVPR2023/) | [Vedio](https://youtu.be/wPNgvnJZGCE) | [Code]()

Impressionism expressed the scientific meaning of "light" in artistic creation. The light color reflected by the luminous flux through the medium in the air became the concept of impressionists’ creation.

After collecting the web imagination of global citizens about SARS-COV-2, we trained the generative model and let the computer randomly synthesize it. We adjusted various parameters during the training process making the results such as Dou Jia, Monet, Renoir , their style paintings.

Through this work the diffusion path of SARS-COV-2 spreading the molecular of the virus through the air, just like the scattering phenomenon formed by light through the particles in the air. Color is exclusive to the humans’ world, and COVID_19 is also born with humans.

The colorful world we see in this work represents the equality of races on the earth. The array of 196 pictures represents 196 countries were invaded by the SARS-COV-2. As human beings, none of us are spared from this disaster.

## Statement
[![IMAGE ALT TEXT HERE](https://drive.google.com/uc?export=view&id=1WShAvQeCuWsfFyr6aiBVgsL-Oki0VL2W)](https://www.youtube.com/embed/QZXdjV6TTPc)

## Generative Model: Self-Attention GAN
The proposed art-generating model is realized by a model called Self-Attention Generative Adversarial Network (SAGAN). GANs consists of two adversarial models: a generative model G and a discriminative model D. Generator captures the data distribution, and Discriminator estimates the probability that a sample came from the training data rather than Generator. Both Generator and Discriminator are trained simultaneously. 

<img style="float: left;" src="./image/SAGAN.png" width="100%">
<pre>
   
</pre>

## Self-Attention
For each query location, self-attention block calculates the pairwise relationship between the query location and all locations to form an attention map, and then aggregates the features of all positions through the weighted sum with the weights defined by the attention map. Finally, the aggregated features are added to the features of each query position to form the output. The basic self-attention architecture is shown in the following figure. 

<img style="float: left;" src="./image/SelfAttention.png" width="100%">
<pre>
   
</pre>

## Super Resolution - SASR-Net
SASR-Net consists of convolution layers, attention block, and a deconvolution layer as illustrated in follow figure. Convolution layers and activation function layers are primary components of typical CNN. The other prime component of CNN is a pooling layer, also called a subsampling layer. The pooling layer chooses featured values from the image for progressive reduction of the number of parameters and the computational cost in the network, but it causes loss of input image information. In order to keep the feature values, the proposed method excluded the pooling layer in its architecture and designed SASR-Net with the deconvolution layer to upsample the low-resolution SARS-COV-2 paintings. We also introduce channel-wise attention in our model, which can capture the feature importance during convolution processes. By focusing on a part of the channels of the input feature and deactivating non-related concepts, the models can focus on the concepts of interest.

<img style="float: left;" src="./image/SASR.png" width="100%">
<pre>
   
</pre>

## Gradual Change by Graph Neural Network
In this section, we have developed an extended work: Gradual Change. We use Graph Neural Network technology to present 196 paintings of the new coronavirus created by A.I. to the audience one by one in a gradual manner. It symbolizes that the current new coronavirus will continue to evolve, and the speed of vaccine development cannot keep up with the speed of virus mutation. This work symbolizes that SARS-CoV-2 has brought challenges that the world has never had before.

<img style="float: left;" src="./image/GNN1.png" width="100%">
<pre>
   
</pre>

## Artwork
Our works generated 196 paintings through the Self-Attention Generative Adversarial Network after learning the creation of SARS-COV-2 art works by artists from all over the world. We trained the generative model and let the computer randomly synthesize it. We adjusted various parameters dur-ing the training process making the results such as Dou Jia, Monet, Renoir, their style paintings. Then, we use Self-Attention Super Resolution Network to obtain a higher resolution painting. Through SASR-Net, we can build a deeper network for feature extraction without the vanishing gradient problems. The final artwork of SARS-COV-2 paintings produced by artificial intelligence is shown as below Figure.

<img style="float: left;" src="https://drive.google.com/uc?export=view&id=1oWi11S6MvdDFTmNUSesZZxulN7utEXWR" width="100%">
<pre>
   
</pre>

## Gradual Change
Finally, we have developed an extended work: Gradual Change. We use Graph Neural Network to present 196 painting of the new coronavirus created by SAGAN to the audience one by one in a gradual manner. It symbolizes that the current new coronavirus will continue to evolve, and the speed of vaccine development cannot keep up with the speed of virus mutation. This work symbolizes that SARS-CoV-2 has brought challenges that the world has never had before.

[![IMAGE ALT TEXT HERE](https://drive.google.com/uc?export=view&id=110sVfN2y3466GiyM3CD9-xLixrDzYTgS)](https://www.youtube.com/embed/vpkR4jU1aec)

## Authors
### YuanFu Yang (楊元福)
#### International collegiate PHD program student in National Tsing Hua University, TW.
#### Data Scientist / tsmc
Born in Taipei, Taiwan in 1979. Yang is the Ph.D. student at National Tsing Hua University for his research on Artificial Intelligence (AI) to enhance human creativity. He joined Taiwan Semiconductor Manufacturing Company in 2006. Yang conducts research and production across fields such as defect inspection and yield prediction using deep learning techniques. Yang, himself, has been exploring the potential expansion of painting creativity through the AI and human experts.
### Iuan Kai Fang (房元凱)
#### International collegiate PHD program student in National Tsing Hua University, TW.
#### Master degree in lighting design from Parsons School of Design, NY. The other’s in interior design from Chung Yuan University, TW.
He has been engaged in interior design for nearly 20 years. His works have won numerous awards including Red Dot ,IF,etc. However, he just started to touch the field of AI Art . Currently, he is studying the technology of 2D single image automatic generates to a 3D model.

<img style="float: left;" src="./image/authors.jpg" width="100%">
