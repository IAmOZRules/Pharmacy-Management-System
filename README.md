# Pharmacy Management System
A Pharmacy Management System made using Node.js, Express.js and MySQL

### Steps to Run the Project:
#### Make sure you have MySQL and Node.js installed before you begin!

1. Clone this repository, and navigate to the repo directory.
2. In a terminal in the same directory, run ```npm i```.
3. Install NODEMON by running ```npm install -g nodemon```.
4. Open MySQL Workbench, and create a new schema (say ```pharmacy``` in this case).
5. In the repo directory, create a ```.env``` file in this format:
```
DB_HOST=localhost
DB_USER=root
DB_NAME=<schema name>
SESSION_SECRET=<any string longer than 8 bits>
DB_PASS=<your MySQL password>
```
6. Run the following commands in the workbench:
```
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '<your MySQL password>';
flush privileges;
```
7. Run the ```pharmacy.sql``` script in the ```pharmacy``` schema.
8. Once all this is done, run ```nodemon server.js``` in the terminal, and wait for the server to start.
9. In any browser, type ```localhost:8080``` to start the application.

#### To login, use ```username = tester``` and ```password = tester```.
#### NOTE: The "Requests by Patients" tab doesn't yet work! Opening it will crash the application!
