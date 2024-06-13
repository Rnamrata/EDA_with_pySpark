This is the report of the 'Exploratory Data Analysis using PySpark' assignment. The dataset was collected from The World Bank and the data description was adapted from the same website. Here is the link to the website - https://microdata.worldbank.org/index.php/catalog/2334/data-dictionary/F7?file_name=2012ihses05_education.

Exploratory Data Analysis (EDA):
At first, the necessary libraries were loaded along with installing pySpark and findspark. Then after initializing the Jupyter Notebook and sparksesstion, the dataset was loaded using the sparksesstion.

In this phase, the dataset schema, sample size, feature size, name of the features, and counting missing values regarding the features were checked. A pie chart representing the proportion of missing values by feature has been generated for better understanding.

Feature Engineering:
In this stage, features were selected based on the number of missing values. The features with a higher count of missing values and insignificant information such as, 'idcode', 'Questionnaire Identifier', etc were not selected.

Here is the description of the features: ' strat' - m Strat'um we' - ght Weight (Inverse of the selection probability, adjusted to match qadha-wise n' by recall ' - rnorate q6:' Gove' - te qh'ada q7' - luster cluster': ' - er serial hh hh'h Hou' - Number hsize q27: S'ode r' - nt education q0502 q502: Hav'est c' - ate you attained q0504' like' - The minue your education q0506 q506: Main re' enro' - school / /what grade ar q0508 q508: The 'ng ab' -om syou choothe l some day's dur_1' - school qthe 0515 q0515: 'Do use ' - q0516_1 the q0516_1: Wher'e use i' - ) q0516_2the q0516_2: Wh'ere use' - (2) q0516the _3 q0516_3: 'Where u' - t (3) q051the 6_4 q0516_4:' Where ' - et (4) q05the 17_1 q0517_1': How d' - rnet (1) qthe 0517_2 q0517'_2: How' - ternet (2) q0ing1the I_3 q0517_3:' How do' - net (3) q0518ing1the I q0518_1: Pu'rpose f' - ernet (1) q05ing8the _2 q0518_2: 'Purpo' - se internet (2) q0518_3 q051

Four new features were generated due to a better understanding of purpose. The values were adopted from the website mentioned in the description. These new features are 'governorate_names', 'literacy_status', 'internet_access', and 'education_status' for 'governorate', 'q0504', 'q0515', and 'q0502' accordingly. As 'governorate' had a variety of data, instead of using a function, a new string-type column was generated from the existing one and then replaced with the values.8_3: Purpose for use internet (3) q0519 q0519: Average hours/week of Internet

Data Visualization:
Two types of visualization were done here. One is statistical analysis and the other one is graphical analysis using graphs and charts.

Statistical Analysis:
Numerous statistical analyses such as a summary of the dataset or different features, minimum or maximum value, mean value and standard deviation, and the frequent value of specific features were measured.

A random sampling and a comparison was done. The total unique values and the count of a feature were calculated.

A filter was generated for a single value of the Governorate.

Graphical Analysis:
Five different types of graphical analyses were performed here to represent data. These include pie charts, histograms, line charts, bar charts, and box plots.