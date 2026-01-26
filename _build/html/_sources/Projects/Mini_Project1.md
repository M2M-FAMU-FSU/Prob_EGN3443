## Mini Project 1 - Design an Email Inbox Server
*Check Canvas for Deadlines and Office Hours*

**Goal**: Determine and test the daily capacity of Email Inbox Server (EIS) for your entire team to minimize costs. 


The EIS service provider has a per-day-subscription-charge with \$1 per email thread (i.e., includes back-and-forths). A missed email thread will cost you $5 (every new email thread above your designed capacity). You will be *testing* your email server on the **first Monday to the following Sunday (7 days) in February**.

Test your proposed capacity on the mentioned testing period and provide the cost incurred during that period (example below). You are supposed to use past data from your team's inboxes to come up with an optimal EIS capacity (*testing* implies that you are not going to use the data from those dates to inform your design). You will be evaluated on your reasoning for your capacity design and *not the actual values*.   

In Outlook Email, you can use ``received: mm/dd/yyyy`` command in search bar to list the email threads on a particular day and count them. 

**Submission Requirements**
* Single pdf file (no more than 2 pages)
    * Describe your design and logic drawn from historical data (need not provide the past data).
    * Provide the *testing table* as below.

**Example Testing**
Say, your designed EIS capacity is 10 email threads per day. Thus, the subscription charge is \$10 per day. 



| Testing Day | Total \# of Email Threads | Subscription Cost | Overflow  Cost | Comments
| --- | --- | --- | --- | --- |
| Mon | 5| \$ $10$| - | Need to pay for the subscribed capacity though the \# is low
| Tue | 7 | \$ $10$| - |   
| Wed | 14 | \$ $10$ | $4 \times 5 = \$ 20$ |one missed email thread will cost you \$5
| Thur | 11 | \$ $10$ | $1 \times 5 = \$ 5$ |
| Fri | 5 | \$ $10$ |
| Sat | 3 | \$ $10$ |
| Sun | 2| \$ $10$|
| **Total** | | **\$70** |**\$25**|    






**Notes**
* Be creative, but provide clear logic on your proposed capacity for your team's EIS.
* Instructor/TA will not help you in contacting your team members. 
* Your team will receive a single grade irrespective of individual members' contributions. 
* You can use the *Complimentary Feedback* deadline to submit your project for feedback with no impact on your grades. 
* Costs provided above are hypothetical. 