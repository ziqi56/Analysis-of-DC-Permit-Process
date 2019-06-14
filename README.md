To replicate the outcome of our analysis, scripts in the code folder of our repository need to be
run in the following sequence:
1. data_merging.ipynb -- the code merges the DCRA and CAMA datasets
2. data_cleaning_per_permit.ipynb -- the code cleans the merged dataset treating missing
values and transforming variables. It also creates relevant variables like agency dummies,
etc. The output csv forms our primary data which we use for the subsequent analysis
3. data_description.ipynb -- Describes the main variables in the merge dataset on the csv
generated in step 2.
4. ROC_curve.ipynb -- the code performs a comparative analysis of all potential models we
are considering on the csv generated in step 2.
5. decisiontree_model.R -- the code models the dataset using the Decision tree classifier on
the csv generated in step 2. The output is the decision tree plot and variable importance
plot.
6. logit_model.ipynb -- the code models the dataset using the Logistic model on the csv
generated in step 2.
