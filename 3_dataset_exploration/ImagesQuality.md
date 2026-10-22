### Image quality directly affects annotation accuracy and model performance. This section evaluates brightness, blurriness, and contrast across the dataset to identify potential issues that may impact downstream tasks.

#### ☑️Dataset

It is compose of 16,638 where 210 are underexposed, 143 are overexposed, 23 are low‑contrast, and 68 are blurry. These are small fractions of the dataset and will not affect the performance of the model.

#### ☑️Brightness analysis

Most images fall into a mid‑brightness range, but a noticeable portion is underexposed. Dark images reduce labeler visibility and can cause missed objects or inaccurate bounding boxes.

Most images are mid-range in brightness clustering around mean intensities near ~75–150. Very few images are extremely dark or extremely bright, so exposure is generally acceptable.

![Brightness distribution](../assets/brightnessDis.png)

#### ☑️Blurriness analysis

A subset of images shows high blur levels, likely due to motion or focus issues. Blurry images make object boundaries harder to identify, increasing annotation inconsistency.

The majority of images show low  blurriness, with counts falling rapidly as sharpness increases. While many images are not perfectly sharp, only a modest number exceed high‑sharpness thresholds so is acceptable.

![Blurriness](../assets/BlurrinessDis.png)

#### ☑️Contrast analysis

Low‑contrast images reduce object separability from the background. This can lead to ambiguous annotations and lower model confidence during training.

Contrast values concentrate in a moderate range , with a bell‑shaped distribution around the dataset mean. Very low‑contrast images are rare.

![Contrast](../assets/ContrastDis.png)
