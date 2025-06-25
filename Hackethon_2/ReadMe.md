
1. About Dataset
  The National Health and Nutrition Examination Survey (NHANES) is a nationally representative health study conducted by the CDC’s National Center for Health Statistics. 
  It uniquely combines interviews, physical exams, and lab tests to assess the health and nutritional status of U.S. children and adults. 
  This dataset is a subset, focused part of the NHANES study by CDC, which looks at health and nutrition trends in the U.S. 
  It has 6,287 entries and 7 key features: covering things like body stats, lifestyle, and lab results. 
  The task is simple: predict if a person is a senior (65+) or not. NHANES collected data through home visits, mobile clinics, and lab tests, giving a good mix of real and reported info. 
  This trimmed version keeps only what’s needed, making it perfect for health-based age prediction.

 

*  This Hackathon is in collaboration with by Consulting and Analytics Club, IIT Guwahati for Summer Analytics 2025. *
2. About data:
  The data contains two files: train.csv and test.csv

     train.csv - which contains the training set observations. 2,016 rows, which have the target variable (age_group) values as well for training the model.

     test.csv - which contains the testing set observations. 312 rows, with the target column missing. Use the trained model to predict and submit the values of the target column.


   Additionally, a sample-submission.csv file is provided to show you what your CSV submission should look like.
   Note that the header has 'age_group' for the column name and the number of rows is equal to the number of rows in the test set.

  Respondents 65 years old and older were labeled as “Senior” and all individuals under 65 years old as “Adult”. 

  Make sure to mark Adult as 0 and Senior as 1. This is important. Look at sample submission file, it accepts only 0 or 1. 

3. Target Variable Classes:
  age_group: Adult - 0

  age_group: Senior - 1


3.Features:
  The dataset contains the following features:

  SEQN: Sequence number (identifier)

  RIAGENDR: Respondent's Gender (1=Male, 2=Female)

  PAQ605: Physical activity questionnaire response: If the respondent engages in moderate or vigorous-intensity sports, fitness, or recreational activities in the typical week

  BMXBMI: Body Mass Index

  LBXGLU: Glucose level

  DIQ010: Diabetes questionnaire response

  LBXGLT: Glucose tolerance (Oral)

  LBXIN: Insulin level


Note: The dataset may contain missing values (NaN) which should be handled appropriately. In case of same scores, the top-5 will be selected based on Featuring Engineering and EDA approach.

Disclaimer: We don't own this data, we have modified/pre-processed few of the data points for this Hackathon for students to try classification ML algorithms, Feature engineering and EDA. 

