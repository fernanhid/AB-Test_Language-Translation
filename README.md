# A-B-Test-Website-Language-Translation


<b>Data: </b><br>
A company that had previously deployed their website with the same translation to all Spanish speaking countries has decided to offer each country custom translations. 


<b>Objective: </b><br>
Analyze the results of the A/B test and see whether the results are statistically significant. 


<b>Insights: </b><br>
The results pointed to the single translation as doing better then the custom translations, which seemed unlikely.<br> To double check it did two things:
1. I ran <u>T-tests</u> on features to see if the results where statistically significant
2. I automated the process by building a <u>decision tree</u> and seeing if any feature was statistically significant. The dependent variable was whether it was in the test sample or control sample and ideally, no feature should be predictive if the samples are indeed random. However, in this test sample two features came out as predictive which points to the test sample being biased. 

<b>Conclusion: </b><br>
<u>A. If the Results Seem Unbelievable, They Probably Are</u> <br>
We intuitively know that a custom website for each region would yield better results.
So when it didn't it's important to take extra precautions to make sure that the test was run appropriately,
in this case we found that the test sample wasn't indicative of the population<br>
<u>B. We can Automate This Process Using Machine Learning</u> <br>
By building a model that can show us if any features can predict whether a user is in the test or control sample, we can automate the process. We can set a threshold for feature significance and let the model tell us automatically if the sample is biased or not! This gives us more time to deal with deeper subjects.<br>
<u>C. By simply looking at feature distributions, we miss the subtly of sample bias</u> <br>
When we saw the distribution of features, all the features seemed balanced. There were a little discrepancies in country but aged seemed balanced. If we had not run T-test or the decision tree to prove statistical significance then we would of missed age as the major indicator of a biased data set. When running an A/B test, the quality of the test is just important if not more important than the results. 