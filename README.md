# YOLO
YOLO implementation from scratch for detection of rudimentary shapes

***
### MultiClass
Localization and classification of objects of two different shapes (Circles / Rectangle)

![Multiclass image examples](https://image.ibb.co/krnAeq/multiclass-example.png)

###### Detection output using trained model 


<img src="https://j.gifs.com/2v3xXj.gif" alt="IMAGE ALT TEXT HERE" width="315" height="315" border="30" /> <img src="https://j.gifs.com/wmOV5z.gif" alt="IMAGE ALT TEXT HERE" width="315" height="315" border="30" />

Class prediction coloring -  `Blue : Rectangular` `Red : Circular`

Video links : [**Video1**](https://www.youtube.com/watch?v=K16a2hizF6s) [**Video2**](https://www.youtube.com/watch?v=hyrMQS7HMpU) 

***

### Combined 
Localization of 2 objects

![Combined image examples](https://image.ibb.co/hWtVUq/Combined-input.png)

***
### Circles
Localization of single circular object

![Circle image examples](https://image.ibb.co/f1mdFV/Circle-input.png)

### Blocks
Localization of single rectangular object

![Circle image examples](https://image.ibb.co/gimTFV/Blocks-input.png)


---
### Notes
 - For the prediction task, a probability map has not be used (as used in original paper). Instead class probabilities are predicted for every bounding box
 - For multiple object detection, a 1x2 grid has been used with a single bounding box associated with each grid cell
 - To simplify the learning task, input images were created in a manner that ensured that each cell always had a object in it
 - Ensembling.ipynb : Code to ensemble multiple trained YOLO models. Ensemble model shown to outperform individual models
 - VideoCreater.ipynb : Code for patching together multiple predicted output images
 
