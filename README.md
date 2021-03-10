# image-classifier

image classifier using CNN to detect which hotdog and not hotdog (the file for not hotdog containing the image of pizzas)

so first I want to explain the dataset : *I cant upload it to github because of the big size :" I will upload it as soon as I have resize the dataset* </br>
there are 3 folders, train, test and val
![image](https://user-images.githubusercontent.com/76993601/110578249-f6c33d80-8196-11eb-94dd-92fd8c673105.png)

this is the directory structure of the dataset:

hotdog_dataset</br>
|</br>
|---test</br>
| </pre>   |---hotdog</br>
|    |---not hotdog</br>
|---train</br>
|    |---hotdog</br>
|    |---not hotdog</br>
|---val</br>
|    |---hotdog</br>
|    |---pizza</br>

each folder 'hotdog','not hotdog','pizza' contains images the 'not hotdog' and 'pizza' both contains the images of pizza
so we want to classify which are hotdog and pizza, which there are 2 labels in this classifier.
the val folder is used for the validation of the model.

we use CNN architecture for the classifier, before we get into the classifier the image must be reshaped into the same size altogether
