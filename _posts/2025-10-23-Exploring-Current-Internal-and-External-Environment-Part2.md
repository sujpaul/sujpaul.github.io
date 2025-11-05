---
title: "Exploring Current Business Internal and External Environment (Part 2)"
date: 2025-11-03
categories: [AI, Strategy, ML, DL]
tags: [strategy, AI, DL,ROI, Payback Period, Productivity]
read_time: true          # ✅ Shows estimated reading time (e.g., "7 min read")
toc: true                # ✅ Enables Table of Contents
toc_sticky: true         # ✅ Keeps TOC visible as you scroll (nice for long posts)
---


In the previous blog Exploring Current Business Internal and External Environment (Part 1), I discussed about the external factors to consider in developing the strategy.  In this blog, I will discuss the internal factors.

## Lights on {#Lights on}

Now that you have an understanding at a high level, the next thing that I do is to understand how work gets done.  This opens up a smorgasbord of information, the different dynamics that exist and the culture of the organisation that is driving how work is carried out and what others think about each other and how, above all else, customers are served and products delivered. If fact-based management is the reason you have been tasked to do the strategy, then data gathering is a crucial component in your tool kit. It is at this data gathering phase that there will be road bumps.  Some will be willing to share the data and knowledge while others might be reticent in sharing the information. And you can begin to see the culture of the place! So, having the appropriate air cover from the crucial superiors, coupled with diplomatic skills, will help to navigate the terrain while you try to understand and fit into the culture.

Lean Six Sigma principles help in uncovering the workflow processes. There are 2 different ways by which this can be tackled.  You have already uncovered the Value Proposition by interacting with marketers to know the 4Ps and have an understanding of what constitutes the DNA of the organisation.  Along with this, the vision, purpose and the values are already there in the web site, so people are aware.  If employees are unaware, then this is something that needs to be revisited by including them in preparing the vision and purpose.  

***Note***:  *It is incumbent on leadership to ensure that employees are enlightened with strategy so that they know and understand that what they are doing is tied to the organizational goals and aligned with the values.*  

***Tip***: *One way of ensuring this is to use collaborative tools like Slack, Teams or Discord to celebrate successes that are aligned with goals and values, like collaboration, are mentioned in the channels for people to be recognised and everyone to see.*

The other way is to find out if there is a SIPOC (Supplier, Input, Process, Output and Customer) and a Process map.  If neither exists, then you have to start from the beginning and get the appropriate stakeholders to capture the information. This is also known as the ‘Discovery’ phase or the Define phase.  

SIPOC helps to map out the critical elements of the process.  It is a manual process where inputs from teams belonging to different departments are captured.  At first, I capture what are the processes that are currently being used by the different departments and try to gauge how they collaborate.  Then I understand who the customers are.  Sometimes the customers are internal and suppliers can also be internal customers who are providing the necessary inputs to the process.  This captures how business is conducted and what constitutes the voice of the customer(VOC).  

***Note***: *VOC constitutes the needs, wants and desires of the customer*

The gaps identified in the underlying process is what we are trying to improve; rather continuous improvement is the mantra that we need to abide to.  How much of the process is value-added and how much of it is not value-added can also be deciphered at this stage. Value-added is the process which directly affects the customer. Remember it’s the customer who is paying our salary.  They are willing to pay the price for the value that we are providing.  If the customer does not exist the business ceases to exist.  So in essence business exists to create values while customers derive values and there is a mutual exchange.  


***Note***: *Value creation is the act of transforming a set of inputs into outputs that generate revenue that is greater the costs incurred to make the product or deliver the service*

These are the core processes. Anything else that indirectly contributes to service delivery of the customer is non-value added.  For example, IT infrastructure, Finance, Supply Chain would be non-value added.  This is something that is essential but does not contribute directly to the customer.  The customer is not concerned how the IT system works.  This will not make the customer satisfied or dissatisfied as per Kano Modeling(4). The voice of the customer together with the voice of the process constitutes the voice of the business.  It is not possible to totally eliminate non-value added component as they are the enablers of running the business but reducing waste, like fixing a problem the first time, improves process efficiency.


