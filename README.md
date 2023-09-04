<a name="top"></a>
# Rocket League - AI Item Predictor
**Image classifier** of items from the video game '*Rocket League*'. 

\* The project is currently on hold until I have enough knowledge to proceed with the **multi-labeling classification** :) \*

*First job with Artificial Intelligence.*

## Table of contents
* [Description](#description)
* [Visuals](#visuals)
* [Versioning](#versioning)
* [Technologies](#technologies)
* [Bibliography](#bibliography)
 
<a name="description"></a>
### 1. Description
This is a project to try to identify the type of different `Rocket League` items via images. I created a dataset collected, modified and cleaned from [rlgarage](https://rocket-league.com/items).
All the images were *220x220*px and `.png` format.

The images were separated into different directories according to the type they corresponded to. The training and validation directories were also added with `1584 images belonging to training` and `395 images belonging to validation`.

I had to remove the "explosions" element type, since it would create a big problem for the model when it comes to differentiating between "boosts" and "explosions", since in the images they were practically impossible to classify even for a person with knowledge about the game.

This is my first project related to `AI`, with `CNN` and `image classification` and if possible I would like to improve the scope of this project to deploy the model in a real environment when it is finished and is able to classify several items in a single photo.

---
 
[Go up⬆️](#top)

<a name="visuals"></a>
### 2. Visuals

For example, given this image:

![](https://rocket-league.com/content/media/items/avatar/220px/42a71338bd1551122241.png "42a71338bd1551122241.webp")

The model predicted this:

```
Saving 42a71338bd1551122241.webp to 42a71338bd1551122241.webp
1/1 [==============================] - 7s 7s/step
42a71338bd1551122241.webp
This image is in: [wheels]
```

---
 
[Go up⬆️](#top)
 
<a name="versioning"></a>
### 3. Versioning
 #### Update [26/08/2023]

**Version 0.1.1** is out! This version includes the following:

- `RL_items` dataset available to download and use inside the notebook.
- `86% accuracy example model` added for easier understanding of the project.
-  Image augmentation included to try to improve the model's accuracy.
-  Allows users to build their own model from a prebuilt example.

Weak points:

- `86% accuracy example model` should be modified or redone to improve it's accuracy.
- `Model predictions` should be easier to understand for the final user, instead of showing the results with numbers.
  
Future Improvements:

- `Save & Download your model` feature should be added.
- `Model predictions` should be easier to understand for the final user, instead of showing the results with numbers.
-  Finish the 'Conclusions' section in the notebook.
  
#### Update [27/08/2023]

Few changes added!

- `96% accuracy example model` in order to substitute the old example model.
-  Image augmentation was removed as the main objective of the project is to identify the type of the object from a specific type of image, allowing the model to improve it's accuracy by `10%`.
-  `Save & Download your model` feature was added. Now you can continue working with your own creation!
-  `Model predictions` are now shown as the type of object that was predicted instead of a bunch of numbers.

 Weak points:

- The model struggle to differenciate sometimes images between `boosts & trails`.
- There is no `Table of Contents` in the notebook.
  
Future Improvements:

- Add the version of the project to the notebook.
- Maybe I could improve the explanations of each block inside the notebook for the reader to understand it better.
- This is was the first milestone in the project, now I can start studying the possibilities to expand the model or create a new one to classify various items in the same image.
- Finish the 'Conclusions' section in the notebook.

---
  
[Go up⬆️](#top)
 
<a name="technologies"></a>
### 4. Technologies

`tensorflow` and `tensorflow.keras` for the model training and the model structure.

`matplotlib.pyplot`, `numpy` and `PIL.Image` for showing the results of the training and some examples of the dataset.

`gdown` and `google.colab` to load/download the model into your PC once it has been saved.

---
 
[Go up⬆️](#top)

<a name="bibliography"></a>
### 5. Bibliography

 [DeepLearning.AI TensorFlow Developer Professional Certificate - DeepLearning.AI on Coursera🔗](https://www.coursera.org/professional-certificates/tensorflow-in-practice?)
 
 [RL Garage Items Database🔗](https://rocket-league.com/items)

 [gdown - PyPi🔗](https://pypi.org/project/gdown/)

 [Sparse Categorical Cross-Entropy vs Categorical Cross-Entropy - Felipe A. Moreno - Medium🔗](https://fmorenovr.medium.com/sparse-categorical-cross-entropy-vs-categorical-cross-entropy-ea01d0392d28)

 [Save, serialize, and export models - Neel Kovelamudi, Francois Chollet - TensorFlow🔗](https://www.tensorflow.org/guide/keras/serialization_and_saving)

 ---
 
[Go up⬆️](#top)

## License

[MIT](https://choosealicense.com/licenses/mit/)

## Made by

- [Pikeras72](https://github.com/Pikeras72)
  
## Special Thanks

- [blitty-codes](https://github.com/blitty-codes)
