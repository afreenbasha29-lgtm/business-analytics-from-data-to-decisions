# From Data to Business Decisions: A Practical View of Business Analytics

Business analytics is often associated with SQL queries, dashboards and statistical models. 
However, the real value of analytics comes from understanding a business problem, identifying 
the right measures, interpreting the resulting patterns and using them to support decisions.


1. Starting With the Business Problem
   
1.1 Data is not the starting point
Business analytics should start with a business problem, not with a query or dashboard. A company may have thousands of records, but the important question is what those records can help the business understand or improve.
For example, a hospital may want to understand which departments are handling the most patients, where waiting times are high, or whether high-revenue departments are also delivering a good patient experience. An airline may want to know which routes generate value, which customers travel frequently, or which customer groups contribute more revenue.
The same data can therefore be analysed in many ways depending on the decision that needs to be made.

1.2 Understanding the business structure
Before calculating anything, an analyst needs to understand how the business operates and how its data is organised.
In the hospital data, a patient visit connects patients, doctors, departments, diagnoses, treatments and payments. In the flight data, a ticket connects passengers with flights, airlines and airports.
This structure determines what can be compared. For example, hospital revenue can be analysed by department or payment method, while airline revenue can be analysed by airline or route.
________________________________________
2. Preparing Data for Analysis
2.1 Data quality affects business decisions
A business can make a poor decision from perfectly written SQL if the underlying data is incorrect.
Common issues include:
•	duplicate records
•	missing values
•	inconsistent categories
•	incorrect dates
•	incorrect relationships between tables
•	duplicated rows caused by joins
This is why data cleaning and validation are part of analytics itself.
For example, if a hospital visit is accidentally counted twice because of an incorrect join, the resulting department volume and revenue will both be overstated. The problem is not with the final calculation; it is with the data relationship used before the calculation.
2.2 Choosing the right level of detail
The level at which data is analysed can also change the result.
A hospital can be analysed at the visit level, but management may need information at the department level for resource planning. Similarly, airline data can be viewed at ticket level, passenger level, route level or airline level depending on the question.
Choosing the wrong level can produce technically correct but practically useless analysis.
________________________________________
3. Measuring What Matters
3.1 Revenue and volume
One of the simplest forms of business analysis is measuring activity and financial contribution.
In the hospital analysis, visits and revenue can be compared across departments. In the airline analysis, ticket sales and total revenue can be compared across airlines.
This helps answer questions such as:
Which departments are most active?
Which airlines generate the most revenue?
But the result becomes more useful when the metrics are considered together.
A department with high revenue may simply have a very high number of visits. An airline with high ticket volume may not necessarily generate the highest revenue.
This means that revenue and volume answer different business questions.
3.2 Revenue by payment method
The hospital analysis also compares revenue generated through different payment methods.
From a business perspective, this is not just a way of grouping transactions. It can help management understand how customers are paying and how much business activity flows through each method.
Depending on the actual business context, this could lead to further questions about payment convenience, transaction costs, customer preferences or dependence on particular payment channels.
The important point is that the initial analysis does not need to answer every question. It identifies where a business may need to investigate further.
________________________________________
4. Comparing Business Performance
4.1 Ranking
Ranking is useful when a business has many entities but limited management attention.
The hospital analysis ranks departments by revenue, while the flight analysis ranks airlines by revenue and airports by activity.
A ranking immediately makes the data easier to prioritise:
Which areas are performing strongly?
Which areas require attention?
Where is most of the business activity concentrated?
However, ranking alone is not enough to define success.
For example, a hospital department may rank first in revenue but have poor patient satisfaction. An airline may rank first in revenue but serve a very different customer or route mix.
Therefore, ranking should usually be followed by comparative analysis.
4.2 Comparing multiple dimensions
The hospital analysis combines department-level satisfaction and waiting time. This gives management a different view of performance.
A department with high patient volume and long waiting times may represent a capacity problem. A department with high satisfaction and lower demand may raise a different operational question.
This type of analysis helps move from:
“Which department is biggest?”
to:
“Which departments may require operational attention, and why?”
________________________________________
5. Customer Analytics
5.1 Segmentation
Customer analytics becomes more useful when customers are divided into meaningful groups.
The hospital analysis segments patients by age group and examines visit volumes and average bill amounts. The flight analysis examines passenger behaviour using number of flights, spending and frequent-flyer status.
Instead of asking:
“How much revenue do we have?”
a business can ask:
“Which customer groups generate the most value?”
This can support different decisions around customer retention, service design, loyalty programmes or targeting.
5.2 Identifying high-value customers
The flight analysis identifies the highest-spending passenger within each frequent-flyer status group.
This is useful because total customer count is not the same as customer value.
A small group of high-value customers may contribute a significant share of revenue. A business may therefore want to understand what these customers have in common, how frequently they travel and what keeps them returning.
However, the analysis only identifies a pattern. It does not prove why these customers spend more. Further analysis would be needed to understand the underlying drivers.
5.3 Customer preference
The flight analysis also identifies the most frequently used airline for each passenger.
This can help reveal repeat behaviour and potential loyalty patterns.
From a business perspective, the next question is not simply:
“Which airline does this customer use most?”
but:
“What characteristics are associated with repeat usage?”
That could lead to deeper analysis of route preferences, pricing, frequency, loyalty status or customer segments.
________________________________________
6. Operational Analytics
6.1 Finding bottlenecks
Analytics can be particularly useful for identifying operational bottlenecks.
In the hospital data, waiting time and patient satisfaction can be compared across departments.
Suppose one department has both unusually high waiting times and lower satisfaction. This does not immediately tell management what to change, but it identifies a problem worth investigating.
Possible explanations could include:
•	higher patient demand
•	staffing constraints
•	scheduling problems
•	resource availability
•	case complexity
The data therefore helps management locate the problem before investigating its cause.
6.2 Capacity planning
The monthly visit analysis provides another operational perspective.
If visit volumes change over time, management can examine whether the pattern is seasonal, growing or declining.
This can influence decisions related to:
•	staffing
•	scheduling
•	resource allocation
•	capacity planning
A simple monthly count is descriptive. But once the business understands the pattern, it can move towards forecasting future demand.
________________________________________
7. Using Time and Trends
7.1 Why trends matter
An overall number tells us what happened across an entire period. A time-based analysis tells us how that activity changed.
For example, monthly hospital visits and running totals can show whether demand is increasing and where peaks occur.
For an airline, similar analysis could be applied to ticket sales, route demand or revenue over time.
This becomes particularly useful when the business must plan ahead.
7.2 Alternative methods
A simple monthly aggregation may be sufficient for understanding historical activity.
However, other methods could be used depending on the business question:
•	Moving averages to reduce short-term fluctuations
•	Year-over-year comparisons to understand growth
•	Seasonal analysis to identify recurring patterns
•	Time-series forecasting to estimate future demand
The method should follow the decision. There is little value in building a complex forecasting model if the actual business question is simply whether activity increased compared with the previous month.
________________________________________
8. Making Inferences Carefully
8.1 From observation to explanation
Analytics becomes more valuable when it moves beyond describing a number.
Suppose a hospital department has long waiting times and low satisfaction.
The data gives us an observation.
We can then form a hypothesis that capacity or scheduling may be contributing to the problem.
But we should not immediately claim:
“Waiting time caused low satisfaction.”
The available analysis may not establish that relationship.
This distinction becomes important when decisions are expensive or difficult to reverse.
8.2 The importance of sample size
The doctor satisfaction analysis applies a minimum of 100 visits before comparing average satisfaction scores.
This is a useful example of how context changes interpretation.
A doctor with a very high average satisfaction score based on only a few visits may look better than a doctor with a slightly lower score across hundreds of visits.
The business lesson is simple:
A metric should be judged together with the amount and quality of data behind it.
________________________________________
9. Choosing the Right Analytical Method
9.1 Descriptive analysis
Descriptive analysis answers:
What happened?
Examples include:
•	total visits
•	total revenue
•	tickets sold
•	monthly activity
•	revenue by airline
This is usually the first stage of analysis.
9.2 Diagnostic analysis
Diagnostic analysis asks:
What could be behind the pattern?
Examples include:
•	comparing satisfaction with waiting time
•	comparing department performance
•	examining passenger spending by loyalty status
•	identifying differences between routes
It helps narrow down possible explanations.
9.3 Predictive analysis
Predictive analysis asks:
What could happen next?
For example, historical demand could be used to forecast hospital visits or airline demand.
This can support decisions involving staffing, inventory, capacity or scheduling.
9.4 Experimentation
Sometimes historical data cannot answer the business question.
Suppose a company believes that changing a customer offer will increase purchases. Historical analysis may show that certain customers already behave differently, but it cannot necessarily determine whether the new offer caused the increase.
An experiment such as an A/B test can provide stronger evidence about the effect of the change.
This is an important progression:
Analysis identifies an opportunity → experimentation tests the intervention.
________________________________________
10. Where Analytics Can Become Misleading
10.1 Correlation versus causation
Two variables can be related without one causing the other.
For example, higher patient volume may occur alongside lower satisfaction, but staffing, case complexity or scheduling could also influence both.
Therefore, analysts should distinguish between:
What the data shows
and
What the data proves.
10.2 Aggregation can hide important differences
An overall average can hide major differences between customer segments, departments or routes.
For this reason, businesses often need to analyse data at several levels before making a decision.
10.3 Missing information
A dataset may not contain every variable that affects business performance.
A flight database may show ticket price and passenger behaviour but not necessarily the customer's reason for choosing a particular airline. A hospital database may show waiting time but not every operational reason behind it.
The absence of a variable does not mean the factor does not exist.
________________________________________
11. From Insight to Business Action
11.1 What makes an insight useful?
An insight is useful when it changes what a business should examine or decide.
For example:
High hospital waiting time
→ investigate capacity, staffing or scheduling.
High-value airline customers
→ investigate retention and loyalty opportunities.
High-revenue routes
→ examine demand, pricing and capacity.
Increasing hospital demand
→ consider future resource and staffing requirements.
The analysis does not necessarily provide the final answer. It helps the business decide where to focus next.
11.2 Recommendations should match the evidence
If the analysis only establishes a pattern, the recommendation should be presented as a hypothesis or an area for further investigation.
This prevents a common analytical mistake:
turning a descriptive result into a causal conclusion.
A strong recommendation therefore considers both the opportunity and the strength of the evidence.
________________________________________
12. The Final Goal: Better Decisions
The complete analytics process can be viewed as:
Business Problem
↓
Understand the Data
↓
Prepare the Data
↓
Select KPIs
↓
Analyse Patterns
↓
Test Explanations
↓
Develop Insights
↓
Recommend Action
↓
Measure the Outcome
The final output is not the SQL query or the dashboard. Those are tools used along the way.
The real output is a better understanding of the business and, ultimately, a better decision.
Conclusion
Business analytics connects data with the decisions that businesses make every day. SQL can help identify patterns, statistical methods can help evaluate whether those patterns are meaningful, and visualisation can make the findings easier to communicate. But none of these methods are useful in isolation.
The value comes from understanding the business context, choosing the right metrics, questioning the results, recognising the limits of the data and connecting the findings to an actual business action.
A good analyst therefore does more than answer “What happened?”
The more important questions are:
Why might it have happened?
What can we reasonably infer from the data?
What can we not conclude yet?
And how can this information help the business make its next decision?

