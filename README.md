# ObjectDetection
Object detection using Yolo v3 algorithm on DeepFashion Dataset. The model is able to predict objects of 50 different categories by creating a bounding box around the object. This is based on the code https://github.com/AntonMu/TrainYourOwnYOLO

<b> Training the model</b>

python Train_YOLO.py --annotation_file 'training_data.txt' --classes_file 'deepfashion.name' --epochs 5 --weights_path 'trained_weights_final.h5'

<b> Prediction </b>

python Detector.py --input_path 'test_images' --output 'det2'  --box_file 'det2/Detection_Results0427.csv' --classes 'deepfashion.name' --no_save_img --yolo_model 'models/trained_weights_final.h5'
