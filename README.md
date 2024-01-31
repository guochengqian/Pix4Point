# Pix4Point [3DV 2024]
### [arXiv](https://arxiv.org/abs/2208.12259) | [code](https://github.com/guochengqian/PointNeXt) | [doc](https://guochengqian.github.io/PointNeXt/projects/pix4point/)
*by [Guocheng Qian](https://www.gcqian.com/), [Abdullah Hamdi](https://github.com/ajhamdi), [Xingdi Zhang](https://cindy-xdzhang.github.io/), [Bernard Ghanem](https://www.bernardghanem.com/)*

Webpage for paper `Pix4Point: Image Pretrained Standard Transformers for 3D Point Cloud Understanding`

**Code is avaliable in https://github.com/guochengqian/PointNeXt, refer to [documentation](https://guochengqian.github.io/PointNeXt/projects/pix4point/) for training and testing details**

**Open an issue in https://github.com/guochengqian/PointNeXt if you have question regards to Pix4Point**. 

---
**Pix4Point: Image Pretrained Standard Transformers for 3D Point Cloud Understanding**

![TEASER](misc/teaser.png)

**TL;DR:** We formulate a novel pipeline dubbed Pix4Point that allows harnessing pretrained Transformers in the image domain to improve downstream point cloud tasks. 


**Abstract**: 
While Transformers have achieved impressive success in natural language processing and computer vision, their performance on 3D point clouds is relatively poor. This is mainly due to the limitation of Transformers: a demanding need for extensive training data. Unfortunately, in the realm of 3D point clouds, the availability of large datasets is a challenge, exacerbating the issue of training Transformers for 3D tasks. In this work, we solve the data issue of point cloud Transformers from two perspectives: (i) introducing more inductive bias to reduce the dependency of Transformers on data, and (ii) relying on cross-modality pretraining.  More specifically, we first present Progressive Point Patch Embedding and present a new point cloud Transformer model namely PViT. PViT shares the same backbone as Transformer but is shown to be less hungry for data, enabling Transformer to achieve performance comparable to the state-of-the-art. Second, we formulate a simple yet effective pipeline dubbed _Pix4Point_ that allows harnessing Transformers pretrained in the image domain to enhance downstream point cloud understanding. This is achieved through a modality-agnostic Transformer backbone with the help of a tokenizer and decoder specialized in the different domains. Pretrained on a large number of widely available images, significant gains of PViT are observed in the tasks of 3D point cloud classification, part segmentation, and semantic segmentation on ScanObjectNN, ShapeNetPart, and S3DIS, respectively. Our code and models are available at [PointNeXt repo](https://github.com/guochengqian/pointnext). 

<p float="left">
  <img src=misc/s3dis_result.png width="47.5%" />
  <img src=misc/training_curves.png width="50%" />
</p>

![vis](misc/s3dis_vis.png)

# News
- :boom: Sep 2022, Code released in https://github.com/guochengqian/PointNeXt
-  :pushpin:  [Bernard Ghanem](https://www.bernardghanem.com/) is hiring visiting students. Monthly salary is paid with free housing. Contact Guocheng if interested: guocheng.qian@kaust.edu.sa


### Citation
If you are using our code in your work, please kindly cite the following:  
```
@inproceedings{qian2022improving,
  author={Guocheng Qian and Xingdi Zhang and Abdullah Hamdi and Bernard Ghanem},
  booktitle = {3DV},
 title={Improving Standard Transformer Models for 3D Point Cloud Understanding with Image Pretraining},
  year = {2024}
}
``` 

