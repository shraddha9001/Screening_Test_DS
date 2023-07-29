# Screening_Test_DS
1) Read the target and type of regression to be run
 
2) Read the features (which are column names in the csv) and figure out what missing imputation needs to be applied and apply that to the columns loaded in a dataframe
 
3) Compute feature reduction based on input. See the screenshot below where there can be No Reduction, Corr with Target, Tree-based, PCA. Please make sure you write code so that all options can work. If we rerun your code with a different Json it should work if we switch No Reduction to say PCA.
 
4) Parse the Json and make the model objects (using sklean) that can handle what is required in the “prediction_type” specified in the JSON (See #1 where “prediction_type” is specified). Keep in mind not to pick models that don’t apply for the prediction_type specified
 
5) Run the fit and predict on each model – keep in mind that you need to do hyper parameter tuning i.e., use GridSearchCV
 
6) Log to the console the standard model metrics that apply
7) NOTE: Please write generic code that can parse any JSON that follow this JSON format. So goal is you are using generic function in python.
It will be most efficient if you use sklean pipelines for each stage namely a) feature handling part b) feature reduction part and c) model fit with grid search cv so that you can execute the pipeline object. For your testing try and change the fields in the JSON like say enable some algos setting ‘is_selected’ to true and now that algo should get executed when you run your script again. 

