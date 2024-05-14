
| Column Name        | Description                                           | Data Type |
|--------------------|-------------------------------------------------------|-----------|
| RowNumber          | Corresponds to the record (row) number and has no effect on the output. | integer   |
| CustomerId         | Contains random values and has no effect on customer leaving the bank. | integer   |
| Surname            | The surname of a customer has no impact on their decision to leave the bank. | string    |
| CreditScore        | Can have an effect on customer churn, since a customer with a higher credit score is less likely to leave the bank. | integer   |
| Geography          | A customer’s location can affect their decision to leave the bank. | string    |
| Gender             | It’s interesting to explore whether gender plays a role in a customer leaving the bank. | string    |
| Age                | This is certainly relevant, since older customers are less likely to leave their bank than younger ones. | integer   |
| Tenure             | Refers to the number of years that the customer has been a client of the bank. Normally, older clients are more loyal and less likely to leave a bank. | integer   |
| Balance            | Also a very good indicator of customer churn, as people with a higher balance in their accounts are less likely to leave the bank compared to those with lower balances. | real      |
| NumOfProducts      | Refers to the number of products that a customer has purchased through the bank. | integer   |
| HasCrCard          | Denotes whether or not a customer has a credit card. This column is also relevant, since people with a credit card are less likely to leave the bank. | string    |
| IsActiveMember     | Active customers are less likely to leave the bank.    | string    |
| EstimatedSalary    | As with balance, people with lower salaries are more likely to leave the bank compared to those with higher salaries. | real      |
| Exited             | Whether or not the customer left the bank.             | string    |
| Complain           | Whether the customer has a complaint or not.           | string    |
| Satisfaction Score | Score provided by the customer for their complaint resolution. | integer   |
| Card Type          | Type of card held by the customer.                     | string    |
| Points Earned      | The points earned by the customer for using a credit card. | integer   |

