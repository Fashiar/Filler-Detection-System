# Filler-Detection-System
Filler Detection System (FDS) to Detect, Classify, and Segment the Composite Fillers (Fibers and Particles)

Here, we used the Mask-RCNN as the backbone of FDS to classify, detect and segment two types of fillers (fibers and particles) from artifically generated SEM images. To run the demo successfully, follow the steps shown below:

1. Run the "simulate_image_with_annotation.py" file to synthesize the images

      -It will create the necessary images and their corresponding masks
      
      -It will also create the .JSON annotation file
      
           Following are the structure of the dataset 
            dataset
              |--train
                  |--images
                  |--masks
              |--val
                  |--images
                  |--masks
              |--test
                  |--images
          
2. Clone the matterport Mask_RCNN repository from https://github.com/matterport/Mask_RCNN
3. Install the pycocotools as demonstrated in https://github.com/matterport/Mask_RCNN
4. Run the "filler_detection_system.ipynb" file to train and testing
In case of failing to open the "train_mrcnn.ipynb" file here, go to: https://nbviewer.jupyter.org/ and paste https://github.com/Fashiar/Filler-Detection-System/blob/main/filler_detection_system.ipynb to the viewer tab

Due to the storage size, we did not uplaod the train and test images. However you will able to generates images using "simulate_image_with_annotation.py" file.

Acknowledgement: Thanks to Emmersive-limit to give the idea of image systhesis for coco-like dataset
