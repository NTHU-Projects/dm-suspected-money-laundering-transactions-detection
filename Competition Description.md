## Competition description
##### Do you say suspicious or not? －Prediction of suspected money laundering transactions?

For the financial industry, money laundering prevention is an inevitable problem and challenge. Criminals use various money laundering channels to bleach illegal funds to evade investigation and prosecution by judicial authorities, and even reuse the proceeds of crime for other illegal activities. If financial institutions do not actively review all kinds of transactions handled by them, they will become a bleaching channel for criminal groups. In addition to damaging their own goodwill, financial institutions have the characteristics of collecting funds from the masses, which will disrupt the financial market. order. In addition, financial criminals continue to use emerging technologies or channels to disguise or conceal their ill-gotten gains, and money laundering takes on new forms. As a result, it is clear that the financial industry alone is not enough to identify suspicious criminal activities.

Yushan Bank attaches great importance to the maintenance of corporate social responsibility and financial order, and is also committed to introducing artificial intelligence technology and applying it to the identification service of suspicious transaction activities. On each business day, Yushan Bank screened out suspected money laundering transactions that should be reported to the Investigation Bureau of the Ministry of Justice according to various predefined suspicious activity patterns, and manually reviewed each transaction and wrote an investigation report. However, this not only consumes a lot of manpower and man-hours, but also has the possibility of omissions, and the existing cumulative number of cases that meet the declaration is also one of the key factors affecting the effectiveness of model training.

Therefore, this Yushan Artificial Intelligence Open Challenge was conceived on the topic of this business pain point, and invited experts from all walks of life to solve the bottleneck of the current practice. Yushan Bank will provide information such as de-identified customer account transactions and final suspicious transaction reporting (SAR) results, allowing participants to design their own algorithms to build models to more accurately screen out suspicious transactions that should be reported and reduce suspicious transactions. The false positive rate of the activity. It is hoped that with the application of artificial intelligence technology, manpower will be reserved for more complex and difficult case review operations, and to contribute to an orderly and healthy financial environment in Taiwan!

Yushan Bank is now sending out hero posts! The total prize is 230,000, waiting for you to challenge!

### The competition will proceed as follows:

- Teams must register for the competition on the T-Brain platform before the registration period.
- Teams must join the Yushan Artificial Intelligence Challenge Slack Workspace community to get first-hand information about the competition ( please refer to the Dataset Download section: Slack Workspace link ).
- The participating teams will download the training data set from the Dataset Download area of ​​the T-Brain platform during the competition schedule. The organizer will provide the de-identified customer account transactions and the results of the final suspicious transaction declaration (SAR) report (please refer to Dataset Download area: training data set, training data field description ).
Start model training!
- Teams should upload the model prediction results to the Leaderboard system in accordance with the specified file content format (please refer to the Dataset Download area: list of cases to be predicted and sample files to be submitted ) to the Leaderboard system, and the Leaderboard will evaluate each submission result.
- After submitting the prediction results, the participating teams will get the scores of the Public Leaderboard evaluation as a reference. Three days before the end of the competition (2022/12/23) at 11:00 am, the organizer will announce the Public Leaderboard's prediction solution and the correlation of the next month in the Dataset Download area. The data will be used by the participants to modify the model, and the data will be used before 3:00 pm on the day when the competition ends (2022/12/26).Last uploaded forecastAs the result of the Private Leaderboard, the organizer will announce the result separately, and use this result for the final ranking. The final ranking will be announced on the T-Brain platform on 2023/01/06.

### Contest details are described on the following pages:
#### Forecast description
- Predict the probability of filing a Suspicious Transaction Activity Report (SAR) for each case in the next month.
- The cases to be predicted are all the case lists in the "Dataset Download area: List of cases to be predicted and examples of submitted files".
- The prediction result only contains floating point numbers between 0 and 1, and does not include other prediction results. If it is not between 0 and 1, it is regarded as a prediction error.

#### Registration Specifications
- The number of participating teams is 1 to 8 people.
- Students (above colleges and universities, including master and doctoral students) or people in the industry can sign up to participate (except current colleagues in Yushan and current employees of Trend Micro).
- Each member must complete a mobile phone verification upon registration.
- After the registration deadline, no new team registration or registration to join an existing team is allowed.
- During the competition, teams are not allowed to split.
- Contestants are only allowed to join one team (the organizer will check from time to time whether the contestants have illegally joined multiple teams).

#### Eligibility and method of receiving awards
1. At least half of the team members (inclusive) must have the nationality of the Republic of China or have a work visa of the Republic of China, and the team is eligible to receive the award.
2. In addition to submitting the prediction results, the winning team must provide the organizer's implementation program and related documentation for review by the organizer to determine the ranking after the competition, and agree that at least one member of the team will attend the award ceremony and exchange and sharing session for modeling Techniques and experience briefings, and accept on-site questions, otherwise all team members will lose their eligibility to receive the award, and the award will not be available.
3. If the winning team has any missing or incomplete content in the application documents, implementation programs or related explanatory documents, and the documents are not supplemented within 7 days from the next day after the notification of the supplementary documents, all team members will be disqualified to receive the prize.
4. Participants who join multiple teams at the same time will not be eligible or disqualified to receive the prize.
5. The prize money will be paid by remittance in New Taiwan Dollars, and the payment object is limited to the teams that meet the registration criteria and are eligible to receive the prize. The winning team should appoint a representative with a local NTD account in Taiwan to receive the prize, and use the team member as the Taiwan tax filer.
6. The results of the participating teams' models on the Private Leaderboard must be better than the scores in the "List of Cases to be Predicted and Examples of Submitted Files" in the Dataset Download area in order to be eligible for the award.

