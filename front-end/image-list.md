# Image List

## Default 

| Action                                                       | Expectation |
| ------------------------------------------------------------ | ----------- |
| Navigate to `Test` page, click on `START TESTING ON VALIDATION SET` and  `START TESTING ON TEST SET`, wait for both to finish. |             |



## S1: Train Page Navigation

| Action                                                       | Expectation                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Navigate to `Training Data` page under `Inspect Data`        | session storage has entry {"train": 0}; Page number is 0     |
| Click `NEXT PAGE` twice.                                     | Session storage has entry {"train": 2}; `Page Number` is 2   |
| Select `cat` in the `Class Name` dropdown and click on `GOTO CLASS`. | Session storage has entry {"train": 125}; `Page Number` is 125 |
| Input 9999 to`Page Number` and click `GOTO CLASS`            | Session storage has entry {"train": 1124}; `Page Number` is 1124; `NEXT PAGE` is disabled. |
| Click `PREV PAGE` twice.                                     | Session storage has entry {"train": 1122}; `Page Number` is 1122 |

## S2: Test/Validation Page Navigation

| Action                                                  | Expectation                                                  |
| ------------------------------------------------------- | ------------------------------------------------------------ |
| Navigate to `Validation Data` page under `Inspect Data` | Session storage has entry ("train": 1122), and ("validation_correct": 0); `Page Number` is 0 |
| Select `Incorrectly Classified` in the top dropdown.    | Expect 8 images on the page.                                 |
| Input 9999 in `Page Number` and click `GOTO PAGE`       | `NEXT PAGE` disabled; `Page Number` > 0.                     |
| Select `Correctly Classified` in the top dropdown.      | Expect 8 images on the page; `Page Number` = 0.              |