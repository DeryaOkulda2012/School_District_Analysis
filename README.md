# School_District_Analysis

## Overview of the school district analysis: Explain the purpose of this analysis.

Data from fifteen (15) schools with a total of more than 39,000 students and with a total budget of $24 MUSD, is analyzed to see various effects of funding on educational outcome. Parameters include school size, and whether the school is a district school or a charter school. Result from math and reading test are used for this analysis.

Due to suspicions regarding 9th grade data at Thomas High School, that data is removed from overall analysis.

## Results: Using bulleted lists and images of DataFrames as support, address the following questions.

* How is the district summary affected?  There is very little change
* How is the school summary affected?   There is very little change with or without 9th grade data.
* How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools? Removing the suspicious 9th grade data from Thomas High school does not change the results much as that grade represents around 2 percent of the entire school/student dataset.

How does replacing the ninth-grade scores affect the following:
* Math and reading scores by grade - When looking at each school on its own, both math and reading scores at each school changes very little when going from 9th grade, to 10th, to 11th, then to 12 grade. There is very little change in removing the 9th grade scores at Thomas from the entire set as that subset is around 2 percent of the entire dataset.
* Scores by school spending - surprisingly, schools with a lower per student budget seem to have better performing students than the schools which spend much higher per student, with the worst performing schools being the ones spending the most per student (spending_summary_df.png). Clearly, more money spent does not necessarily improve education. Other factors must be analyzed to understand this result. Again, there is very little change in removing the 9th grade scores at Thomas.
* Scores by school size - the largest schools (of more than 2000 students) have significantly lower test scores, for both math and reading. Schools of up to 1000 students and between 1000 to 2000 students both seem to have higher test scores (size_summary_df.png). Again, there is very little change in removing the 9th grade scores at Thomas.
* Scores by school type - charter schools seem to have a much better outcome for math and reading test results over district schools as there seem to be a significant difference in those test results (see type_summary_df.png).  Again, there is very little change in removing the 9th grade scores at Thomas High School.

## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

The 9th grade scores at Thomas High School (both math and reading) does not skew the results when running the analysis by including and then not including their 9th grade data (per_school_summary_df.dns and per_school_summary_df_NO_THS_9th.dns). The size, discrict type, spending amount, and overall percent for math and reading does not change the results by much.
