# Hand Gesture Recognition App


## Installation:
1. Install Open CV manager into your phone from Playstore.
2. Open the project (not import)
3. Install if there are missing dependancies needed.

## Usage:

1. The first mode you are in upon starting the app is background sampling mode. You can lower the resolution using the option in the menu to make the app run faster. After finished, just touch the screen and you will be in the second mode: hand sampling mode. You need to cover the seven squares with your hand. This step is crucial to the performance and I suggest you bend your hand a little so that the shadow could also be sampled. 

2. After presampling you can touch the screen again and go into next mode to see the segmented hand. Touch again and you can see the extracted features, along with three buttons. In this mode you can add new gestures to the gesture database, train the SVM model or begin testing. The deletion of gestures has not been implemented yet so be careful when you want to add a new one. All the data of the gestures are stored in the ExternalStorageDirectory/MyDataSet folder. If you don't know the location on your phone, just click "Add Gesture" button and try to add a new gesture, the folder will be generated automatically in the external storage directory. You can use the existing data set which is located in the project directory. You can click "Test" button to see the realtime recognition performance of SVM classifier, but make sure the model has already been generated, i.e., trained. 

3. To add a new gesture to the training set, simply make a static gesture before the camera and click "Add Gesture" button. If you want to increase the number of a gesture that is already in the training set, you need to click "Data Collection" in the menu and choose the image representing the gesture, and then click "Add Gesture" button. After you click that button, the app will start gathering data immediately for a certain number of frames(currently the number is set to be 10). Finally a dialog will pop up asking you wheather to save those data or not.

4. This app can also let you quickly launch other apps using gestures. But first you need to map your gestures to the apps by selecting "Map Apps" in the menu. The selection is stored in the app so you don't need to map it every time you run the app. Then you can test it by choosing the "App Test" in the menu.

A demo of the app can be found on YouTube: http://youtu.be/PF6hY-0VuN4

Project page: http://eaglesky.github.io/2015/12/26/HandGestureRecognition/ 


