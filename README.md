# Assessment-in-Python-to-assess-the-knowledge-of-developers.-
Pizza Shop Management features Akrom would like control are various patterns of orders, customer queues, pizza ovens, and customer tables.

Pizza Shop Management System
Akrom wants to have his own pizza shop. 
But he is concerned about an issue regarding how to deal with customer-wait-queues. Akrom would like to see a model of pizza shop system that is scalable for various customer demands for simulation purposes.
So, he decided to test a model of pizza shop management system first and see how large pizza shop he can manage. 
Help Akrom implement an efficient simulation of pizza shop management system!
Pizza Shop
Pizza Shop Management features Akrom would like control are various patterns of orders, customer queues, pizza ovens, and customer tables.
Order
•	Order is a single request received when a customer or a group of customers come to Pizza Shop to eat-in. Order includes the number of customers per request, and the details of pizza they would like to have.
•	Order(s) comes and gets registered into the Pizza Shop system.
Pizza
•	Pizza is a single pizza item.
•	Pizza comes in different sizes, which are SMALL and LARGE.
•	There is a fixed time a one person (a customer) spends for finishing one whole pizza depending on that pizza size.
Oven
•	Oven cooks a pizza one after another. No multiple pizzas are cooked at any instance of time. 
•	There can be one or many ovens, with each its own pizzas-to-be-cooked queue.
•	There is a fixed time each oven spends to cook one pizza depending on pizza size.
•	There is a status that expresses the current status of the each oven, e.g. COOKING or EMPTY.
•	When there are more than one ovens, Pizza Shop Management System has to implement and decide a mechanism of allocating each pizza to the queue of a particular oven. Customers do not decide on this.
Table
•	Table is a place where customers receive their cooked pizza.
•	Each table has a fixed capacity to accommodate customers.
•	Customers belonging to the same order should start and finish eating together in one table. 
•	There is time to spend if a group of customers are reassigned and moved to a different table.
•	Customers should start eating only when all pizzas in their order are ready together. 
•	One table can serve more than one group of customers at a time.
•	Pizza Shop Management System has to allocate each ready order to a particular table. Customers do not decide which table they go to.
Timestamps
•	Pizza Shop Management System uses a virtual time and is called a timestamp.
•	There are two types of timestamps.
•	Timestamp A is used to configure only request arrival intervals. 
•	Timestamp B is used to configure the timing of oven(s), and table(s).
•	Timestamp starts at 0 and increases by 1 at a time. Duration of one time stamp for each type is fixed by Pizza Shop Management System.
Control method
•	See the Missions.docx for information on the pizza shops to be controlled.
•	Mission0_dataset.txt file contains input data for a small Pizza Shop.
•	Mission1_dataset.txt file contains input data for a large Pizza Shop.
•	One order consists of 5 data such as (Request Index, Issue time, Number of customers in the request, Number of large pizzas, Number of small pizzas )
•	What the Issue time means is the time the request arrived at.
o	Data (0,2,2,1,3) is a request of 2 people to eat 1 large pizza and 3 small pizzas at timestamp 2.
o	Data (2,30,5,10,0) is a request of 5 people to eat 10 large pizzas and no small pizzas at timestamp 30.
•	More than one requests can occur in the same timestamp.

Simulation should be showing the status of requests, ovens, and tables at any instance of the time.
Mission_sample_dataset.txt (Annotated)
_________________________________________________________________________________________________________________
Short simulation      brief description of the simulation
0,30,1,2,0            one customer arrives at timestamp (A) 30 into the simulation
1,35,5,5,2            five customers arrive at timestamp (A) 35 into the simulation
2,45,3,6,0            three customers arrive at timestamp (A) 45 into the simulation
3,45,1,0,2            one customer arrives at timestamp (A) 45 into the simulation
4,90,1,1,0            one customer arrives at timestamp (A) 90 into the simulation
END                   the "END" tag marks the end of the customer arrivals
_________________________________________________________________________________________________________________

