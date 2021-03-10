# image-classifier

image classifier using CNN to detect which hotdog and not hotdog (the file for not hotdog containing the image of pizzas)

so first I want to explain the dataset : *I cant upload it to github because of the big size :" I will upload it as soon as I have resize the dataset* </br>
there are 3 folders, train, test and val
![image](https://user-images.githubusercontent.com/76993601/110578249-f6c33d80-8196-11eb-94dd-92fd8c673105.png)

this is the directory structure of the dataset:

hotdog_dataset</br>
|</br>
|---test</br>
|     |---hotdog</br>
|     |---not hotdog</br>
|---train</br>
|    |---hotdog</br>
|    |---not hotdog</br>
|---val</br>
|    |---hotdog</br>
|    |---pizza</br>

each folder 'hotdog','not hotdog','pizza' contains images the 'not hotdog' and 'pizza' both contains the images of pizza
so we want to classify which are hotdog and pizza, which there are 2 labels in this classifier.
the val folder is used for the validation of the model.

we use CNN architecture for the classifier, before we get into the classifier the image must be reshaped into the same size altogether, after it was reshaped then label it using integer, '1' for hotdog and '2' fot pizza
</br></br>
before creating the CNN model, visualize the data and verify it is the correct images with the correct label</br>
![image](https://user-images.githubusercontent.com/76993601/110593766-917b4680-81ae-11eb-987f-a1f506b74d1c.png)

creating the CNN model : 
![image](https://user-images.githubusercontent.com/76993601/110593818-a48e1680-81ae-11eb-8b67-4c95f4000176.png)

now use the test data for testing the model : </br>
![image](https://user-images.githubusercontent.com/76993601/110594001-da32ff80-81ae-11eb-81cf-b0bccf4481af.png)
as you can see, the accuracy keep improving almost every epoch
</br> </br> 

now it's time to do the validation using the val data :

![image](https://user-images.githubusercontent.com/76993601/110594154-05b5ea00-81af-11eb-9a35-0c94a8e6d672.png)

the accuracy reach 100%, first because there is only 2 class, which the probablity of the predict will be higher, also when the training the data the accuracy already high and improving almost every epoch so in conclusion it is possible to reach 100% when validating the data
