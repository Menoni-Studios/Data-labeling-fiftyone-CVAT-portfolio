
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

![Website Screenshot](../assets/1.png)

# Profling FityOne dataset