***Note***: *TIMWOODS (Transportation, Inventory, Motion, Waiting, Overproduction, Overprocessing, Defects, (underutilised)Skills) is the acronym of 8 different kinds of wastes.  By reducing and eliminating these wastes you can improve the operational efficiency.*

ML algorithms can gather data in the processes from systems like ticketing systems and process logs, workflow systems and then analyse to identify bottlenecks and lags to make recommendations to suggest improvements.  This continuous method of feedback ensures that the dynamic system is reliant on both AI learning and human feedback.  It also ensures that to generate SIPOC, it reflects the current state and any changes in the process is captured while not depending on the human factor alone.  As discussed earlier you can see that learning is happening with both AI systems and human factors at the same time.


***Note***:  *All re-work is non-value added*

### Confluence {#Confluence}

The watering hole of any businesses operations is the application that deals with the service tickets; the main barometer of all the logged operations that the business is dealing with the customers.  Irrespective of whether it is a customer-facing job (the core processes of the business) or non-customer facing positions (non-value added), it is a repository of how customers are being served.  This is supposedly a veritable place of single source of truth where customers’ needs, wants and desires are captured. Some of the questions that I would ask is what kind of SLA (Service Level Agreement), OLA are in place.  What is the MTTR (mean time to resolve), MTTF (mean time to fail) and how many nines does the business provide?  

***Note***: *Number of nines indicate how long the system will be up and running.If you are using Cloud based system then the last one is provided by the Cloud vendor itself.  Amazon, for example, provides 12 nines.*

***Note***:  *If SLA does not exist this is the time that the business needs to be educated about the implications of not having one whether the customers are external or in-house.  If the business is not meeting the expected timeline across the distribution channel within which customers are to be served than other than unhappy customers, you also are at a risk of leaking revenue*

Tools like ServiceNow, Jira, vFire can be used to track the quality of the servicing. The inventory (the tickets in the system) in the database would reveal the MTTR, bugs and how the tickets have been resolved.  The throughput in the system, cycle time and takt time are the measures by which how the different departments are synchronised in serving the customers.  

***Tip***:  takt time τ=(Available Time)÷(Customer Demand) 

This also tells a lot about the culture in the organization.  If there is technical debt (4,5,6,7), then it can have dire consequences for not updating software versions can lead to duplicate issues that have not been resolved the first time! 

In formulating a strategy, depending on the type of business that you are operating in, the timeline for delivery can be 3 to 5 years.  In that situation, you want to ensure that there are not more than 5 to 8 priorities that you want to address.

The best way to prioritize items is to use a Pareto chart(80/20 rule) to identify which are the top most items that needs to be tackled.  Which or what kind of issues are consuming the most in the delivery of the operations?   What techniques are being used to do a root-cause analysis (RCA)? Are there any training programs that are being offered in the organization for employees to engage skills in troubleshooting? 

***Tip***: *5whys and Kepler-pegnoe are 2 examples of RCA*

For example, are there any bugs that you have identified?  Then that would be a defect. 
Quality may not be at the top of the priority list in some organizations even though they vouch for continuous improvement in their strategies!  Quality and safety, as we will discuss in chapter 6, go hand in hand.  As such, employees are not cognisant of the importance of quality and its importance in delivering value for the business.  If leadership have not implemented performance driven quality metrics, then it is difficult for employees to adhere to.  

The DMBOK framework lists Data Quality and Data Governance are the 2 main components.  AI, as you know, is trained on data and if the quality of the data, for example missing data, erroneous data, duplicate data that is not contextualised, traced back and rectified than erroneous result will be produced and you can clearly see how important Quality is.  In fact, Quality 4.0 uses AI to weed out inefficiencies, waste, and timely accuracy of the result.

***Tip***: *Tools like Powerdesigner, ERWIN can be used to do data modelling and also monitor Data Quality*

When I did a search on Github about AI, the top 5 topics about AI and the corresponding stars are shown in Table 1.  It might be different in your case as of this writing.

