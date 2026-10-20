# Enviroment

After the creation of an enviroment. FiftyOne and huggingface_hub should be installed.

*In VScode run*

*Code:*

import fiftyone as fo
import fiftyone.utils.huggingface as fouh

dataset = fouh.load_from_hub(
    "Voxel51/Coursera_lecture_dataset_train",
    dataset_name="lecture_dataset_train",
    persistent=True
    )

test_dataset = fouh.load_from_hub(
    "Voxel51/Coursera_lecture_dataset_test",
    dataset_name="lecture_dataset_test",
    persistent=True
    )

dataset.compute_metadata()

test_dataset.compute_metadata()

After this the dataset should be downloaded and ready to go.
