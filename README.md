# Megaline-Statistical-data-analysis

The telecommunications operator Megaline offers its customers two prepaid rates, Surf and Ultimate. The commercial department wants to know which of the plans generates the most income in order to adjust the advertising budget.

This project is a preliminary analysis of megaline rates: Ultimate and Surf, based on a selection of 500 clients of the company in 2018.

Customer behavior will be analyzed and with this it will be determined which prepaid rate generates the most income.
Determining which plan, on average, brings in more income is a question that will be addressed through statistical testing.

## General conclusions after data analysis:
1. *With the statistical analysis of the behavior of users in calls, messages and internet by plans, it is concluded that*:
     - For calls, in both plans the average number of monthly calls is around 6. The average number of monthly minutes is around 8.3 and the variance is around 28 in both cases.
     - For sending messages, the mean and variance behavior is also very similar. However, we can consider some surf plan users atypical, as they send many more messages than their plan covers. These users could probably be convinced to change their plan to ultimate, or adapt the surf plan to meet the needs of these users.
     - For internet use, we see that there is no difference in the behavior of the users, both groups of users use around 17 GB per month and the monthly internet traffic has a variance of around 60. However, it is evident that for the surf plan, this average exceeds the data included in the plan, so many users end up paying an extra cost for internet use.


2. *With the statistical analysis of the profit we see that the profits for each plan have a different mean and variance. This is confirmed by the hypothesis test, which tells us that there is indeed a difference between the profits of both plans.*
     - With these results it is concluded that although the average monthly income is a little higher in the ultimate plan, the surf plan has more users, and given that both groups of users demand a very similar data plan, minutes and messages, *I could recommend focus advertising and marketing strategies on this plan and also, extend the coverage of the surf plan in gigabytes and megabytes, to better meet the needs of the user population in general, since in this way, users will be more convinced of hiring the plan by not having to pay extra fees.*

 
3. *Similarly, when doing a hypothesis test to find out if the average earnings of the NY-NJ region are different from those of the other regions combined, we obtain a difference in these earnings as a result.*
     - This shows that the income obtained from a densely populated region such as NY-NJ cannot be compared with the income obtained from users in other regions, since the difference between income is clearly significant and even greater for the other regions, So, if we want to equalize profits in the NY-NJ region, a sales and/or advertising strategy should focus on this sector.
___

## Rates Description

**Note**: Megaline rounds seconds to minutes and megabytes to gigabytes. For calls, each individual call is rounded up: even if the call lasted only a second, it will be counted as a minute. For web traffic, individual web sessions are not rounded. Instead, the total for the month is rounded up. If someone uses 1025 megabytes this month, they will be charged for 2 gigabytes.

Below it can be seen a description of the rates:

#### Surf

- Monthly payment: $20.
- 500 minutes per month, 50 SMS, and 15 GB of data.
 -If package limits are exceeded:
- 1 minute: 3 cents.
- 1 SMS: 3 cents.
- 1 GB of data: $10.

#### Ultimate

- Monthly payment: $70.
- 3000 minutes per month, 1000 SMS, and 30 GB of data.
- If package limits are exceeded:
- 1 minute: 1 cent.
- 1 SMS: 1 cent.
- 1 GB of data: $7.
- Data Dictionary
- In this project, you will work with five different tables.

## Data Description:
#### users table (data about the users)
- ***user_id***: unique user identifier.
- ***first_name***: user's first name.
- ***last_name***: user's last name.
- ***age***: user's age (in years).
- ***reg_date***: subscription date (dd, mm, yy).
- ***churn_date***: the date the user stopped using the service (if the value is absent, the tariff was in use when this database was extracted).
- ***city***: user's city of residence.
- ***plan***: name of the tariff.

#### calls table  (data about the calls):
- ***id***: unique call identifier.
- ***call_date***: call date.
- ***duration***: call duration (in minutes).
- ***user_id***: identifier of the user making the call.

#### messages table (data about the SMS):

- ***id***: unique SMS identifier.
- ***message_date***: SMS date.
- ***user_id***: identifier of the user sending the SMS.

#### internet table (data about the web sessions):

- ***id***: unique session identifier.
- ***mb_used***: volume of data used during the session (in megabytes).
- ***session_date***: web session date.
- ***user_id***: user identifier.

#### plans table (data about the tariffs):

- ***plan_name***: tariff name.
- ***usd_monthly_fee***: monthly payment in US dollars.
- ***minutes_included***: minutes included per month.
- ***messages_included***: SMS included per month.
- ***mb_per_month_included***: data included per month (in megabytes).
- ***usd_per_minute*** price per minute after exceeding the package limits (for example, if the package includes 100 minutes, the operator will charge for minute 101).
- ***usd_per_message***: price per SMS after exceeding the package limits.
- ***usd_per_gb***: price per gigabyte of extra data after exceeding the package limits (1 GB = 1024 megabytes).

___ 
