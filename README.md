## Gold Recovery Prediction Model

This repository contains a machine learning model developed for [Zyfra](https://www.zyfra.com/), a company specializing in providing efficient solutions for the mining, oil and gas, chemical, and engineering industries. The project uses linear regression and random forest models to predict the amount of gold recovered from gold ore using extraction and purification data.

## Background

Gold recovery involves a series of stages including flotation and purification. The flotation process separates gold ore mixture into rougher gold concentrate and tails. Subsequently, the rougher concentrate undergoes purification stages to yield a final concentrate with higher gold content. The stability of the process is crucial and depends on the state of the flotation pulp.

## Data Description

The dataset includes various parameters and features related to the gold recovery process. Here's a brief overview:

### Technological Process
- Rougher Feed: Raw material input.
- Rougher Additions: Flotation reagents including Xanthate (promoter or flotation activator), Sulphate (sodium sulphide for this process), and Depressant (sodium silicate).
- Rougher Process: Flotation process carried out in float banks to separate gold ore mixture.
- Rougher Tails: Residues from the rougher process.
- Cleaner Process: Further purification stages.
- Rougher Au: Rougher gold concentrate.
- Final Au: Final gold concentrate.

### Parameters of Stages
- Air Amount: Volume of air used in the process.
- Fluid Levels: Levels of fluids involved.
- Feed Size: Particle size of the feed material.
- Feed Rate: Rate of feed input.

## Data Preprocessing and Analysis

Python libraries such as Pandas, Matplotlib, and Scikit-learn are used for data analysis and preprocessing. This includes handling missing values, comparing train and test sets, and removing unnecessary features. Visuals like line graphs and box and whisker plots are incorporate to help understand the distributions of concentrations of substances.

## Model Building

I train two models for predicting the rougher and final gold recovery outputs: **Random Forest and Linear Regression**. Cross-validation is employed to assess model performance, and the symmetric Mean Absolute Percentage Error (sMAPE) is calculated to evaluate predictions against actual values.

## Results

After thorough analysis and model training, the Random Forest model was found to perform better for predicting final gold recovery, while Linear Regression was more effective for predicting rougher gold recovery. 

## Future Improvements

- Further tuning of hyperparameters to enhance model performance.
- Exploration of additional features that may contribute to better predictions.
- Integration of the model into Zyfra's existing systems for real-time predictions and decision-making.

## Acknowledgements

I would like to thank Zyfra and TripleTen Data Science bootcamp for providing the dataset and task.
