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
  * Matplotlib.pyplot
  * Seaborn
  * Datetime
  * Stats

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

 * Study the credit bureau score distribution. How is the distribution for defaulters vs. non-defaulters? 
<img width="766" height="470" alt="Capture18" src="https://github.com/user-attachments/assets/0dc6daf8-ed0e-4897-84be-46f6fc8a1ffa" />
<img width="890" height="481" alt="Capture19" src="https://github.com/user-attachments/assets/ec373ec3-57d0-4837-bb1c-0078e97e5b42" />

* Explore the primary and secondary account details. Is the information in some way related to the loan default probability?
<img width="639" height="571" alt="Capture20" src="https://github.com/user-attachments/assets/00787e0f-1c4d-4e85-a581-a7e1309a59a1" />
<img width="847" height="545" alt="Capture21" src="https://github.com/user-attachments/assets/81a42cb9-54e6-4bdb-9488-e6f87b94efe2" />
<img width="817" height="536" alt="Capture22" src="https://github.com/user-attachments/assets/724ae613-dca2-423d-92b1-558d5f6eef62" />
<img width="846" height="543" alt="Capture23" src="https://github.com/user-attachments/assets/6c2acb4f-df47-450d-8fd6-660d178f076a" />
<img width="845" height="556" alt="Capture24" src="https://github.com/user-attachments/assets/74a110f6-43c3-4d86-840f-859b30bb24c5" />
<img width="847" height="542" alt="Capture25" src="https://github.com/user-attachments/assets/c59c4591-a517-48fc-924d-1c1810e9b844" />
<img width="853" height="541" alt="Capture26" src="https://github.com/user-attachments/assets/8ff15dcb-3bc8-4d24-b85c-6ee59db47579" />
<img width="844" height="536" alt="Capture27" src="https://github.com/user-attachments/assets/766f4e64-8f2f-497d-bbbf-5e94a28fafa3" />
<img width="839" height="555" alt="Capture28" src="https://github.com/user-attachments/assets/d9eefa7d-f380-4bf4-8575-9b40b74b3491" />
<img width="832" height="549" alt="Capture29" src="https://github.com/user-attachments/assets/9f7234ae-a1f1-4a7e-9d9d-b8de1a4d0c9c" />
<img width="841" height="530" alt="Capture30" src="https://github.com/user-attachments/assets/298a83a5-ccba-429a-8288-cc2c2f62df19" />
<img width="845" height="544" alt="Capture31" src="https://github.com/user-attachments/assets/7b682e71-189b-40a6-9465-90275e83f1e3" />
<img width="843" height="552" alt="Capture32" src="https://github.com/user-attachments/assets/ed51b561-f98b-417a-bf05-e8bba4d39150" />
<img width="649" height="652" alt="Capture33" src="https://github.com/user-attachments/assets/56ed62da-2486-4f49-9b53-82778859d327" />
<img width="721" height="555" alt="Capture35" src="https://github.com/user-attachments/assets/c672ba0b-8149-4582-ac93-601ab302041a" />

* Is there a difference between the sanctioned and disbursed amount of primary and secondary loans? Study the difference by providing appropriate statistics and graphs.
<img width="725" height="818" alt="Capture36" src="https://github.com/user-attachments/assets/be36676a-e9ae-4812-b165-63f497fd701f" />
<img width="573" height="708" alt="Capture37" src="https://github.com/user-attachments/assets/43f813d5-2c82-48e3-ab8e-343d5eef249a" />
<img width="578" height="789" alt="Capture38" src="https://github.com/user-attachments/assets/140b4687-dadd-422e-a161-d274ccd16174" />
<img width="559" height="716" alt="Capture39" src="https://github.com/user-attachments/assets/fb7d0f4f-8936-4edf-9594-4990f2794096" />
<img width="589" height="390" alt="Capture40" src="https://github.com/user-attachments/assets/7900e1c6-6084-4668-b565-efa9a1be6769" />

* Do customers who make higher numbers of inquiries end up being higher risk candidates?
<img width="530" height="624" alt="Capture41" src="https://github.com/user-attachments/assets/f5ca64f5-6cf3-4463-bbd9-da3ec7137880" />
<img width="674" height="536" alt="Capture43" src="https://github.com/user-attachments/assets/ce6b762f-c4da-4995-bf75-c6448c85a9b2" />
<img width="570" height="840" alt="Capture42" src="https://github.com/user-attachments/assets/0af3b418-d5b0-485a-ba56-5a5d770a8863" />

* Is credit history, that is, new loans in the last six months, loans defaulted in the last six months, time since the first loan, etc., a significant factor in estimating the probability of loan defaulters?
  <img width="674" height="536" alt="Capture43" src="https://github.com/user-attachments/assets/1aa39ddb-0260-4cda-9c19-5bd330b482e9" />
  <img width="634" height="773" alt="Capture44" src="https://github.com/user-attachments/assets/472105e7-69a2-49a4-8585-9ab7d7e15665" />
  <img width="432" height="833" alt="Capture45" src="https://github.com/user-attachments/assets/7d78e8df-2908-4686-a157-a3a2c3a5ee69" />
  <img width="576" height="1005" alt="Capture46" src="https://github.com/user-attachments/assets/cd8f0306-ce60-4794-85b2-310eff6bfe32" />
  <img width="503" height="804" alt="Capture47" src="https://github.com/user-attachments/assets/2e4866c6-8bc9-4466-b04d-d13f6a1b9232" />
  <img width="506" height="791" alt="Capture48" src="https://github.com/user-attachments/assets/84353a2a-7412-487a-9127-cb68f0e69d7b" />

* Perform logistic regression modeling, predict the outcome for the test data, and validate the results using the confusion matrix.
<img width="676" height="821" alt="Capture49" src="https://github.com/user-attachments/assets/2d983e09-a771-4b32-b7bb-a6beeeb1a38c" />
<img width="388" height="318" alt="Capture50" src="https://github.com/user-attachments/assets/9fe482e5-6cf3-47bb-97ac-86040363e492" />

### Conclusion
* Confusion Matrix Insight
   * True Negatives (TN): 36,646 → correctly predicted non-defaulters
   * False Positives (FP): 87 → flagged as defaulters but actually safe
   * False Negatives (FN): 9,845 → missed defaulters
   * True Positives (TP): 53 → correctly predicted defaulters
* Who Will NOT Default (Class 0)
    * Total: 36,733
    * Correctly predicted: 36,646
* Who WILL Default (Class 1)
    * Total: 9,898
    * Correctly predicted: 53
    * Missed: 9,845
* Summary
     * The model is extremely good at identifying safe customers. Almost every non-defaulter is correctly classified.
     * The model fails to detect defaulters. It identifies only 1 out of every 100 actual defaulters.




