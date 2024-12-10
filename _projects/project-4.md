---
title: "Vehicle Detection Through Transfer Learning"
excerpt: "<div style='text-align: justify;'> 
<b>A Transfer Learning framework for detecting vehicles in aerial images</b>
<ul>
<li>Utilised the potential of transfer learning with VGG16 network architecture.</li> 
<li>Attained quicker convergence on vehicle detection dataset.</li>
<li>Conducted trials on grey and coloured images and obtained model accuracy of 60%.</li>
"
collection: projects
permalink: /projects/project-4

---

<h2>A Transfer Learning framework for detecting vehicles in aerial images</h2>

<p>In this work, I have utilized transfer learning to train the VGG16 model for vehicle detection in multi-modal imagery. I used the Vehicle Detection in Aerial Imagery (VEDAI) dataset, which contains overhead imagery.</p>

<h2>Dataset</h2>
<ul>
  <li>All experiments are performed using the VEDAI dataset, which contains aerial, ortho-normalized imagery from the publicly available Utah AGRC database.</li>
  <li>The original large field-of-view satellite images have been partitioned into images of size 1024 × 1024 and contain a wide diversity of vehicles, backgrounds, and confuser objects. The imagery is available in three visible color channels and one near infrared channel. While the VEDAI dataset contains 9 classes of objects, we focus our attention on small vehicles, namely the car and pickup classes.</li>
</ul>

<h2>Experiment</h2>
<ul>
  <li>The original VEDAI dataset contains vehicles of 9 classes, but in the experiments, we selected vehicles of two classes only: car and pickup.</li>
  <li>There are 2754 objects of the class 'car' and 1910 objects of the class 'pickup'. The VEDAI dataset used in our experiments contains images of resolution 512x512 and bounds the vehicle objects in boxes of resolution 20x20.</li>
  <li>The original VGG16 model was trained on the ImageNet dataset, which contains objects of 1000 classes. The model takes images of size 224x224 as input, so we had to resize the images of size 20x20 into 224x224.</li>
</ul>

<h2>Modification in Original VGG16 Model</h2>
<ul>
  <li>Since the original VGG16 model takes input size as 224x224, we had to resize the 20x20 images into 224x224. However, the images got blurred by resizing from the small pixel size of 20x20 to the high pixel size of 224x224. Therefore, we decided to modify the input to adapt to the different size. This technique worked effectively.</li>
</ul>
<h2>Conclusion</h2>
<ul>
  <li>In this work, we modified the original VGG16 model to accept input sizes of 128x128 and 64x64. We also utilized transfer learning by using the pre-trained weights of ImageNet and only training the last three dense layers.</li>
  <li>To prevent the model from overfitting, we used a dropout of 50% during training. When training, a percentage of the features are set to zero (50% in our case, since we are using Dropout(0.5)). During testing, all features are used (and scaled appropriately). This approach makes the model more robust and leads to higher testing accuracy.</li>
</ul>

<h2>Prediction</h2>
<img src="/images/vehicle_detection.png" width="35%" alt="Result" />

