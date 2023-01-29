We created this YOLOv5 trained model for detecting endangered species of Florida in the wild. Our model was trained on a dataset of close to 800 images including the images of panthers, manatees, sea turtles, key deers and alligators.

The project used YOLOv5 trainer and detector provided by Ultralytics on their github repo <a href="https://github.com/ultralytics/yolov5" target="_blank">here</a>.

The model has been trained on 300 epochs and has some impressive accuracy. The pytorch file for the trained weights can be downloaded from <a href="https://github.com/Dauntlesshokage/Swamphacks1422/tree/main/runs" target="_blank">here</a> from the runs folder in our repository.

To test our custom trained model with your own image or video, you can use the google colab notebook provided by official yolov5 release.
Steps :
1) Follow the link to open <a href="https://colab.research.google.com/github/roboflow-ai/yolov5-custom-training-tutorial/blob/main/yolov5-custom-training.ipynb" target="_blank">google colab notebook</a> 
2) Install the requirements in `requirements.txt` after cloning the yolov5 github repository provided in the step 1 of the notebook.
3) Skip the steps for collecting dataset and training the model since we already have trained weights file to be used for detection. So jump to the "run inference" step 4) Download our `weights.pt` from our runs folder and upload it to working directory in your google notebook by creating a folder under the name `runs` or the name of your choice for the folder(to avoid confusion we used the same name for the folder and refer it to as runs)
5) Run `detect.py` by giving the path (runs/best.pt) for the weights and after the source enter the path of the image or the video you would like to test(upload the image or the video into a folder in the working directory and use the same path).
6) To get your result, go to the path returned by the `detect.py` file and you will find your result saved there.