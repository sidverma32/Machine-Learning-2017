# Future-Datathon
Hackerearth Future Group Datathon

In this problem, you've to predict clusters of customers by store location. Knowing the set of customers that behave evenly will help them target their product promotions accordingly.

**Score on Private Leaderboard:** 1.00 (**Rank 1**)



## Data Description

The dataset consists of Big Bazar consumers.

BigBazaar runs various loyalty programs, festive offers which provide their customer more opportunities to avail discounts. Customers can use these offers or loyalty program to either avail discount or make payment.

**products.csv** <br />
This file contains products transaction information and highlights the discounts used by customers in each transaction.

**Features**<br />
<br />

**Variable**	Description <br />
**customerID**	unique customer ID <br />
**DOB**	date of birth of customer <br />
**Gender**	Gender <br />
**State**	customer's state<br />
**PinCode**	pincode of area where customer lives<br />
**transactionDate**	date of transaction<br />
**store_code**	unique code of big bazaar store<br />
**store_description**	description of store<br />
**till_no**	counter no. in the store<br />
**transaction_number_by_till**	unique transaction number by counter, transactionDate, store_code<br />
**promo_code**	if promotional code (offer) used in the transaction<br />
**promo_description**	description of the offer<br />
**product_code**	unique code of the product purchased<br />
**product_description**	description of the product purchased<br />
**sale_price_after_promo**	sale price of the product after applying promotion<br />
**discountUsed**	after promo, customer used this discount(s) on transaction<br />
<br />

**tenderModes.csv** <br />
This file contains information on payment mode(s) used by a customer in making a transaction.


**Variable**	Description<br />
**customerID**	unique customer ID<br />
**DOB**	date of birth of customer<br />
**Gender**	Gender<br />
**State**	customer's state<br />
**PinCode**	pincode of area where customer lives<br />
**transactionDate**	date of transaction<br />
**store_code**	unique code of big bazaar store<br />
**store_description**	description of store<br />
**till_no	counter no.** in the store<br />
**tender_type**	mode used to make payment<br />
**transaction_number_by_till**	unique transaction number by counter, transactionDate, store_code<br />
**payment_amount_by_tender**	amount paid using the payment mode<br />
**PaymentUsed**	description of mode of payment<br />


**Evaluation Metric**<br />

Submission will be evaluated based on:

score = silhouttescore - (weight * silhouttescore)

The weight applied is based on the number of clusters of customers per store.
