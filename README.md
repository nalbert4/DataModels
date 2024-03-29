# DataModels
A Model to Predict Annual Claims Data Costs for Patients with Diabetes and Additional Chronic Disease
By Nisa Albert and Marilyn Zeppetelli 

Our project created two main data models to predict claims costs for Type 2 Diabetes Medicare patients with additional chronic diseases. For our project, we will use the Data Entrepreneur’s Medicare Claims Synthetic Public Use Files (DE-SynPUFs) for our analysis.  Two data models were used Multiple Linear Regression in the first build and the three models (Ridge, Lasso, and Elastic-Net) in the second build. We used R programming language to construct the data models. Our results illustrate that there is some relation among the variables but for future implementation a stronger relationship among the predictor variables is needed to build an effective data model to predict costs. Also, more quantitative predictor variables are needed.
We used the DE-SynPUFs for our analysis because it contains anonymous data of the beneficiaries to protect their privacy. It is also a common dataset that is used for creating data models without using actual Medicare data. The Data Entrepreneur’s Synthetic Public Use File data was created from actual Medicare and Medicaid beneficiary data.  The synthetic data variables were then masked by mixing beneficiary information from similar but different ‘donor’ beneficiaries, changing variable values within claims where the data could disclose identifiable information about the beneficiary.  File underwent a Synthetic File Creation Process and various methods were used by CMS to generate the synthetic data, including hot decking-based procedures, variable reduction/suppression/substitution/imputation, and data perturbation to mask timelines and intervals between events. The data files for the models are .csv files that were already pre-processed and ready to be used for the data model.
R programming as it has packages for running data models. 
Instructions for Running both data models in R:

Multiple Linear Regression Model code in R:
1.	Download these files: "2008_benef_model.csv", "2008_benef_model_orginal.csv" and "Multiple_Linear_Regression.rmd" and save in one folder.
2.	Open the “Multiple_Linear_Regression.Rmd” file in R to edit the setwd() command.
3.	There are two setwd() commands, please alter the commands to your working directory where all the files for the project are installed.
4.	To Run the file, click on the first line in the R code and select "Run Current Chunk" or "Run All" to run the entire R code for the model.
5.	Output will display 4 graphs: Residual vs Fitted, Normal Q-Q, Scale Location, Residuals vs Leverage.
6.	It will also display actual vs predicted predictor values to compare the accuracy of the model.

Three Models (Ridge, Lasso, and Elastic-Net) code in R:
1.  Download the “DE1_0_2008_Beneficiary_Summary_File_Sample_2_Reduced.csv” and “Ridge_Lasso_ElasticNet.Rmd".
2.  Open the “Ridge_Lasso_ElasticNet.Rmd” R Markdown file in R Studio.
3.  On line 16, alter the fully qualified filename to the correct directory location where the data file has been saved on your computer.
4.  To Run the file, click on the “Run” drop down menu and select “Run All”.
5.  The output for each code section will appear directly below that chunk of code in the main window.  Scroll through the main window to see the output for each chunk of code. Please note that there may be multiple output frames that you can click on in each output section to see the various command outputs.

It is important to note, that this analysis was undertaken using synthetic Medicare data.   If the models created here could run with actual Medicare data, then the output would be more useful to analyze.  The synthetic Medicare data we used provided a very useful means for learning how to utilize data to predict Medicare costs. 




