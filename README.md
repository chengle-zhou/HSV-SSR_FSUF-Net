#### FSUF-Net | IEEE TGRS 2024 | SSR of RGB Videos
---
## RGB-to-HSV: A Frequency-Spectrum Unfolding Network for Spectral Super-Resolution of RGB Videos

***Chengle Zhou, Zhi He, Anjun Lou, and Antonio Plaza***

*IEEE Transactions on Geoscience and Remote Sensing, vol. 62, pp. 1-18, Feb. 2024*

---

![framework](https://github.com/chengle-zhou/MY-IMAGE/blob/ed752dfbc251620c844b2cdf1790ed8b13f9b295/FSUF-Net/framework1.png)

Fig. 1. Overview of the proposed FSUF-Net method.



## Abstract

Hyperspectral videos (HSVs) play an important role in the monitoring domain, as they can provide more information than RGB videos about the movement of interesting objects from the perspective of material interpretation. However, the acquisition of HSV data is expensive and time-consuming, whereas RGB videos are readily available. In order to obtain HSV data from its corresponding RGB data, this paper proposes a lightweight frequency-spectrum unfolding network (FSUF-Net) for spectral super-resolution (SSR) of RGB video data. Specifically, the proposed FSUF-Net method belongs to a data-knowledge-driven joint paradigm, which is an interpretable SSR model instead of an end-to-end black-box architecture. The FSUF-Net consists of five main steps. First, the conversion representation of RGB video data to HSV data is derived into an initial recovery term, a data term, and a prior term according to a variable splitting method. Second, the spectral response function between hyperspectral images (HSIs) and RGB images is utilized to achieve the initial recovery term. Third, a convolutional neural network (CNN)-based frequency-domain subnetwork (called F-Net) is designed to solve the data subproblem for recovering the spatial detail information from the HSI, and a Transformer-based spectrum-domain subnetwork (called S-Net) is developed to solve the prior subproblem for reconstructing the spectral information of the HSI. Fourth, two network modules are employed to conduct parametric self-learning. Finally, the HSV data can be obtained in a fixed number of iterations, including alternately solving the above data subproblem and the prior subproblem. Experiments performed on several real HSV datasets demonstrate that the FSUF-Net can effectively reconstruct HSV from RGB videos as compared to traditional and state-of-the-art SSR methods.


## Results

Analysis of the influence of parameters D and N on the SSR performance of the FSUF-Net for different datasets. (a) WHISPERS dataset. (b) HyViD dataset. (c) Parameters of the FSUF-Net on the two HSV datasets.

![image-20240707160804744](https://github.com/chengle-zhou/MY-IMAGE/blob/1adca3bc2310c2c4ea2ec3578bb0423e02348328/FSUF-Net/image1.png)

Spectral super-resolution obtained for the WHISPERS hyperspectral video dataset by the competitive methods and our FSUF-Net method. The bold type is used for the optimal indicator, and the italic underline is used for the sub-optimal indicator.

![image-20240707161056020](https://github.com/chengle-zhou/MY-IMAGE/blob/1adca3bc2310c2c4ea2ec3578bb0423e02348328/FSUF-Net/image2.png)

Reconstructed results of “Worker” video 9-th frame from the WHISPERS dataset. Along 470, 500, 540, 580, and 620nm, the ground truth (GT) and
the reconstructed image of the SSR methods are presented. The first row is the ground truth (CC/SAM), and the second to last rows are the results of competitive methods and our FSUF-Net method.

![image-20240707161212394](https://github.com/chengle-zhou/MY-IMAGE/blob/1adca3bc2310c2c4ea2ec3578bb0423e02348328/FSUF-Net/image3.png)

Reflectance of “Board” video 9-th frame from the WHISPERS dataset at the timber, metal, and plant positions. (a) Timber, metal, and plant positions. (b) Reflectance at the timber position. (c) Reflectance at the metal position. (d) Reflectance at the plant position. (e) Total reflectance error at the timber, metal, and plant positions for each SSR methods.

![image-20240707161341011](https://github.com/chengle-zhou/MY-IMAGE/blob/1adca3bc2310c2c4ea2ec3578bb0423e02348328/FSUF-Net/image4.png)



In preparation for release soon.

Please cite our new paper:

**Plain Text:**

Chengle Zhou, Zhi He, Anjun Lou, and Antonio Plaza, "[RGB-to-HSV: A Frequency-Spectrum Unfolding Network for Spectral Super-Resolution of RGB Videos](https://ieeexplore.ieee.org/document/10419369)," IEEE Transactions on Geoscience and Remote Sensing, vol. 62, pp. 1-18, 2024, Art no. 5609318, doi: 10.1109/TGRS.2024.3361929.

**BibTex:**

```latex
@ARTICLE{zclVSSR2024,
  author={Zhou, Chengle and He, Zhi and Lou, Anjun and Plaza, Antonio},
  journal={IEEE Transactions on Geoscience and Remote Sensing}, 
  title={RGB-to-HSV: A Frequency-Spectrum Unfolding Network for Spectral Super-Resolution of RGB Videos}, 
  year={2024},
  volume={62},
  number={},
  pages={1-18},
  keywords={Spatial resolution;Videos;Image reconstruction;Superresolution;Optimization;Convolutional neural networks;Transformers;Deep unfolding;hyperspectral videos (HSVs);spectral super-resolution (SSR);Transformer},
  doi={10.1109/TGRS.2024.3361929}}
```



