# Amazon_Vine_Analysis

### Background
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

### Deliverable 1 
Using your knowledge of the cloud ETL process, you’ll create an AWS RDS database with tables in pgAdmin, pick a dataset from the Amazon Review datasets and extract the dataset into a DataFrame. Transform the DataFrame into four separate DataFrames that match the table schema in pgAdmin. Then upload the transformed data into the appropriate tables and run queries in pgAdmin to confirm that the data has been uploaded.

### code to create tables

-- Create Active User Table

CREATE TABLE active_user (
 id INT PRIMARY KEY NOT NULL,
 first_name TEXT,
 last_name TEXT,
 username TEXT
);

CREATE TABLE billing_info (
 billing_id INT PRIMARY KEY NOT NULL,
 street_address TEXT,
 state TEXT,
 username TEXT
);

CREATE TABLE payment_info (
 billing_id INT PRIMARY KEY NOT NULL,
 cc_encrypted TEXT
);


![image](https://user-images.githubusercontent.com/57301554/121820089-71986a80-cc56-11eb-8170-f910a14a1b4d.png)

![image](https://user-images.githubusercontent.com/57301554/121820205-3fd3d380-cc57-11eb-9054-0f6c88af4b4c.png)


## Dataset for Analysis

![image](https://user-images.githubusercontent.com/57301554/121820264-89242300-cc57-11eb-8339-2a57d043e28e.png)

## Data Frames

## Reviews

![image](https://user-images.githubusercontent.com/57301554/121821970-0e143a00-cc62-11eb-947c-f677153fa625.png)

## Customers

![image](https://user-images.githubusercontent.com/57301554/121822018-4e73b800-cc62-11eb-9985-59f05279efc9.png)

## Products

![image](https://user-images.githubusercontent.com/57301554/121822024-5f242e00-cc62-11eb-84e3-6955949df728.png)

## Review

![image](https://user-images.githubusercontent.com/57301554/121822046-8844be80-cc62-11eb-8bc1-b745a36658fe.png)

## Vines

![image](https://user-images.githubusercontent.com/57301554/121822062-9db9e880-cc62-11eb-981e-a345736884c0.png)

### Loading the DataFrames into pgAdmin
- Make the connection to your AWS RDS instance.
- Load the DataFrames that correspond to tables in pgAdmin.
- In pgAdmin, run a query to check that the tables have been populated.

![image](https://user-images.githubusercontent.com/57301554/121822745-4cabf380-cc66-11eb-82c1-7116d249395c.png)

![image](https://user-images.githubusercontent.com/57301554/121822779-80871900-cc66-11eb-9370-489f385c194f.png)





