---
{"dg-publish":true,"permalink":"/notes/finding-conditional-prabability-intuitively/","tags":["statistics","probability"]}
---

# finding [[Notes/conditional probability\|conditional probability]] intuitively
we first construct a [[Notes/contingency table\|contingency table]] containing the data for our analysis.

| test results/symptoms | _Negative_ | _Positive_ |
| --------------------: | ---------: | ---------: |
|                  _No_ |        860 |         90 |
|                 _Yes_ |         10 |         40 |


finding $P(\text{positive test result given presence of symptoms})$
$P(\text{positive test result given presence of symptoms}) = \large{\frac{P(\text{positive test result})\text{ AND P(presence of symptoms)}}{\text{P(presence of symptoms)}}}$

$P(\text{positive test result) AND P(presence of symptoms)}$ = `contigency_table.iloc[1,1]` = 40
$P(\text{presence of symptoms})$ = `contingency_table.iloc[1,1] + contingency_table.iloc[1,0` = 10 + 40 = 50

Hence:

$P(\text{positive test result given presence of symptoms}) = \large{\frac{40}{50}} = 80.0\%$

##### finding the conditional probability using pandas
```python
test_results = {"Negative": [860, 10], "Positive": [90, 40]}
symptoms = ["No", "Yes"]

import pandas as pd
contingency_table = pd.DataFrame(test_results, index= symptoms)

  
  

# find the probability of getting a positive result, knowing in
# advance the presence of symptoms
# i.e. P(positive test result | presence of symptoms)
# this would equal to :
# P(positive test result AND presence of symptoms) / P(presence of symptoms)

  
  
# P(positive test result AND presence of symptoms) = 40
# P(presence of symptoms) = 

  

# modeling it using python code
P = (contingency_table.iloc[1,1] / \
(contingency_table.iloc[1,1] + contingency_table.iloc[1,0]))
print(f"Conditional probability: {P * 100}%")
```