<table>
<thead>
<tr class="header">
<th>Rank</th>
<th>Repo Name</th>
<th>Repo URL</th>
<th>Stars </th>
<th>Main Topic</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>1</td>
<td>AutoGPT	175431</td>
<td>(https://github.com/Significant-Gravitas/AutoGPT)</td>
<td>3175431</td>
<td>AI</td>
</tr>
<tr class="even">
<td>2</td>
<td>stable-diffusion-webui</td>
<td>(https://github.com/AUTOMATIC1111/stable-diffusion-webui)</td>
<td>152597</td>
<td>deep learning</td>
</tr>
<tr class="odd">
<td>3</td>
<td>dify</td>
<td>(https://github.com/langgenius/dify)</td>
<td>7805</td>
<td>AI</td>
</tr>
<tr class="even">
<td>4</td>
<td>n8n</td>
<td>(https://github.com/n8n-io/n8n)</td>
<td>95917</td>
<td>Automation</td>
</tr>
<tr class="odd">
<td>5</td>
<td>open-webui</td>
<td>(https://github.com/open-webui/open-webui)</td>
<td>95259</td>
<td>Ollama</td>
</tr>
</tbody>
</table>

Table 1: The top 5 AI repositories in Github

***Note***: *The code for this result is in the author’s github repository*

***Tip***: *If you want to find out how many AI repositories have been created since January 1, 2025, you need to login Github and then filter out by the programming language and sort them based on the number of stars.  Here is the search condition that I used:
AI language:Python created:>2025-01-01 sort:desc  is:public*

The output (122K) is shown below

![Confluence](/assets/images/intro_strategy/media/image3-1.png)

Figure 1 :  Filtering out the AI repositories for current year


As you can see Ollama(1) is one of the main topics that is in the top 5 AI related repositories.  A good way of demonstrating how you can use AI to quickly recognise the kind of problems that any department or the organisation is plagued with is shown below.  In this case, we are going to use an open source LLM(Large Language Model) with Ollama that can be downloaded locally on your machine.  Ollama is an open-source generative AI tool.  The many benefits of using a tool like Ollama:

•	There is no cost associated with it and also the developmental community is large so you can seek help with the wider user community 
•	Since you can run the Ollama server locally in-house you do not have to communicate over the cloud and incur cloud based costs
•	You can then use many of the available foundational models like llama, mistral and others from hugging face to customize your applications including fine-tuning the models offering flexibility to your projects
•	Unlike OpenAI, Anthropic and other Generative AI systems you do not have to worry about sending data or uploading sensitive documents in contrary to company policies outside your company’s network.  Since data stays in-house there is enhanced privacy and security
•	Additionally, there is no restricted usage and not limited by the response and the usage of the number of tokens issued by API related LLM
•	Since the models are run locally this helps to augment the performance and reduce latency allowing models to be used for continuous analysis

***Note***: *Tokens are numerical IDs of the words that are broken down from text. This process is known as tokenization*

You can then use, for example, the organisation’s ticketing system or a manufacturing company’s defects as a data source for the model to work with and can then initiate prompt engineering to churn out charts. 

In this case, all you need is to seek access or ask for the dataset that you can use to demonstrate the usage of AI in what is impacting the efficiency of the operations. These charts will effectively display the exploratory data analysis and you can then use to identify the main problems and the root cause of them. You do not need to run around either for money or coax, cajole or exhort stakeholders as all you have to do is a few lines of code to make it work for you and then use the output to win the naysayers and have allies as your anchors.  You can use it to demonstrate a quick win that has tangible ROI. Bear in mind that a quick win enables you to scale up the operations across the organization otherwise it is a futile exercise.  Ensure that before you do a quick win the strategic objective has already been clearly stated so that you have the necessary stakeholders to marshal the required resources when you need. 

The dataset have been taken from Kaggle (2).  The dataset has 16 independent variables (columns) and one target variable. Each of the 16 columns are categorised under Production Metrics, Supply Chain and Logistics, Quality Control and Defect Rates, Maintenance and Downtime, Inventory Management, Workforce Productivity and Safety, Energy Consumption and Efficiency, and Additive Manufacturing.  The target variable is DefectStatus which is used to predict the defect status (0 indicates low defects while a value of 1 means high defects).

The application shows the kind of model you can select from the drop-down box on the left and then choose the csv (Comma-Separated Value) file. Once the file is loaded, it displays the top 3 rows of the dataset. You can scroll across the table to get a feel for the kind of data with which you are dealing. 

![Confluence](/assets/images/intro_strategy/media/image3-2.png)

Figure 2 :  Streamlit application showing the different LLM models to identify the defects in the manufacturing dataset

I then asked in the prompt to plot the heatmap so that I can explore if there are any correlations among the 16 independent variables.  This is shown in Figure 3 while the heatmap is shown in Figure 4.

![Confluence](/assets/images/intro_strategy/media/image3-3.png)

Figure 3 :  Application showing the Prompt to enter the question

***Note***:  *There are different kinds of prompts. The one shown here is called zero-shot learning as I have asked a single instruction to the LLM (mistral) model.  There is also few-shot learning where examples are included in the instruction so that a prompt can provide a better response.  This is also called in-context learning. In this example, my purpose is to demonstrate to my inner customers (staff at the company) the ease with which they can use generative Ai to solve their problems and at the same time pique their interest.*

![Confluence](/assets/images/intro_strategy/media/image3-4.png)

Figure 4 :  Heatmap showing the correlation among the different columns

From the correlation matrix, it can be seen that the following 4 columns are correlated:
ProductionVolume, MaintenanceHours, DefectRate and QualityScore.  You can see that QualitScore is inversely proportional to the other 3 variables. So if the number of defect rate goes down there will be an increase in the QualityScore.
ProductionVolume (in units/day) is one of the Performance metrics while DefectRate and QualityScore(in %) belongs to the category of Quality Control. MaintenanceHours (in hours) belongs to the category of Maintenance and Downtime.
Next, I asked for the distribution of the data for these columns in the prompt.  This is shown in Figure 5.

![Confluence](/assets/images/intro_strategy/media/image3-5.png)

Figure 5: Distribution of the data for the 4 independent correlated variables(columns)

From the above figure you can see that the probability of more defects peaks for production volume peaks after 800 units while for maintenance hours it peaks after 10 hours.
So let us find the root cause. We will use 5whys to prompt the model to find the root cause and the reasons behind it. 5whys is a technique in Lean Six Sigma where in order to find the root cause of the problem you ask a question starting with ‘why’ 5 times till you identify the problem. 
From Figure 6, you can see that the root cause behind the low Quality Score is due to high Defect Rate and Production Cost.  The reasons are also shown in the figure.


![Confluence](/assets/images/intro_strategy/media/image3-6.png)

Figure 6: Identification of the root cause(The average defect rate is 274.9%)

The average defect rate the LLM found was 274.9%.  This is incorrect.  The correct one is 2.78%.  LLMs are prone to put out erroneous result set.  Bear in mind that LLMs are probabilistic and not deterministic by nature. So you have to be mindful of what it spits out and accordingly select the appropriate model

***Note***: *While coding it is possible to validate the response!*

The crux of the matter in strategy is to generate value.  This can be done either by procuring more customers, improving service delivery and generating revenue.  The other option is to improve operational efficiency by improving quality and reducing wastes.  Earlier, in Section Lights on I mentioned the different kinds of waste of which defects is one of the waste that not only puts a dent to the operational efficiency but also reduces customer goodwill and affects the brand of the organization.   As the organisation tries to fix the defects it risks losing the customers to the competitors.  That’s why it is crucial that defects are captured early on and remediations are provided before the product is shipped out.  By removing any of the wastes we are eliminating any cost inefficiencies and rework associated with it but also adding to the improvement of operating cost which has direct bearing to the operating income.  In the next section, I will discuss how to evaluate ROI.

***Note***: *Operating income is also known as EBIT: Earnings Before Interest and Taxes
EBIT= (revenue-cost of sales)-operating expenses=(gross profit-operating expenses)*


### Return of Investment (ROI) {#Return of Investment (ROI)}

AI algorithms, and that includes LLMs as mentioned earlier, are stochastic(probabilistic) by nature and hence they can generate misleading or inaccurate outcomes.  When prompted LLM models, can make up information if they are not aware, a process known as hallucination.  As such, considerations should be made of both the tangible and intangible benefits that can be accrued while remaining vigilant on the negative implications of deploying such applications.  While the race is on, it’s even more important to ensure that a valid business case is made even at the project levels that aligns with the organizational strategy.  Fear of missing out should not be the reason for embarking on an AI solution specially if the domain that you are working on, AI is not the core process but an enabler.  This should not deter you from traversing the path.  However, with the advent of any new technologies there are concerns that employees and society at large might have.  While some might be beyond our control, business transformation is an essential ingredient of any organization that strategically decides to traverse the path.

Business’ existence is to generate value.  They come in 3 different forms: 
	Strategic Value
	Financial Value
	Non-Financial Value

All of these 3 values are intrinsically linked with each other.  The long term value of organization, usually between 3 to 5 years, is the strategic value that sets the goals the company is trying to achieve.  Financial value includes the tangible monetary metrics that most companies and shareholders, be it at the project, operational or at the wider business level, look into to see how the company is performing relative to the industry.  The metrics that I will be discussing are ROI, payback period and productivity.

AI solution can be categorized into hard and soft benefits. Hard benefits are those that are tangible like increase in revenue or reduction in cost while soft benefits are those that improves customer satisfaction by reducing lead time in answering questions (eg creating a chatbot to answer queries) and increasing employee trust, fosters innovation by spurring creativity and leading to the development of new products or services(automating routine jobs), improving operational performance by reducing defects and tasks without losing headcount. 

Hence when evaluating ROI (6,8,9) ensure that you factor in both the tangible and the intangible benefits. Also, a number of times organizations tend to evaluate ROI for each of the projects.  It is better to evaluate the projects at the portfolio level that way there is a synchronicity of the projects.

ROI is defined as follows:
ROI=[(Net Benefits-Investments)÷Investment]x100%

Anything greater than 1 is a positive ROI.  This is the hard-hitting financial metric that business executives care about.  The total investment includes all the costs associated with the implementation of AI while the Net Benefits are the tangible gains. 


<table>
<thead>
<tr class="header">
<th>Cost Components</th>
<th>QuickWin<br>Year 1<br>Amount($)<br>Inhouse</th>
<th>ScalingUp<br>Year 2<br>Amount($)<br>Inhouse</th>
<th>ScalingUp<br>Year 2<br>Amount($)<br>Cloud</th>
<th>Continuous Ops<br>Year 3<br>Amount($)<br>Inhouse</th>
<th>Continuous Ops<br>Year 3<br>Amount($)<br>Cloud</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Licensing (Open source + APIs)</td>
<td>10000</td>
<td>11000</td>
<td>11000</td>
<td>12100</td>
<td>12100</td>
</tr>
<tr class="even">
<td>Data Engineering / ETL</td>
<td>20000</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
</tr>
<tr class="odd">
<td>Cloud / Compute Infrastructure</td>
<td>15000</td>
<td>15450</td>
<td>15450</td>
<td>15913.5</td>
<td>15913.5</td>
</tr>
<tr class="even">
<td>Training / Change Management</td>
<td>5000</td>
<td>5150</td>
<td>5150</td>
<td>5304.5</td>
<td>5304.5</td>
</tr>
<tr class="odd">
<td>Maintenance/Support</td>
<td></td>
<td>5000</td>
<td>5000</td>
<td>5150</td>
<td>5150</td>
</tr>
<tr class="even">
<td>Model Quantization</td>
<td></td>
<td>8200</td>
<td>8200</td>
<td>0</td>
<td>0</td>
</tr>
<tr class="odd">
<td>Energy Costs</td>
<td></td>
<td>12000</td>
<td>7000</td>
<td>12000</td>
<td>7000</td>
</tr>
<tr class="even">
<td><strong>Total Cost</strong></td>
<td><strong>50000</strong></td>
<td><strong>56800</strong></td>
<td><strong>51800</strong></td>
<td><strong>50468</strong></td>
<td><strong>45468</strong></td>
</tr>
</tbody>
</table>

Table 1:Total Cost components

The following Assumptions are made (3,4,5)

<table>
<thead>
<tr class="header">
<th>Assumptions</th>
<th></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Units Produced/Yr</td>
<td>100000</td>
</tr>
<tr class="even">
<td>Cost/Defective Unit($)</td>
<td>200</td>
</tr>
<tr class="odd">
<td>Inflation(%)</td>
<td>3.00%</td>
</tr>
<tr class="even">
<td>Defect rate(%)</td>
<td>2.75%</td>
</tr>
<tr class="odd">
<td>Annual Defect Cost($)</td>
<td>550000</td>
</tr>
<tr class="even">
<td>MFP ($)</td>
<td>50000</td>
</tr>
<tr class="odd">
<td>Defect Reduction(using GenAI) (%)</td>
<td>0.25</td>
</tr>
<tr class="even">
<td>Annual Savings($)</td>
<td>137500</td>
</tr>
<tr class="odd">
<td>Annual Savings with MFP ($)</td>
<td>187500</td>
</tr>
<tr class="even">
<td><br></td>
<td><br></td>
</tr>
<tr class="odd">
<td><strong>Quantization & Energy Costs</strong></td>
<td></td>
</tr>
<tr class="even">
<td>Model Quantization/year ($)</td>
<td>8200</td>
</tr>
<tr class="odd">
<td><br></td>
<td><br></td>
</tr>
<tr class="even">
<td><strong>Energy Costs</strong></td>
<td></td>
</tr>
<tr class="odd">
<td>In-house/year ($)</td>
<td>12000</td>
</tr>
<tr class="even">
<td>Cloud-based ($)</td>
<td>7000</td>
</tr>
<tr class="odd">
<td><br></td>
<td><br></td>
</tr>
<tr class="even">
<td><em>*Using free open source model(Ollama) so Model development costs are not needed</em></td>
<td></td>
</tr>
</tbody>
</table>

Table 2: Assumptions made

Payback period=Total Cost÷Savings

The ROI and the Payback period for the 3 years are shown below

<table>
<thead>
<tr class="header">
<th>YEARS</th>
<th>ROI(%) [In-house]</th>
<th>ROI(%) [Cloud]</th>
<th>Payback Period (Inhouse)</th>
<th>Payback Period (Cloud)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>1</td>
<td>175.00</td>
<td>0</td>
<td>4.36</td>
<td>0</td>
</tr>
<tr class="even">
<td>2</td>
<td>142.08</td>
<td>165.44</td>
<td>4.96</td>
<td>0.38</td>
</tr>
<tr class="odd">
<td>3</td>
<td>172.45</td>
<td>202.41</td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

Table 3: ROI and Payback period(months) for both inhouse and cloud 


### Productivity {#Productivity}

In discussing the ROI of a Generative-AI from a Product manager’s perspective, productivity as the best metric was explored(7).  The formula for Productivity is:

Productivity=Outputs÷Inputs

The value of Inputs can be anything that is related to resources eg. Cost of materials, wages, any additional overhead while the value of outputs correspond to the production of goods and services.  Productivity can be tied to any specific measures that can be monitored for trends that requires improvement in the delivery of goods and services.  For example, you can monitor the productivity of printers to determine the efficiency of printers and find ways to improve the cost. The denominator is the number of printers.  The thing that you have to do is reduce the denominator while keeping the numerator constant.  

When exploring the usage of Productivity, two things need to be considered.  They are labour productivity and multifactor productivity(MFP).  Labour productivity is measured by which the number of hours worked or the cost associated with it provides an output.  MFP factors in all the resources (labour, materials, capital input, upskilling)  put in the production process to provide the necessary output.  Hence it is an index that measures the efficiency of the production process.   Growth in MFP is associated with “technological progress, organizational innovations or economies of scale”(10). However, as in the example above (section), where productivity improvements are determined by internal processes it can be difficult to quantify the costs associated with it.  In that sense, it is not deterministic but an approximation. 

***Note***: *Process maps containing swimlanes can map out the processes of a task as it traverses the different departments before the completion.*

In our example you can see using Gen-AI there is a better understanding of the product defects which leads to reduced costs and higher efficiencies.  Optimizing workflows and routine and tasks can increase output per labour hour (11, 12).  

***Tip***: Depending on the digital maturity of the organization (whether they are champions, followers, innovators or novices or a combination of any of them in each of the departments) you can then use them to generate an AI solution by having Human-in-the-loop(HITP) or fully autonomous with no humans in the loop. By having Human in the loop with AI and learning from each other you can develop mutual trust between AI and the employees.

From Table 1, you can see the amount of capital invested to get the application (Manufacturing Defect Root Cause Analysis) running and the labour skill upgrading that will manifest after the Quick Win demonstration and what you need to scale up AI.  As you can see the organizations’ capital investment in structure, either in Cloud based systems or inhouse equipment and intellectual property drives up labour productivity through upskilling.  At a high level the concomitant growth in labour productivity “determines the growth in Canada's GDP per capita and living standards”(14).

By factoring in productivity(Assumption of MFP($50000/year), the ROI and the payback is shown in Table 4.

<table>
<thead>
<tr class="header">
<th>YEARS</th>
<th>ROI(%) [In-house]</th>
<th>ROI(%) [Cloud]</th>
<th>Payback Period (Inhouse)</th>
<th>Payback Period (Cloud)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>1</td>
<td>275.00</td>
<td>0</td>
<td>3.20</td>
<td>0</td>
</tr>
<tr class="even">
<td>2</td>
<td>230.11</td>
<td>261.97</td>
<td>3.64</td>
<td>0.00</td>
</tr>
<tr class="odd">
<td>3</td>
<td>271.52</td>
<td>312.38</td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

Table 4: ROI and Payback period(months) while factoring MFP

You can see by including MFP in the calculation, the ROI has improved 57 %( [275-175]/175) in the 1st year alone while the payback period has reduced from 4.6 months to 3.2 months.  This is a significant increase in ROI.

## 🔗 Code Repository

The complete code and analysis tool is available on GitHub:

**[Exploring Current Business Internal and External Environment (Part 2)](https://github.com/sujpaul/AI-External-analysis)**


## References {#references} 
1\. <http://www.ollama.com>

2\. (https://www.kaggle.com/datasets/fahmidachowdhury/manufacturing-defects)

3\. https://cyfuture.cloud/kb/ai-data-center/breaking-down-ai-data-center-costs

4\. https://sujpaul.github.io/ai/strategy/ml/dl/Introduction-to-AI-Strategy-and-Business-Value/

5\. https://www.coherentsolutions.com/insights/ai-development-cost-estimation-pricing-structure-roi

6\. https://www.neurond.com/blog/generative-ai-roi

7\. (https://manishsharma.blog/2024/12/30/the-roi-of-generative-ai-a-product-managers-perspective/)

8\. (https://epoch.ai/gradient-updates/how-much-energy-does-chatgpt-use)

9\. "An Immersive Workshop to Calculate the ROI of AI Strategy - AUTONOMOUS session", https://www.youtube.com/watch?v=ZI2XuOfZ5iU

10\. https://www150.statcan.gc.ca/n1/daily-quotidien/250407/dq250407b-eng.htm

11\. Caranci, B., & Marple, T. (2023). "The AI Revolution: Opportunities and Challenges for Businesses and Workers." TD Economics. 

12\. "The economic potential of generative AI: The next productivity frontier", https://www.mckinsey.com/capabilities/tech-and-ai/our-insights/the-economic-potential-of-generative-ai-the-next-productivity-frontier



