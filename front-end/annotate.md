# Annotate

## S1: Normal Flow

| Action                                                                                                                 | Expectation                                                                       |
| ---------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| Navigate to `Training Data` page under `Inspect Data` -> Click button `Annotate` on the first image                    | The item `split` in session storage should have value "train"                     |
| Click button `Send Edit` for 3 times -> Wait for loading                                                               | Success -> The value of item `image_url` in session storage should increment by 3 |
| Navigate to `Annotated Data` page under `Inspect Data`                                                                 | 3 images should be displayed                                                      |
| Click button `Annotate` on the first image -> Click button `Send Edit` twice -> Navigate back to `Annotated Data` page | 3 images shown should be the same and in the same order                           |

## S2: Editing Validation Set

| Action                                                                                                                            | Expectation                                                            |
| --------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| Navigate to `Validation Data` page under `Inspect Data` -> Click button `Annotate` on the first image -> Click button `Send Edit` | Failure (Annotated image should not be modified again)                 |
| Navigate to `Test Data` page under `Inspect Data` -> Click button `Annotate` on the first image -> Click button `Send Edit`       | The value of item `image_url` in session storage should increment by 3 |
