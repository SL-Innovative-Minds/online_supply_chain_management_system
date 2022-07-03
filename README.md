# Online Supply Chain Management System #

### Requirements ###

•	Site users are __Customer, Admin, Inventory Manager, Customer Care, Transport Manager__.


#### Customer ####

•	Customer should create an account (with E-mail and userdefined password) to proceed an order.

•	A customer account must contain __customer name, phone, e-mail and NIC number__. 

•	Duplication of e-mail and NIC number in the database is not allowed. 

•	An account must contain a cart. 

•	An account should have ongoing order list and canceled order list.

•	Confirmed and not confirmed orders should view in the ongoing order list and should contain the current state as __(confirmed or not yet confirmed)__.

•	A customer can place multiple orders.

•	Before confirmation of order, customer can update an order.

##### Paying methods ####

•	Customer should have the options to pay via __bank__ or __on-site__ when placing the order.

•	If the customer chooses to pay via __bank__, 
		
		* customer should receive a receipt of payment details with amount to be paid via email.
		
		* customer should upload image of the successful payment recipt with invoice number to the particular order description.
		
		* If the provided recipt is valid customer care should confirm the order.

•	If the customer chooses pay __on-site__, 
		
		* an e-mail containing total amount with order details should be sent.
		
		* Inventory Manager should consider order as confirmed when placed an order.(at this stage, consider the order is conformed)

#### Orders (in the customer domain) ####

•	Oders should view in the customer account as a list with order state __(confirmed, prepared, delivery, cancel)__ (in ongoing/cancel order list).

•	Order state should viewable to Customer, Transport Manager, Customer Care, Inventory Manager and the Admin.

•   Order must confirm only if the payment is placed. 

•   Order will be canceled with in __five(5) days__. There should be __three(3)__ periodical warning notification by then.
	
		* If the order is canceled, then particular order should be removed from the ongoing order list and then view it on the canceled order list.

#### Orders (in the customer care domain) ####

•	If customer notify to cancel the order to Customer Service, Customer Care should have the ability to proceed the cancelation.

#### Inventory ####

•	Inventory detail __(item code, name, price, quantity, available)__ should viewable to anyone. 

•	When an order is confirmed, the inventory details should update.

#### Inventory Manager ####

•	should update the inventory details when,
	
	* New stock is added from manufactures.
	
	* customer cancel a confirmed order with in five days.
 
#### Transport Manager ####

•	should have a separate view of all confirmed orders with customer details.