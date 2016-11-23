# VSST 
Here we provide the code for the following paper:

    Imbalanced Video Summarization via Spatio-Temporal Deep Architecture, paper id #860, CVPR 2017
    
### Updates
- Nov 21, 2016
  * Release the first version VSST (branch: master) compatible with [caffe toolbox](https://github.com/yjxiong/caffe)

### Two-stream deep ConvNet trained on the SumMe and CLA dataset
First, we provide our trained two-stream CNN models on the SumMe dataset, 

["Spatial net model (VSST-RGB&MV)"](https://drive.google.com/file/d/0B7XqN7JTUuAlemhwOTI1c2hJZEk/view?usp=sharing) </br> 
["Temporal net model (VSST-RGB&MV)"](https://drive.google.com/file/d/0B7XqN7JTUuAlcGtnQnlUcV8wVlk/view?usp=sharing) </br>
["Spatial net model (VSST-imbalance)"](https://drive.google.com/file/d/0B7XqN7JTUuAlRFlTc0JjYWdTOFE/view?usp=sharing) </br> 
["Temporal net model (VSST-imbalance)"](https://drive.google.com/file/d/0B7XqN7JTUuAlbHJvTGtuT3NSM2s/view?usp=sharing) </br>

and CLA dataset.

["Spatial net model (VSST-RGB&MV)"](https://drive.google.com/file/d/0B7XqN7JTUuAlUjR4eC1TRDdEMUE/view?usp=sharing) </br> 
["Temporal net model (VSST-RGB&MV)"](https://drive.google.com/file/d/0B7XqN7JTUuAlYmo0cDQ0c09WbE0/view?usp=sharing) </br>
["Spatial net model (VSST-imbalance)"](https://drive.google.com/file/d/0B7XqN7JTUuAlakZybnBjZkVqLVE/view?usp=sharing) </br> 
["Temporal net model (VSST-imbalance)"](https://drive.google.com/file/d/0B7XqN7JTUuAldkpMYkp4N0ptc1k/view?usp=sharing) </br>


### VSST demo code
Here, a matlab demo code for VSST is provided.

- **Step 1**: RGB Extraction </br>
You need extract the RGB frames of the video by yourself. 
- **Step 2**: MV Extraction </br>
You need download the motion vector code and compile it by yourself. [Motion Vector](https://github.com/zbwglory/MV-release)
- **Step 3**: caffe  </br>
You need download the public caffe toolbox. Our VSST code is compatatible  with [caffe toolbox](https://github.com/yjxiong/caffe). </br>
- **Step 4**: train two-stream deep Convnet  </br>
- **Step 5**: Extract feature for each video frame through two-stream deep ConvNet </br>
- **Step 6**: use SVR to predict the summmary score for each frame </br>
