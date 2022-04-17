# Auto Annotation

## Default 

| Action                                                        | Expectation                                                  |
| ------------------------------------------------------------  | ------------------------------------------------------------ |
| Navigate to `Auto Annotate` page                              | Expect 0 task in the task panel                              |
| Delete the default input number 0 and input 5                 | 
| Click on `START AUTO ANNOTATION`, wait for the task panel.    | Expect 1 task in the task panel                              |
| Click on `Annotated Data` under `Inspect Data`                | Expect to see 5 images


## S1: Delete the only one task

| Action                                                       | Expectation                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Navigate to `Auto Annotate` page                             | Expect 0 task in the task panel                              |
| Delete the default input number 0 and input 50               | Expect 0 task in the task panel                              |
| Click on `START AUTO ANNOTATION`, wait for the task panel.   | Expect 1 task in the task panel                              |
| Click the `Task Panel` icon and delete the task              | Expect 0 task in the task panel                              |


## S2: Input an out-of-bounds number 

| Action                                                        | Expectation                                                  |
| -------------------------------------------------------       | ------------------------------------------------------------ |
| Navigate to `Auto Annotate` page                              | Expect 0 task in the task panel                              |
| Delete the default input number 0 and input 9999              | Expect run 1 task with the length of the dataset 
| Click on `START AUTO ANNOTATION`, wait for the task panel.    | Expect 1 task in the task panel                              |


## S3: Input an String

| Action                                                        | Expectation                                                  |
| -------------------------------------------------------       | ------------------------------------------------------------ |
| Navigate to `Auto Annotate` page                              | Expect 0 task in the task panel                              |
| Delete the default input number 0 and input "abc"             | Expect prompt: Auto annotation failed to start
| Click the `Task Panel` icon and delete the task               | Expect 0 task in the task panel                              |
 