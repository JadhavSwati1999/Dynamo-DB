# Dynamo-DB
Dynamo Database Service
## **What is Amazon DynamoDB?**

Amazon DynamoDB is a serverless, NoSQL, fully managed database with single-digit millisecond performance at any scale.

DynamoDB addresses your needs to overcome relational databases' scaling and operational complexities. DynamoDB is purpose-built and optimized for operational workloads that require consistent performance at any scale.

## **Characteristics of DynamoDB**

- Serverless
- NoSQL
- Fully managed
- Single-digit millisecond performance at any scale

## **DynamoDB use cases**

- Financial service applications
- Gaming applications
- Streaming applications

## **Capabilities of DynamoDB**

- Multi-active replication with global tables
- ACID transactions
- Change data capture for event-driven architectures
- Secondary indexes

How to create a NoSQL Table

- Login to AWS Console using login credentials.
- Search for DyamoDB in the search box.

- Click on it and you will be directed to the dashboard of DynamoDB.
- Click on Create Table.


Create a table and give a name to the table.

The partition key is used to spread data across partitions for scalability. It’s important to choose an attribute with a wide range of values and that is likely to have evenly distributed access patterns. Type ***Artist*** in the **Partition key** box.

d. Because each artist may write many songs, you can enable easy sorting with a sort key. Enter **Mona Lisa** in the **Sort key** box.


 Next, you will enable DynamoDB auto-scaling for your table.

DynamoDB auto scaling will change your table's read and write capacity based on request volume. Using an AWS Identity and Access Management (AWS IAM) role called *DynamoDBAutoscaleRole*, DynamoDB will manage the scaling process on your behalf. DynamoDB creates this role for you the first time you enable auto scaling in an account.

To enable DynamoDB auto-scaling for your table, select **Customize settings.**

Scroll down the screen past **Secondary indexes, Estimated read/write capacity cost, Encryption at rest,** and **Tags** to the **Create table** button. We won't change these settings for the tutorial.


Now choose **Create table**.

When the ***Paintings*** table is ready, it appears in the table list with a check box.


## Add data to the NoSQL Table

In this step, you will add data to your new DynamoDB table.

 Select **Explore items** from the left menu, then select the radio button next to the **Paintings** table. Click the **Create item** button.


In the data entry window, type the following:

Artist- no one and Mona Lisa- The girl with rose


Repeat the process to add a few more items.

To create items.



Select the Scan. 

Select the checkbox next to *No one*. In the **Actions** dropdown list, choose **Delete items**. You will be asked whether to delete the item. Choose **Delete** and your item is deleted.



In this step, you will delete your DynamoDB table.

 You can easily delete a table by using the DynamoDB console. It is a best practice to delete tables you are no longer using so that you don’t keep getting charged for them.

- In the DynamoDB console, select the checkbox next to the *** Paintings *** table and then choose **Delete**.
- In the confirmation dialog box, enter the text *delete* and choose the **Delete** **table**.


## Summary

We created our first DynamoDB table, added items to our table, and then queried the table to find the items we wanted. We also learned how to visually manage our DynamoDB tables and items through the AWS Management Console.

DynamoDB is a great fit for mobile, web, gaming, ad tech, and IoT applications where scalability, throughput, and reliable performance are key considerations.
