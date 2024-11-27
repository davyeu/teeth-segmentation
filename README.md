<h1> Teeth Segmentation</h1>

The following project aim is classify and segment teeth in dental X-ray images
with SOTA image processing models: detectron2 and nvidia/mit-b4 models.
The Dice score of both models is quite impresive. Demonestration
of the metric results presented below. 

<h2> The Data </h2>

The socure of the dataset is from [kaggle]([url](https://www.kaggle.com/datasets/humansintheloop/teeth-segmentation-on-dental-x-ray-images)) 
and it is done manually by 12 Humans in the Loop trainees in the Democratic Republic of Congo as part of their trainings, 
using the Panoramic radiography database published by Lopez et al.
The dataset consists of 598 images with a total of 15,318 polygons, where each tooth is segmented with a different class.
