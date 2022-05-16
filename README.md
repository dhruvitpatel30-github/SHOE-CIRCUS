# SHOE-CIRCUS
CSCI 466 GROUP PROJECT (WEB BASED STORE as SHOE-CIRCUS) at NORTHERN ILLINOIS UNIVERSITY


# CSCI 466 Group Project (Spring 2022)
# Web-based Store (300 pts)
Introduction
This is the group project for 466, in which i and my team members will be designing and developing an application using the tools covered in the class.
The project will involve using most of the elements learned in the class, from designing the database schema with an ER diagram,
to converting it to relations, to translating those relations into SQL DDL, and all the way to implementing the web application
with PHP/PDO.

# Application
The application i will be designing and implementing will be a web-based, database-driven tool that handles an online store.
I will be responsible for designing and implementing both the user-facing portion of the web store and the employee-facing
side.
# Inventory
My application allows the owner of a store to look at his inventory. which includes at minimum a list of all of the products
and how many of each of them are left.
It must also be able to showcase the products that are in stock. This includes a listing that indicates what items are available, as
well as another view that allows a user of the webpage to see details on an individual product. 
Each of the product detail pages should include a way of adding some number of the product in question to the shopping cart.
Shopping Cart
Each user will have a shopping cart. It starts off empty and grows as users add more items to it. Many products can be in a shopping
cart, and a user may intend to order than one of a given product. There must be a page where a user can view the current contents
of their shopping cart.
In this page, the user should have an option to remove things from the cart, or to change the quantity that they will be ordering.
In order to do this, i will need to store some kind of state information. There are many ways to do this, including writing info
to the database, hidden form elements, and session variables. 
Once the order has been submitted, the items ordered should be associated with the order, so they can be looked up later. The
shopping cart should reset to empty once the order is complete.
The page showing the cart should have a link to another page that allows them to check out.
# Checking out
The checkout page should allow the user to enter a shipping address, and billing information (see the note below). It will show
them, at a minimum, the total value of the items in their cart, and allow them to finish submitting an order.
Note: AT NO POINT SHOULD ANY ACTUAL CREDIT CARD INFORMATION BE ENTERED. MAKE UP
FAKE DATA AND KEEP YOUR BILLING INFO SAFE.
# Orders
When an order is placed, the info on the order needs to be placed into the database. When an order goes into the system, it will
be marked as “Processing”. This will be changed as the store workers fulfill orders. The application will need it to generate three
different views:
1 Order tracking for the user. The user should be able to visit a URL within site and see information on their order and
its current status. This would include things like whether the order has been processed, shipped, etc., as well as info on
tracking numbers for shipping. The amount paid for each order should be a part of this view, as well as the total amount
paid for all orders.
CSCI 466 Group Project (Spring 2022) 2 of 3
2 A list of all of the outstanding orders, which the employees of the store can use as a guide to know which items still need to
ship.
3 An order fulfillment page that allows store employees to see details on individual orders, and mark them as shipped, add
notes, contact the user, etc.

# CSCI 466 Group Project (Spring 2022) 3 of 3
What to turn in?
Submit, via Blackboard (one submission per group), the following:
1 The ER diagram (in PDF format) that you designed for the database that is used for the application. This should be your first
step, and the other steps should be based upon this ER diagram. It would be best to draw this with some sort of software,
but if no one in your group can make that happen, then hand-drawn and scanned diagrams will be accepted, but legibility
will be critical and points will be lost for anything a grader cannot read. All entities and relationships must be drawn, along
with any identifiers or intersection data. Other attributes do not need to be drawn, but must appear in…
2 … a description of all of the entities, relationships, and attributes that are a part of your ER diagram. This will obviously
include their names, their purpose, and any additional data that is important to know. This can be a part of your ER diagram
PDF, or a separate PDF file, but it must be present and easy to find.
3 In a PDF, include the relational schema of the database, converted from the ER diagram. Include information on which
attributes are primary/foreign keys, and make sure to identify what the home relation is for the foreign keys used. This can
be in the same PDF, or a separate one, but it must be present and in an obvious location. It should be based on the ER
diagram from before. We will check to make sure it matches, so make sure that any changes made are applied to the ER
diagram and the schema here.
4 An SQL script, suitable to run with MariaDB, containing the DML code to create the database designed and detailed in the
previous portions.
5 Another SQL script, suitable to run with MariaDB, that inserts the sample data needed to make your application run properly.
This should include at least 20 different products (of your choice), 5 customers, and at least one order per customer.
6 A tarball or zip file containing the PHP code and any additional web-facing files that implement the application.
7 A web link to your group’s application running on the student web server. This can be served from any of the group members’
public_html on turing/hopper, but it does need to be working there to facilitate grading. Make sure not to delete the
implementation until after grading has been completed.
DO NOT submit Word documents. It is acceptable to write them in Word, but make sure to print/export them to PDF before
submission.
