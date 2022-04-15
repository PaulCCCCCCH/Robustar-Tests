# Train

## Default

| Action                                                       | Expectation |
| ------------------------------------------------------------ | ----------- |
| Navigate to `Train` page by clicking on `Train` tab on the left |             |

## S1: Training

Leave to docker test. Need file system manimulation (e.g., check disk for checkpoint), which cannot be handled at the frontend.

## S2: Epoch and Batch Size

| Action                                        | Expectation                                                  |
| --------------------------------------------- | ------------------------------------------------------------ |
| Set `Batch size` to 128                       |                                                              |
| Set `epoch` to 1                              |                                                              |
| Click `START TRAINING` and wait for some time | Task center displays "x/71", where x should be any number > 2. |
| Cancel the task in task center.               | Task center becomes empty.                                   |
| Set `epoch` to 5                              |                                                              |
| Click `START TRAINING` and wait for some time | Task center displays "x/71", where x should be any number > 2. |
| Cancel the task in task center.               | Task center becomes empty.                                   |

## E1: Zero Epoch

| Action                                          | Expectation                                                 |
| ----------------------------------------------- | ----------------------------------------------------------- |
| Set `Epoch` to 0 and click on `START TRAINING`. | A new tab (localhost:6006) is opened. Task center is empty. |