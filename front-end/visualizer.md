# Visualizer

## Default

| Action                                                       | Expectation |
| ------------------------------------------------------------ | ----------- |
| Navigate to `Training Data` page under `Inspect Data` | Image List should be shown out  |
| Mouse over the first image in the image list on the right | A hover window appears with the `ANNOTATE` and `PREDICT` buttons. |
| Click `PREDICT` button       | The `Visualizer` list on the right will pop up. |

## S1: View Model Prediction

| Action                                                       | Expectation |
| ------------------------------------------------------------ | ----------- |
| Click on the `Model Prediction` column | The `Model Prediction` panel pops up and the bar chart is successfully displayed. The order of similarity is from top to bottom in descending order, with the maximum value not exceeding 1 and the minimum value not less than 0.|
| Click on the `Model Prediction` column | `Model Prediction` panel will be put away. |

## S2: View Model Focus

| Action                                                       | Expectation |
| ------------------------------------------------------------ | ----------- |
| Click on the `Model Focus` column | The `Model Focus` panel pops up and successful presentation of four Flash torch visualizations results |
| Click on the `Model Focus` column | `Model Focus` panel will be put away. |


## S3: View Influence Images

| Action                                                       | Expectation |
| ------------------------------------------------------------ | ----------- |
| Click on the `Influence Images` column | The `Influence Images` panel pops up with a corresponding message |
| Click on the `Influence Images` column | `Influence Images` panel will be put away. |

## S4: View Proposed Annotation

| Action                                                       | Expectation |
| ------------------------------------------------------------ | ----------- |
| Click on the `Proposed Annotation` column | The `Proposed Annotation` panel pops up and shows one proposed annotation image |
| Click on the `Proposed Annotation` column | `Proposed Annotation` panel will be put away. |

## S5: Test single page panel expansion/closing

| Action                                                       | Expectation |
| ------------------------------------------------------------ | ----------- |
| Click on the `Model Prediction` column | The `Model Prediction` panel pops up |
| Click on the `Model Focus` column | The `Model Focus` panel pops up and the `Model Prediction` panel remains expanded. |
| Click on the `Influence Images` column | The `Influence Images` panel pops up, the `Model Focus` and  `Model Prediction` panels remain expanded.|
| Click on the `Influence Images` column | `Influence Images` panel will be put away, the `Model Focus` and  `Model Prediction` panels remain expanded. |
| Click on the `Proposed Annotation` column | The `Proposed Annotation`, `Model Focus` and  `Model Prediction` panels are the expanded states, `Influence Images` panel is closed state. |

## S6: Test the expansion/closing of panels during image conversion

Click on the first image in the `Image List`, keep the visualizer list to be the `Proposed Annotation`, `Model Focus` and  `Model Prediction` panels are the expanded states, `Influence Images` panel is closed state.

| Action                                                       | Expectation |
| ------------------------------------------------------------ | ----------- |
| Click on the second image in the `Image List` | The visualizer list still keeps the `Proposed Annotation`, `Model Focus` and  `Model Prediction` panels are the expanded states, `Influence Images` panel is closed state. The relevant data all become based on the second image. |

## S7: Test the expansion/closing of panels during page conversion

Click on the first image in the `Image List`, keep the visualizer list to be the `Proposed Annotation`, `Model Focus` and  `Model Prediction` panels are the expanded states, `Influence Images` panel is closed state.

| Action                                                       | Expectation |
| ------------------------------------------------------------ | ----------- |
| Click on `Test Data` in left sidebar| The visualizer list still keeps the `Proposed Annotation`, `Model Focus` and  `Model Prediction` panels are the expanded states, `Influence Images` panel is closed state. The content in the list is not change. |
