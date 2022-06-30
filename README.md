# School_District_Analysis
Analysis utilizing Jupyter Notebook and Pandas library as installed from Anaconda Distribution package extension for Python version 3.7.

## Project Overview
The task is to aid Maria, the Chief Data Scientist for a city school district to prepare a number of visuals to summarize performance of students at the 15 constituent high schools on standardized tests. Featuring work with DataFrames, one of two primary data structures in Pandas<sup>i</sup> -- the other being Series (arrays are a third perhaps less-prominent structure) -- the analysis brings opportunity to augment yet again the learning data analyst toolkit, this time as CSV files are brought in to Jupyter Notebook for performing mathematical calculations and statistical summarizations and other trend-revealing functions.  The goal: to present a snapshot of school performance so that school and district level <sup>ii</sup> decision-makers may make informed strategic plans. To be produced are the following tables:

	A.  a district-level school metrics summary
	B.  a school-level overview of key metrics
	C.  a summary depicting:
		1.  Top 5 and bottom 5 performing schools based on overall passing rate
		2.  Average scores for math and reading for students at each grade level in each school
		3.  School performance based on budget per student
		4.  School performance based on school size
		5.  School performance based on school type

<sup>i</sup> see website link: https://pandas.pydata.org/pandas-docs/stable/reference/      
<sup>ii</sup> video: Module 4.0.4

### Challenge Overview
Further challenge presents as the school board notifies Maria and her supervisor that one of the data files,
>	the `students_complete.csv` file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered.

As a result, Maria asks for the A-B-C analysis listed above to be repeated, with this report to discuss how changes affected the overalll analysis.

### Challenge Deliverables

#### Images
These are labelled below as "Image D<#>," where <#> represents one of the numbered deliverables.

**Image D1:** Replace reading and math scores for ninth graders in Thomas High School with `NaN`s
![Image D1](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29_code-and-output_replace-ths-9th-scores.png?raw=true)

**Image D2-A:** District summary![Image D2-A](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29_district_summmary_df_post-recode.png)

**Image D2-B:** Overview of Key Metrics ![Image D2-B](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29_ths-metrics_post-recode.png)

**Image D2-C1:** Top 5 and bottom 5 performing schools based on overall passing rate ![Image D2-C1](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29_Top5-and-Bottom5_post-recode.png)

**Image D2-C2:** Average scores for (a) math and (b) reading for students at each grade level in each school ![Image D2-C2(a)](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29_by_school_average_math_scores_by_grade_post-recode.png)
![Image D2-C2(b)](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29_by_school_average_reading_scores_by_grade_post-recode.png)


**Image D2-C3:** School performance based on budget per student ![Image D2-C3](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29_school_capita_spending_summary_df_post-recode.png)

**Image D2-C4:** School performance based on school size (and with THS group in blue)
![Image D2-C4](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29_school_size_summary_df_post-recode.png)
![Image D2-C4](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29_school_size_summary_df_ths-group-in-blue_post-recode.png)

**Image D2-C5:** School performance based on school type ![Image D2-C5](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29_by_type_summary_df_ths-group-in-blue_post-recode.png)


#### Results Analysis

