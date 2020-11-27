# Data_Compliance_Perception

As a group project during the 2nd year of my Master's in Data Science at Ecole Polytechnique and HEC Paris, we analysed how customers perceive Data Policies of companies, and tried to identify bias in customer trust towards data protection.

### Focus

Our analysis attemps to answer the following questions:

1. _What terms/expressions in a data policy makes it perceived as compliant / non compliant by the customers?_
2. _Is customer perception of compliance correct compared to expert ratings?_
3. _What factors best explain customer trust towards a company's data policy?_
4. _What bias can we identify in customer trust?_


### Data

The data we had access to includes:

* __Customer ratings__ of 115 Data Policies (17 questions per questionnaire, over 4 criteria: __Transparency__ of policy, user __Control__ of data, user perceived __Benefits__, and overall user __Trust__).
* __Expert ratings__ of Privacy Policies, over 10 GDPR compliancy criteria.
* __Full content__ (text) of the Data Policies, with __paragraphs annotated__ w.r.t. the GDPR compliancy criterion they cover.


### Methods and conclusions

1. We used __NLP__ (regression using Bag-of-Words tokens) to __identify the groups of words that impact customer Transparency and Control grades the most__. For example, it appears that expressions related to third-party data sharing tend to bring grades down (more in the presentation slides).

2. We computed **correlation** between Transparency & Control grades by users and GDPR Compliance grades by experts. It appears that non-experts are biased in the way they rate Data Policies - this could be due to both lack of legal knowledge and to **latent variables** that drive user perceptions, such as perceived Benefits from the company, and prior beliefs about the company.

3. / 4. We further explored what drives user Trust with __linear regressions__. Perceived Transparency and Control, in addition to being weakly correlated vs. expert views, aren’t enough to explain the Trust we put into Data Policies. Especially, perceived user __Benefits__ weigh in, and twist our perception… Could we even lower our privacy standards if we deem benefits worth enough??


### Next steps

A potential next step would be to dive with more granularity into what types of customer benefits drive trust towards Data Policies - and therefore could have users arbitrage between these benefits and privacy.
