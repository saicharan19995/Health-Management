# Health-Management
Andriod Application that scans a barcode and stores the calories of that product to monitor the calories consumed by the user

#### This Andriod application consists of 2 types of logins
1. Admin Login: Where this login can add new products to the database and also confirm new products which are added by the user.
                It can be logined using a default by <br />
                                                    **Username: admin**
                                                    <br />
                                                    **Password: admin123**

2. User Login: Here user can login with Phone number as user name and Password.They get a page with history and to scan 

User Page : Where user can scan the barcode of the prodcut which they have consumed. This is stored in the history on the date of scaning.
            User can see the data and total consumption in the history page day wise.

Signup: It consists of information of user like Name,Email,Password,Phone number


*This aplication has given the user the feature to add new products if it is not found in database*
*The product added by user should be authenticated later by the admin to add it to the main database. This authentication is kept to verify the calories 
correctness for the product*

##### We have used Firebase Database
##### The Stucture of the Database

Data<br />
&nbsp;&nbsp;&nbsp;|____ Unique Barcode<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|_______Product Cal : Value<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|_______Product Name : Value<br />

User<br />
&nbsp;&nbsp;&nbsp;|____ Details<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|_______ Email : Value<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|_______ Name : Value<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|_______ Password : Value<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|_______ Phone : Value<br />

&nbsp;&nbsp;&nbsp;|____ History<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|____ Date<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|___ Time<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|_______ Product Cal : Value<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|_______ Product Name : Value<br />
<br />
User_Entry<br />
&nbsp;&nbsp;&nbsp;|____ Unique Barcode<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|_______Product Cal : Value<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|_______Product Name : Value<br />

**Data : Where the Products added are stored
User : Contains the details of the user and the history of the products scanned by them
User_Entry : The Products scanned by the user which are not in database.This data needs to be confirmed by the admin to move this data from User_Entry to Data**