Though most metrics for other schools and grades remain unchanged by the re-analysis precipitated by evidence of academic dishonesty for the ninth grade reading and math scores for THS, some changes are to be noted, some with greater variation than others as far as percentage change in before and after value.  In particular, checking these tables reveals a value(s) from before the re-analysis that changes afterwards:

 [x] District-level school metrics summary
	
	Both the math and reading scores and all the passing percentages change by either tenths
	or hundredths of their respective values.(see image a below)

 image a: ![image a](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29__DistrictSummary__before-on-left-after-on-right.png)

 [x] School-level overview of key metrics

	For THS, both the math and reading scores and all the passing percentages change by either tenths
	or hundredths of their respective values.(see image b below)

 image b: ![image b](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29__SchoolLevelSummary__before-on-top-after-on-bottom.png)

 [x] Top 5 performing schools based on overall passing rate
 
	As THS is the second on the top-5 list, the math and reading scores and all the percentages change
	correspondingly for the before and after pics. (see image c below)

 image c: ![image c](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29__Top5-on-top_Bottom5-on-bottom__before-on-left-after-on-right.png)

 [ ]  Bottom 5 performing schools based on overall passing rate

	*No change (image c above)*

 [x] Average scores for math and reading for students at each grade level in each school

	The THS ninth grade scores become "NaN." (see image d below)

 image d: ![image d](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29__AverageScoresBySchoolByGrade_math-on-top_reading-on-bottom__before-on-left-after-on-right.png)

 [ ] School performance based on budget per student

	*No change (image e below)*

 image e: ![image e](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29__school-per-capita_spending_summary__before-on-left-after-on-right.png)

 [x] School performance based on school size

	Differences in before and after by at most hundredths of a value in the category of THS {Medium (1000-1999)}
	(see image f below)

 image f: ![image f](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-29__school-size_summary__before-on-left-after-on-right.png)
	
 [ ] School performance based on school type

	*Unchanged within value rounding for all values. (see image g below)

 image g: ![image g](https://github.com/shanl5/School_District_Analysis/blob/main/Resources/images/Screenshot_2022-06-30__school-type_summary__before-on-left-after-on-right.png)

As for the amount that the value changes, the THS percentage values (passing math, passing reading and overall passing) might be expected to be (and are shown to be<sup>iv</sup>) the most affected, since the number of students (all of the 9th grade reading and math scores) will be the highest percentage in relation to overall THS student population (461 of all of the 1635 scores for the school will be "NaN" and thus inadmissable for scoring -- find this by performing a `.isnull().sum()` chained function on the series resulting from replacing the 9th grade THS filtered students_complete.csv read into a DataFrame<sup>iii</sup>) at the school itself, whereas to affect the *average* scores the scores themselves would likely have needed to have been comprised of highly rare outliers for their removal (and by complementary logic? their addition) to have much affect one way or the other on the average of the rest of the scores (math or reading), i.e. the THS 10th-12th grade scores. Still, the affect overall remains within rounding of **tenths***of a single* (either individual unit, or individual percentage) value, whereas the values themselves are several TENS of (single) values, so it appears that the method via which the values are obtained and the subsequent analysis are largelyunaffected, leaving the overall analysis intact and obtained results robust. 

<sup>iii</sup> refer to the commented code in Step 4. (cell-run input line 5) of Image D1 above (images in Deliverables section).
~~image iii: ![image iii](https://github.com/shanl5/School_District_Analysis/Resources/images/Screenshot_2022-06-29_code-and-output_replace-ths-9th-scores.png)~~

<sup>iv</sup> the three cells (coding steps 12 - 14; input run lines 70-72) with `print()` statements in this image show the initial (prior to re-set of THS 9th grade score) value that is being replaced ONLY on the *initial run* of code in the cell, subsequently the value will have already been written into
~~image iv: ![image iv](https://github.com/shanl5/School_District_Analysis/Resources/images/Screenshot_2022-06-29_Top5-and-Bottom5_post-recode.png)]~~


## Summary
The Pandas library for Python (here a data environment was set up for version 3.7) provides much flexibility to work with and analyze many types of related data sets -- including those read from the ubiquitous CSV text file -- in an efficient and timely fashion, especially after practice engenders proficiency working with the syntax of accessing the structures. And like was mentioned in our most recent class ~~to~~yesterday, new functionality built utilizing earlier (already) created structures and modules is a continually renewing process that only ever adds more richness to the world of programming and data analytics and science both figuratively and literally at our fingertips.


## Resources
- Data Source: schools_complete.csv, students_complete.csv
- Software: Python 3.7.9, Jupyter Notebook, PythonData environment
- Coding template framework: PyCitySchools_Challenge_starter_code.ipynb

**Notes**:
- One coding issue that was solved with input from TA J Caro:
  "FutureWarning" error message on run of `replace()` method in Python code (see two images below) -- solved by method argument setting "regex=True."

<img src="/Resources/images/Screenshot_2022-06-29_FutureWarning_pre-code-mod.png" width="40%">

<img src="/Resources/images/Screenshot_2022-06-29_FutureWarning_code-mod-and-rerun_no-msg.png" width="40%">

- In the images (*all* above), the DataFrame table rows applicable to the THS school or 9th grade student grouping are selected and thus marked with a pale blue highlighter-like background as applicable.

