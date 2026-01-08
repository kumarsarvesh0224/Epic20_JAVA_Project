# Employee management app

Step 1 : Launch Docker desktop application

Step 2 : Open CMD and run -> docker pull cassandra:4.1 

Step 3 : run ->   docker run -d ^ --name cassandra ^ -p 9042:9042 ^ cassandra:4.1   command in the same CMD window

Step 4 : run ->   docker exec -it cassandra cqlsh     in the same CMD window

Step 5 : run inside cqlsh in one line ->  CREATE KEYSPACE employee_keyspace WITH replication = {'class': 'SimpleStrategy', 'replication_factor': 1}; USE employee_keyspace; CREATE TABLE employee ( id uuid PRIMARY KEY, name text, email text, salary double );

Step 6 : type -> exit and close the CMD window

Step 7 : Till here the database part is done

Step 8 : Now open the backend folder in IntelliJ ide 

Step 9 : Navigate to "employee_management_backend\src\main\java\com\example\employee_management_backend\EmployeeManagementApplication.java" file and run it.

Step 10 : Now open the frontend folder in VS Code.

Step 11 : Open a new terminal and execute the command "npm install". It will install package (Ignore the warnings)

Step 12 : In the same terminal execute "npm start". Wait for a webpage to launch in your browser

Step 13 : Booooooom... here is your Employee Management Dashboard

Step 14 : Give the details and test the application



