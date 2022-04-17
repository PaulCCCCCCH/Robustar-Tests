# Test

## Default

| Action                                                            | Expectation                    |
| ----------------------------------------------------------------- | ------------------------------ |
| Navigate to `Validation Data` page under `Inspect Data`           | The image list should be empty |
| Select `Incorrectly Classified` from the dropdown menu at the top | The image list should be empty |
| Navigate to `Test Data` page under `Inspect Data`                 | The image list should be empty |
| Select `Incorrectly Classified` from the dropdown menu at the top | The image list should be empty |

## S1: Normal Flow

| Action                                                                                         | Expectation                              |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------- |
| Navigate to `Test` page -> Click  button `START TESTING ON VALIDATION SET`                     | The task center should have 1 task shown |
| Wait for 30s for the task to finish -> Navigate to `Validation Data` page under `Inspect Data` | 8 images should be displayed             |
| Select `Incorrectly Classified` from the dropdown menu at the top                              |                                          |
| Navigate to `Test` page -> Click  button`START TESTING ON TEST SET`                            | The task center should have 1 task shown |
| Wait for 30s for the task to finish -> Navigate to `Test Data` page under `Inspect Data`       | 8 images should be displayed             |
| Select `Incorrectly Classified` from the dropdown menu at the top                              | 8 images should be displayed             |
