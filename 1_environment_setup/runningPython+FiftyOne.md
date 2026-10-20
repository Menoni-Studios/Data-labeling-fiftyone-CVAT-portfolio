# Import libraries

The most use libraries are: FiftyOne, pandas, opencv, numpy, matplotlib, scikit scikit-image= seaborn, cvat,  scipy, snorkel, pytorch, sci-kit-learn, tensorFlow.

*Code:*

import fiftyone as fo
import fiftyone.utils.huggingface as fouh

# Load the dataset

*Code:*

//In this case the dataset is loaded from Huggingface

dataset = fouh.load_from_hub(
    "Voxel51/Coursera_lecture_dataset_train",
    dataset_name="lecture_dataset_train",
    persistent=True
    )

# Launch the App

*Code:*

//This will lunch FiftyOne with the dataset for a quick visual view

session = fo.launch_app(Voxel51/Coursera_lecture_dataset_train)

![Website Screenshot](../assets/1.png)
