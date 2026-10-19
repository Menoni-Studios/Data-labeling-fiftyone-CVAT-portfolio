
# Import libraries 
import fiftyone as fo
import fiftyone.utils.huggingface as fouh

# Load the dataset from Hugging Face if it's your first time using it

dataset = fouh.load_from_hub(
    "Voxel51/Coursera_lecture_dataset_train", 
    dataset_name="lecture_dataset_train", 
    persistent=True
    )

# Launch the App
session = fo.launch_app(cloned_dataset)

# Profling FityOne dataset

1-Basic dataset information: Getting an overview of the dataset size and structure.

2-Sample examination: Looking at individual samples to understand their fields and content.

3-Detection statistics: Analyzing the number and distribution of detections across the dataset.

4-Label distribution: Examining the frequency and variety of labels in our dataset.

5-Image resolution analysis: Understanding the typical sizes of images in our dataset.

6-Advanced profiling: Using FiftyOne's built-in tools for comprehensive dataset analysis.

