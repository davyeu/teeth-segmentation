<h1> Teeth Segmentation</h1>

This project aims to classify and segment teeth in dental X-ray images using state-of-the-art (SOTA) image processing models: Detectron2 and NVIDIA's mit-b4. The Dice score achieved by both models is impressive, demonstrating their effectiveness. Metric results are presented below.

<h2> Data Source </h2>

The dataset is sourced from [kaggle](https://www.kaggle.com/datasets/humansintheloop/teeth-segmentation-on-dental-x-ray-images). and was manually annotated  by 12 Humans in the Loop trainees in the Democratic Republic of Congo as part of their trainings, 
using the Panoramic radiography database published by Lopez et al.
The dataset consists of <b> 598 images</b> with a total of <b>15,318 </b>polygons, where each tooth is segmented with a different class.
Becuase of space limitation we do not store the image in this repository, instead we write a code to download this file to your local folder.

<h2> Juptyer notbooks Overview </h2>

<div>
  <p>This project includes four Jupyter notebooks:<p>
  <ol>
  
  <li><h3>Teeth Segmentation</h3></li>
  <ul>
    <li>Downloads the images to your local folder.</li>
    <li>Splits the dataset into training and validation sets.</li>
    <li>Trains and evaluates the <strong>NVIDIA mit-b4 model</strong> on the validation set.</li>
    <li>Saves the model parameters in the <code>model</code> directory.</li>
  </ul>
  
  <li><h3>evaluate_model</h3></li>
  <ul>
    <li>Evaluates the saved model from the <code>model</code> directory on the validation set.</li>
  </ul>
  
  <li><h3>detectron2_for_teeth_segmentation</h3></li>
  <ul>
    <li>Uses the <strong>Detectron2 model</strong> for detection and segmentation tasks.</li>
  </ul>
  
  <li><h3>Detectron2 Tutorial</h3></li>
  <ul>
    <li>A beginner-friendly tutorial for getting started with <strong>Detectron2</strong>.</li>
  </ul>
  </ol>
</div>

<h2> metrics </h2>

<table>
  <tr>
  <th> model name </th>
  <th> kind of metric </th>
  <th> result</th></tr>
  <tr>
    <td> nvidia/mit-b4 </td>
    <td> Average Dice Score </td>
    <td> 0.92 </td></tr>
  <tr>
    <td> detectron2 </td>
    <td> Average Dice Score </td>
    <td> 0.85 </td></tr>  
  <td> detectron2 </td>
    <td> Average Recall </td>
    <td> 0.525 </td></tr> 
</table>
<h2> Some images for demonstration </h2>
