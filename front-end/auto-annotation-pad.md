# Auto Annotation

## Default 

| Action                                                        | Expectation                                                 |
| ------------------------------------------------------------  | ------------------------------------------------------------|
| Navigate to `Auto Annotate` page                              | Expect 0 task in the task panel                             |
| Delete the default input number 0 and input 5                 |
| Click on `START AUTO ANNOTATION`, wait for the task panel.    | Expect 1 task in the task panel                             |
| Click on `Annotated Data` under `Inspect Data`                | Expect to see 5 images                                      |
| Click on the first image in the image list                    | Expect to have split: annotated                             |



## S1: Delete the only one task

| Action                                                       | Expectation                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Navigate to `Auto Annotate` page                             | Expect 0 task in the task panel                              |
| Delete the previous input number and input 500               |                                                              |
| Click on `START AUTO ANNOTATION`, wait for the task panel.   | Expect 1 task in the task panel                              |
| Click the `Task Panel` icon and delete the task              | Expect 0 task in the task panel                              |



## S2: Input Zero

| Action                                                       | Expectation                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Navigate to `Auto Annotate` page                             | Expect 0 task in the task panel                              |
| Delete the previous input number and input 0                 |                                                              |
| Click on `START AUTO ANNOTATION`, wait for the task panel.   | Expect 0 task in the task panel                              |
| Click the `Task Panel` icon                                  | Expect to have text "No task is running now."                |


## S3: Input Zero Before Integer

| Action                                                       | Expectation                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Navigate to `Auto Annotate` page                             | Expect 0 task in the task panel                              |
| Delete the previous input number and input 0100              |                                                              |
| Click on `START AUTO ANNOTATION`, wait for the task panel.   | Expect 0 task in the task panel                              |
| Click the `Task Panel` icon                                  | Expect 1 task in the task panel and a dataset of length 100  |



## S4: Input an out-of-bounds number 

| Action                                                        | Expectation                                                  |
| -------------------------------------------------------       | ------------------------------------------------------------ |
| Navigate to `Auto Annotate` page                              | Expect 0 task in the task panel                              |
| Delete the default input number 0 and input 9999              | Expect 1 task in the task panel                              |
| Click on `START AUTO ANNOTATION`, wait for the task panel.    | Expect 1 task in the task panel                              |
| Click the `Task Panel` icon                                   | Expect a dataset of length 9000                              |



## S5: Input a Floating Point Number

| Action                                                        | Expectation                                                  |
| -------------------------------------------------------       | ------------------------------------------------------------ |
| Navigate to `Auto Annotate` page                              | Expect 0 task in the task panel                              |
| Delete the default input number 0 and input 9.9               | Expect 1 task in the task panel                              |
| Click on `START AUTO ANNOTATION`, wait for the task panel.    | Expect 0 task in the task panel                              |
| Click the `Task Panel` icon                                   | Expect to have text "No task is running now. "               |
                                                                                  
 

## S6: Test Start index be negative number

| Action                                                        | Expectation                                                  |
| -------------------------------------------------------       | ------------------------------------------------------------ |
| Navigate to `Auto Annotate` page                              | Expect 0 task in the task panel                              |
| Delete the default input number 0 and input -1                | Expect 1 task in the task panel                              |
| Click on `START AUTO ANNOTATION`, wait for the task panel.    | Expect 0 task in the task panel                              |
| Click the `Task Panel` icon                                   | Expect to have text "No task is running now."                |
                                                                                  

## S7: Test End index be less than -1

| Action                                                        | Expectation                                                  |
| -------------------------------------------------------       | ------------------------------------------------------------ |
| Navigate to `Auto Annotate` page                              | Expect 0 task in the task panel                              |
| Delete the default input number 0 and input -2                | Expect 1 task in the task panel                              |
| Click on `START AUTO ANNOTATION`, wait for the task panel.    | Expect 0 task in the task panel                              |
| Click the `Task Panel` icon                                   | Expect to have text "No task is running now."                |
                                               


## S8: Test End index be less than Start index

| Action                                                        | Expectation                                                  |
| -------------------------------------------------------       | ------------------------------------------------------------ |
| Navigate to `Auto Annotate` page                              | Expect 0 task in the task panel                              |
| Delete the start index default 0 and input 99999              | Expect 0 task in the task panel                              |
| Delete the end index default -1 and input 99998               | Expect 1 task in the task panel                              |
| Click on `START AUTO ANNOTATION`, wait for the task panel.    | Expect 0 task in the task panel                              |
| Click the `Task Panel` icon                                   | Expect to have text "No task is running now."                |


                                               