Project Plan and Timeline
==============================

This is a general guideline for the project. The activities and times alotted are recommended estimates only and are subject to changes.


# Deliverables

- Code file
  - Deadline: **Mar 26 by 6p.m.** (this is the deadline shown on Quercus)
  - Format: A single fully-executed Jupyter Notebook

- Presentation
  - Date: TBD. It'll be one of the last 2 classes.
  - Format: 5 PowerPoint slides (excluding title page)
  - Time for presentation: 5 minutes per team member

# Tentative Plan

## Basics and Analysis (by March 6)

- State the problem.

  - What's the target variable we're trying to model?
  - What problem type is this? (E.g., classification, regression, clustering, etc.)
  - What's the main performance measurement metric?
  - What are some essential concepts / terminologies / technical terms and what do they mean?

- Load the dataset.

  - We may need a standard way to load data across the team for consistency.

- Understand basic data structure without data snooping.

  - Datasets available and their relationship
  - Data type (categorical, numeric, image, text, etc.) and features available
  - Sample size
  - If the target variable is categorical, check if there's class imbalance.

- Split the entire dataset into a training set and test set, and then set aside the test set for the end of the project.

  - Make sure not to do any transformation / scaling / normalization
  - If there is class imbalance found earlier, use stratified sampling to do the splitting.
  - At this stage, do not do any transformation or derive variables that can cause data snooping (such as scaling, normalization, average, etc.)

- Do a deeper analysis on the training data to understand the dataset better.

  - Examine the content of the training data.
  - Examine the data's distribution and visualize it where applicable.
  - Identify features that have a strong correlation

- Clean the data if required.

## Training Models (by March 22)

- Engineer additioanl features that might improve model performance.

- Build and train models

    - Identify all the assumptions used and known caveats of the model.
    - Set random seeds so the results can be replicated.
    - Consider creating a benchmark model to see the minimal performance expected.
    - [Optional] Aside from the loss function, include other relevant metrics to measure different aspects of the model.
    - Consider using k-fold cross validation.
    - Assess model performance during training.
    - Check for overfit
    - Tune the model
    - Dimensionality reduction
    - Remove correlated features

- Compare the models and identify the promising ones.

- Evaluate model performance by passing in the test set left out earlier in the project. **Do not do any further model tuning afterwards.**


## Nice-To-Have

These are topics we can explore if we do have time after completing the essential items above. If there is not enough time, we can skip these.

- Create an ensemble of the better-performing models.
- Train models that are efficient. Please refer to the [description in Kaggle](https://www.kaggle.com/competitions/pii-detection-removal-from-educational-data/overview/efficiency-prize-evaluation) for details.


## Prepare for the Presentation (by March 25)

- Write the presentation slides
- Rehearse for the presentation