# face_recognition
This repository can be used to detect faces present in the photos and video,

I am using two pre-trained models to achieve this purpose.

Facebox for face detection
Facenet for face-recognition

//Summary

Face Detection is the first and essential step for Face Recognition, and it is
used to detect faces present in images and videos in real-time. Face
Detection is a part of object detection and can be used in many areas such
as security, biometrics, law enforcement, entertainment, personal safety,
culprit detection, etc.

In this deep learning model, firstly the implementation​ ​ of ​ FaceBox​ in
TensorFlow is done that can detect faces present in the image.Rectangles
are drawn around the region of pixels where face is detected.

FaceBoxes: A CPU Real-time Face Detector with High Accuracy​ ,is used
because it solves two major problem:
1)The Problem of visual variation of faces in the cluttered backgrounds.
2)The large search space of possible face positions and face sizes in the
image which imposes a time efficiency requirement.

-Next comes the step of Face Recognition with the use of ​ FaceNet​ ,which is
basically a computer vision task of identifying and verifying a person based
on a photograph of their face.

FaceNet: A Unified Embedding for Face Recognition and Clustering​ ,
is a system that, ​ given a picture of a face, will extract high-quality features
from the face and predict a 128 element vector representation of these
features, called a face embedding.

-​ Face Recognition is applied to the 5-Celebrity Faces Dataset present on
Kaggle.
​ First we use FaceBox onto the dataset, to detect regions of pixels
where face is present, then use FaceNet for creating embeddings from
these faces and then use SVM classifier for face recognition.