#### Grading
1. The content of the submitted file must include the reported SAR probability of all cases to be predicted, in descending order of probability, and the format must comply with the regulations (please refer to the Dataset Download area: list of cases to be predicted and sample submission files ).
2. The Leaderboard system will evaluate each submission result.
3. The prediction results provided by the participating teams will be automatically divided into Public and Private by the organizer. The scoring results of the Public Leaderboard in this competition are calculated based on the predicted SAR probability of cases reported in the t month; The result calculated from the SAR probability value of cases reported in t+1 month.
4. During the competition, after submitting the prediction results, the participating teams can use the scores evaluated by the Public Leaderboard as a reference. At 11:00 a.m. 3 days before the end of the competition (2022/12/23), the organizer will announce the Public Leaderboard's positive prediction solution and relevant data for the next month in the Dataset Download area for participants to revise the model. At 3:00 pm on the day of the end of the competition (2022/12/26), the participating teams will be **Last uploaded forecast**
##### As the result of the Private Leaderboard, the organizer will announce the result separately, and use this result for the final ranking.

#### Scoring
This competition will be graded with the Precision of Recall@N-1, which means that the precision under the list of N-1 real SAR cases is caught (rounded to 7 decimal places), the formula is as follows:
(see in the evaluation folder)

#### Competition Rules
1. Test results can only be submitted up to 3 times a day.
2. Be sure to use Machine Learning to make predictions, no human labeling is allowed.
3. The use of non-open source AutoML-related automatic modeling services is prohibited.
4. Programs and eigenvalues ​​cannot be shared privately, but can be discussed publicly in the official communication community forum.
5. The data set is only used for this competition. Participants shall not leak or deliver the data set to non-participants for their own benefit or others; and the data set shall be permanently deleted after the competition, and shall not be stored or retained in any form. If there is any violation, the entrant shall compensate the organizer for all losses (including but not limited to attorney fees) and punitive liquidated damages equivalent to three times the compensation amount.
6. If a data set not provided by the organizer is used, the data set must be additionally provided to the organizer after the competition.
7. If necessary, the organizer reserves the right to adjust the dataset during the competition.
8. Under the following circumstances, the organizer may directly disqualify the entrant or receive the award without notifying the entrant:
- There has been specific evidence that the team belongs to any plagiarism and cheating.
- There has been concrete evidence that the team they belonged to has attacked the Leaderboard system.
- There has been specific evidence that the team to which it belongs affects other participating teams, resulting in unfair situations.
- There has been specific evidence that the team it belongs to has violated the rules of this competition or the terms of use of the contestants of the "T-Brain AI Real Battle Bar Platform Service".
9. Contestants use Slack for this event to abide by the following regulations. If the following regulations are violated, the organizer may cancel the right to use Slack or disqualify them from participating without notifying the participants:
- Don't leak other people's sensitive information on the event Slack.
- Do not post words that affect the perception of others, such as coercive, indecent, obscene or provocative.
- Do not post inappropriate content that is not related to this contest, illegal or commercial.
- Others whose speech or behavior is determined by the organizer to be inconsistent with the purpose of this competition or affect the rights and interests of others.
10. The organizer reserves the right to the final interpretation and ruling of the competition rules.
11. The organizer (hereinafter referred to as the authorized person is Yushan Bank) will take photos and videos during the awards ceremony and sharing sessions and other activities, and use the relevant videos or photos in the scope including but not limited to press releases and publicity. The entrant (hereinafter referred to as the licensor) hereby declares and agrees that:
- Read and understand the following matters within a reasonable period before registering for the competition.
- The authorized person may take photos and videos of the authorized person during the event.
- During the event, the authorized person may permanently use, publicly display or edit, delete or make other necessary modifications to the content of the authorized person's photography and video recording (including the authorized person's portrait).
- The copyright of the author's photographed and videotaped works (including the author's portrait) during the activity period shall be originally obtained by the author, who is the author and enjoys complete copyright personality rights and copyright property rights. .
- The authorizer has been informed by the authorized person of "(Yushan Bank's statutory notice on collection, processing and use of personal data)", and has clearly understood the content of the above statement and notice, and hereby agrees to the specific purpose of personal data collection, collection Item (category), period of use, area, object and method, should be disclosed completely and accurately, as well as relevant requirements for access, request for copy, correction of data, request to stop processing, use or delete, and notify family members, etc., and agree to the authorized person Collect, process and use my personal data within the scope necessary for the specific purpose of the company.
12. During this event, contestants are not allowed to use any indecent words, words, or remarks and behaviors that damage the reputation or goodwill of others. If the organizer determines that their behavior is not in line with the purpose of this competition or affects the rights and interests of others, the organizer has The right to disqualify from the competition.
