# YOLO
YOLO implementation from scratch for detection of rudimentary shapes

***
### MultiClass
Localization and classification of objects of two different shapes (Circles / Rectangle)

![Multiclass image examples](https://image.ibb.co/krnAeq/multiclass-example.png)

###### Detection output using trained model 


![Multiclass image examples](https://media.giphy.com/media/2ZYF7KIrIOFt98RcI9/giphy.gif)

<p>
<a href="http://www.youtube.com/watch?feature=player_embedded&v=K16a2hizF6s&t=17s" target="_blank"><img src="https://image.ibb.co/kqoavV/pred-thumbnail.png" alt="IMAGE ALT TEXT HERE" width="315" height="315" border="30" /></a> <a href="http://www.youtube.com/watch?feature=player_embedded&v=hyrMQS7HMpU" target="_blank"><img src="https://image.ibb.co/iURH9q/pred2-thumbnail.png" alt="Prediction 2" width="300" height="300" border="30" /></a>
</p>

Class prediction coloring -  `Blue : Rectangular` `Red : Circular`

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
#### Notes
 - For the prediction task, a probability map has not be used (as used in original paper). Instead class probabilities are predicted for every bounding box
 - For multiple object detection, a 1x2 grid has been used with a single bounding box associated with each grid cell
 - To simplify the learning task, input images were created in a manner that ensured that each cell always had a object in it
 - Ensembling.ipynb : Code to ensemble multiple trained YOLO models. Ensemble model shown to outperform individual models
 - VideoCreater.ipynb : Code for patching together multiple predicted output images
 
