# kubernetes-wordpress

Step 1 : Apply the file wordpress-db.yaml to create all the resources required for the mysql to run.

Step 2: Create a database by accessing the mysql pod as a root and password configured earlier

kubectl exec -it mysql-pod-name -- bash

mysql -u root -p
CREATE DATABASE wordpress;
show databases;
exit

Step 3: Apply the file wordpress-frontend.yaml to deploy the application


step 4: Now you can access the application from the web.

