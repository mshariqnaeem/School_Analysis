# School_Analysis

## Overview

After completing a quick analysis of the school schools_complete.csv and students_complete.csv files, Maria and her supervisor believe that the file shows evidence of academic dishonesty in the reading and math grades for Thomas High School. Maria has asked us to replace the math and reading scores for Thomas High School 9th grade with Nans while the rest of the data is unchanged. Once this is done she would also like us to repeat the analysis of the module with the updated information.

### Purpose

The purpose of this exercise is to understand how to use Pandas and Jupyter Notebook to manipulate sets of data and how to use different functions within Pandas to re-factor and re-analyze our code to perform analysis on the changed data set 


## Results

### Change Thomas High School Grade 9 marks to show NaNs

During this step we were asked to show NANs. We accomplished this by using the **.loc** method to change the math and reading scores which included both the school name "Thomas High School" and the grade "9th". the code we used is included below along with the end result

student_data_df.loc[(student_data_df["school_name"] == "Thomas High School") & (student_data_df["grade"] == "9th"), "reading_score"] = np.nan

![NANs result](https://user-images.githubusercontent.com/92459399/143796817-87d911a1-18ff-495a-a1d7-bb9895e024ed.PNG)

As you can see the student **Rebecca Tanner** is in grade 9 attending Thomas High School, marks now shows NaN for both Math and reading.


### School Summary without Thomas High School 9th Grade Marks

Now that we have removed the 9th Grade marks for Thomas High School, we proceed to complete the analysis for the schools again to see if there is a significant change in the average mark for the schools.

We recreated the dataframes for the district summary and refactor the code to show the results.
Once the data has been refactored and the dataframe reprinted we came up with the following results.

![old analysis](https://user-images.githubusercontent.com/92459399/143798293-69d96063-de66-427a-b54a-a0ccc2e6ed76.PNG)
![New Analysis](https://user-images.githubusercontent.com/92459399/143798442-2e5c236d-54af-48ba-af03-7796d9b086c1.PNG)

The average for Thomas High school under the adjusted file has changed drastically once we include all the grades excluding the 9th grade scores from 97% to 69% which would indicate to us that there may be significant academic dishonesty in the 9th grade marks for Thomas High School.


## Summary

In conclusion after adjusting the data we learned that there may have been significant academic dishonesty amongst the 9th graders for Thomas High School which boosted the schools overall average.

We also learned how to refactor dataframes after adjusting our data in this exercise and making conclusions from these updated results.
