# X-Ray-images-classification
This project was part of the exam and of the evaluation of the course 'Applied AI in Biomedicine' at Politecnico di Milano. 
We had to face the problem of X-ray image classification regarding chest X-ray images. We implemented and compared three different deep learning models in order to correctly classify X-ray images in 3 possible classes: Normal(N), Pneumonia(P) and Tuberculosis(T). In addition, an Explainable AI analysis has been implemented.
<br />

## Data
The input data consists of 15470 X-ray images of various sizes that are unbalanced between the 3 classes. Each refers to a patient, and there can be images related to the same patient.

## Preprocessing
To feed the images in the neural networks, several preprocessing steps have been made. Firstly, data has been splitted in training, validation and test set to perform the training and the evaluation of the models. Then, all the images were resized to have the same size of 400 x 400. Next, we defined the data generator to allow the model to be trained with batches of data, improving the training time. Finally, data augmentation has been defined to increase the generalization and the model invariance to various transformations.

## Models
We proposed 3 different models: scratch, InceptionResNetV2, and EfficientNetV2B2 models. The model named "scratch" is a model created by us while the last 2 are models fine-tuned from well-known public networks. Then, we tried to combine the previous models creating a socalled ensemble. We tried 2 different approaches: the
classic approach and the confidence approach.

## Results
The models had quite good performances, with accuracy around 90% for the scratch model, around 95% for the fine tuned networks, and even better using the ensamble models. 

## Explainability
In order to have a better understanding of whether our models really "understood" where to extract features useful for the predictions we implemented 2 techniques related to the field of AI explainability: GradCam and Shapley.

## Conclusions
In this project we built three different models with different characteristics, and we proposed two different ensemble approaches, to be considered according to the usage. The results obtained showed a high level of accuracy, proving the effectiveness of using CNNs for image classification tasks. Additionally, the use of Grad-CAM and Shapley explanation helped provide insight into the decision-making process of the model, enhancing its interpretability and reliability.

## Group Components
| Cognome | Nome | e-mail | Codice Persona |
| --- | --- | --- | --- |
| La Greca  | Michele Carlo | michelecarlo.lagreca@mail.polimi.it | 10864460 |
| Nunziante |  Matteo | matteo.nunziante@mail.polimi.it | 10670132 |
