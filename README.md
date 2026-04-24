# Data_Analytics_Car_loan_defaulters.

## Goal
* Required to determined and examine factors that affects the ratio of vehicle loan defaulters. Also use the findings to create a model to predict the potential defaulters.
### Project background
* Financial institution incur significant lossses due to the default of vehicle loadns. THs has led to the tightening of vehicle loan underwriting and an increases in vehicle loan rejection rates. The need for a better credit risk scoring model is also raised by the institution. The institution wants us to estimate and determine of vehicle loan defaulter.

### Data Set
 * Banking Dataset
### Programing Laungage
  * Python
### Library
  * Google.colab
  * Pandas
  * Numpy

### Task Performed
* Importing the required libraries to read the excel file in google colab
  <img width="640" height="356" alt="Capture1" src="https://github.com/user-attachments/assets/e1573d33-1409-4972-be4c-bc9aa3c183d9" />

* Perform preliminary data inspection and report the findings like the structure of the data, missing values, duplicates.
<img width="1786" height="575" alt="Capture2" src="https://github.com/user-attachments/assets/f773bec8-e104-4130-9571-e6cfbdb7c6ba" />
<img width="609" height="800" alt="Capture3" src="https://github.com/user-attachments/assets/effcfc01-18ce-43e8-9d3b-16d7baee0838" />

* Variable names in the data set may not be in accordance with the identifier naming in Python. Change the variable names accordingly.
<img width="1787" height="392" alt="Capture4" src="https://github.com/user-attachments/assets/c284948d-e815-4a2c-947b-8b5c6e9141c7" />

* The presented data set might contain missing values, therefore, Use strategies to fill in the missing values. Devise strategies while exploring the data.
<img width="772" height="795" alt="Capture5" src="https://github.com/user-attachments/assets/e5845f18-15fe-42fa-bfaf-92bf1e292b3f" />


* Provide the statistical description of the quantitative data variables
<img width="1751" height="450" alt="Capture6" src="https://github.com/user-attachments/assets/f2931882-164d-45b8-a3c0-c4f9db22dcfb" />

* How is the target variable distributed overall?
<img width="768" height="766" alt="Capture7" src="https://github.com/user-attachments/assets/188faffc-03db-4cbb-b144-918ec29d7205" />

* The chart shows a highly imbalanced distribution of loan defaults:
     Class 0 (no default): ~180,000 cases
     Class 1 (default): ~50,000 cases
  
 * So roughly:
      ~78% non-default
     ~22% default

* In plain terms, most borrowers did not default, and defaults are a minority class.

* Study the distribution of the target variable(loan defaulter) across the various categories like branch, city, state, branch, supplier, manufacturer, etc.
<img width="585" height="291" alt="Capture8" src="https://github.com/user-attachments/assets/cd5f2854-e598-44ff-b3b1-92ffb6f65ba6" /> <img width="823" height="446" alt="Capture9" src="https://github.com/user-attachments/assets/3353f4ff-5ed9-4bfa-a195-809323624087" />
<img width="815" height="450" alt="Capture11" src="https://github.com/user-attachments/assets/d2806d48-5713-4443-be90-42a23552243a" />
<img width="813" height="466" alt="Capture10" src="https://github.com/user-attachments/assets/02edf269-b3e0-4e18-86e0-11f64e0ce8bd" />

* What are the different employment types given in the data? Can a strategy be developed to fill in the missing values (if any)? Use pie charts to express how different types of employment defines defaulter and non-defaulters.
<img width="631" height="531" alt="Capture12" src="https://github.com/user-attachments/assets/569de8c2-b8c0-43aa-8449-889c23b313e3" />
<img width="902" height="485" alt="Capture13" src="https://github.com/user-attachments/assets/3ad66a65-f2b8-4fca-a609-86f38c5b1811" />

* Has age got something to do with defaulting? What is the distribution of age with respect to defaulters and non-defaulters?
<img width="607" height="443" alt="Capture14" src="https://github.com/user-attachments/assets/c209a959-1350-49b8-9e3d-7a5580c23731" />
<img width="917" height="760" alt="Capture15" src="https://github.com/user-attachments/assets/26c0fbba-f3d8-4d46-9665-475e50bb6ca8" />
* findings from the chart, Both groups are concentrated roughly between 25 and 60 years. The peak for both is around the early to mid 30.
Boxplot tells a clearer story than the histogram: age is not a strong differentiator of default behavior in your dataset.
    ### Key observations
* Median age
Non-defaulters: ~41
Defaulters: ~39
Defaulters are slightly younger, but the difference is small.
Both groups have very similar interquartile ranges (~low 30s to high 40s)
Heavy overlap between the two groups
Range & outliers
Both extend roughly from mid-20s to ~70+
A few high-age outliers in both classes, No meaningful separation at extremes either

* What type of ID is presented by most of the customers as proofs?
<img width="586" height="376" alt="Capture16" src="https://github.com/user-attachments/assets/fce1e261-5f83-4932-b4bd-4a8fe9f06dd1" />
<img width="934" height="640" alt="Capture17" src="https://github.com/user-attachments/assets/2c851304-bff4-45a7-8755-7d0231bf3dbb" />

