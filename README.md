# IMS

In this project, I have build a simple inventory management system (IMS) for a grocery store using json (NoSQL db) file. It provides an easy way to keep a track of the products, customers and orders/transactions information. It also prints a bill invoice for every transaction done and update the inventory after every operation which involves any data manipulation of product's details. 

Backend - Python

_**record.json** contains the product details of all the products present in the inventory._

_**sales.json** contains the order details of every transactions done._

**Product**
* Number of attributes : 10
  * product id, product name, purchase price, sale price, quantity, food category, expiry date, size, brand name, and weight
* Features
  * Add new products,
  * Delete existing products,
  * Update features (like sale price, quantity or purchase price) of any product, and
  * Check stock availability.

**Order**
* Number of attributes : 10
  * order id, customer name, mobile number, product id, time of purchase, mode of payment, quantity purchased, billing amount, and profit made
* Features
  * Total number of sales done,
  * Profit we made in an entire day, and
  * Total billing amount of sales done.

**Functionalities in the User Interface:**
  1. Display the different kinds (such as beverages, snacks, etc.) of products
  2. Display different products belonging to a particular category
  3. Display different features (such as brand name, unit price) of a product
  4. Place an order
  5. Add new products into the inventory
  6. Update any feature of a product
  7. Delete any existing product from the inventory
  8. Check stock availability

Note : 
* Since order() in _inv_mgmt_sys.ipynb_ allows any user to purchase only one kind of product at a time, I have overcome this limitation in _ims_omp.ipynb_.
  * ord_multiple_prod() function in ims_omp.ipynb - allows user to order multiple products at a time.
* _ims_omp.ipynb_ uses prod_record_mp.json as database file and yields sales_mp.json as the output file containing all the transaction details.
* _inv_mgmt_sys.ipynb_ uses record.json as database file and yields sales.json as the desired output file.
* Added a new attribute as unit_price of purchased product to _order_ and a new functionality as check_stock_available() to check available stocks in _ims_omp.ipynb_ notebook.
