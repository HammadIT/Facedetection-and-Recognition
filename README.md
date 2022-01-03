# Facedetection-and-Recognition
Bolly wood stars image detector, 
Image dataset can be downloaded form kaggle
ALL OpenCV or other machine learning models that has the ability to predict human 
face or human follows following 4 principles.
1) From Video or image we have to locate where the face is.
2) Model extract unique features of someone face, like a human being does, it may be nose, ear, moustache and color etc
3) Becuase A person may very due to different lightening or shaved unshaved etc, model eliminate that features.
4) Compare Face features with all other features which are seen or learned by machine learning model.
5) Finally it tells this is the face of which person.

EigenFace Recognizer:
Because not all elements of a face are equally significant or useful for facial recognition, our method takes that into account. When you look at someone,
you can tell who they are by their distinguishing characteristics, such as their eyes, nose, cheeks, or forehead, and how they differ from one another.
It only target the area of maximun change. Like human being detect the change
by looking at nose to eye, or cheek to chin, so it used only area of maximum chage
and discard useless componenets. These components are called principal componenets
1) Extract principal componenets
2) Compare these with all training examples
3) And find bext match, return that face

Fisherface Recognizer:
As Eigen Face took all traing images as whole and then find principal components,
So it is not focused on deatuers that differenitate oneperson from other
It's worth noting that FisherFaces only prevents one person's features from becoming dominant, but it still deems lighting changes to be a good feature. We already know that light variation isn't a helpful 
feature to extract because it's not a component of the face.


LBPH Recognizer:
We know that light affects both Eigenfaces and Fisherfaces, and we can't always expect perfect light conditions in real life. The LBPH face recognizer is a step forward in overcoming this flaw.
The goal of LBPH is to determine the image's local structure by comparing each pixel to its neighbours, rather than looking at the image as a whole.
Histogram for each image is calculated, Then that histogram is matched with the histogram of images that are alredy present, best match will represent class.
LBPH is not affected by lightening conditions.

SVM:
Support Vector Machines (SVM) are classified as classification algorithms, however they can be used to solve both classification and regression issues. 
It can handle both continuous and categorical variables with ease. To differentiate various classes, SVM creates a hyperplane in multidimensional space.
 SVM iterativelygenerates the best hyperplane, which is then utilised to minimise an error.

Logistic Regression:
It is same as linear regression where we are trying to find relation between independent and dependent variables. It is calculated by slope and intercept when model help us to calculate both of above.
 But when there is categorical output/class, two classes here we used logistic regression. Logistic regression is used to return probability of each class against each set of attributes.
This can be used for multi classification purposes.



LDA is a multi-class classification predictive modelling algorithm. 
It can also be used as a dimensionality reduction technique, generating a projection of a training dataset that best divides the samples according to their class.
