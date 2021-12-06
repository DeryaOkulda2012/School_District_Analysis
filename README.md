# School_District_Analysis

## Overview of the school district analysis: Explain the purpose of this analysis.

Data from fifteen (15) schools with a total of more than 39,000 students and with a total budget of $24 MUSD, is analyzed to see various effects of funding on educational outcome. Parameters include school size, and whether the school is a district school or a charter school. Result from math and reading test are used for this analysis.

Due to suspicions regarding 9th grade data at Thomas High School, that data is removed from overall analysis.

## Results: Using bulleted lists and images of DataFrames as support, address the following questions.

* How is the district summary affected? 
* How is the school summary affected?
* How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

How does replacing the ninth-grade scores affect the following:
* Math and reading scores by grade
* Scores by school spending - surprisingly, schools with a lower per student budget seem to have better performing students than the schools which spend much higher per student, with the worst performing schools being the ones spending the most per student (spending_summary_df.png). Clearly, more money spent does not necessarily improve education. Other factors must be analyzed to understand this result.
* Scores by school size - the largest schools (of more than 2000 students) have significantly lower test scores, for both math and reading. Schools of up to 1000 students and between 1000 to 2000 students both seem to have higher test scores. (size_summary_df.png)
* Scores by school type - charter schools seem to have a much better outcome for math and reading test results over district schools as there seem to be a significant difference in those test results (see type_summary_df.png)

## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

The 9th grade scores at Thomas High School (both math and reading) definitely skew the results when running the analysis by including and then not including their 9th grade data (per_school_summary_df.dns and per_school_summary_df_NO_THS_9th.dns).

When looking at all other schools, both math and reading scores at each school does not change when we go from 9th grade, to 10th grade, to 11th grade, then 12 grade. Yet, when we including 9th grade scores at Thomas then reanalyze by removing them, there is a significant difference between grade scores within Thomas High School.

