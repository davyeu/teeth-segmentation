<h1> Teeth Segmentation</h1>

The following project aim is classify and segment teeth in dental X-ray images
with SOTA image processing models: detectron2 and nvidia/mit-b4 models.
The Dice score of both models is quite impresive. Demonestration
of the metric results presented below. 

<h2> The data source </h2>

The socure of the dataset is from [kaggle](https://www.kaggle.com/datasets/humansintheloop/teeth-segmentation-on-dental-x-ray-images).
and it is done manually by 12 Humans in the Loop trainees in the Democratic Republic of Congo as part of their trainings, 
using the Panoramic radiography database published by Lopez et al.
The dataset consists of 598 images with a total of 15,318 polygons, where each tooth is segmented with a different class.
Becuase of space limitation we do not store the image in this repository, instead we write a code to download this file to your local folder.

<h2> Juptyer notbooks explantions </h2>

The project include 4 Jupter notbooks:
<ul>
  <li> <b>Teeth Segmentation</b> : First part of the file is the code for downloading the images to your local folder and split them to training and validation sets.
    The second part of the the project is train and evaluate nvidia/mit-b4 model on the validation sets. The model parametes save in model directory </li>
  <li> <b> evaluate_model</b> : Evalute saved model from model directory on the valiadtion set </li>
  <li> <b> detectron2_for_teeth_segmentation <b>: using detectron2 model for the tasks of detection and segmentation </li> 
  <li><b> Detectron2 Tutorial</b> : Detectron2 Beginner's Tutorial </li>
</ul>

<h2> metrics </h2>

<h2> Some image for demonstration </h2>
