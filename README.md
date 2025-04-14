# dp-203-lab-14
# Lab 14: Use Azure Synapse Link for Azure Cosmos DB

This repository contains my solution and notes for **Lab 14** of the Microsoft DP-203 course: *Use Azure Synapse Link for Azure Cosmos DB*.  
The lab demonstrates how to enable real-time analytics on operational data in Azure Cosmos DB using Azure Synapse Analytics.

## 🔧 Lab Objectives

- Provision Azure resources (Cosmos DB and Synapse Analytics)
- Enable Azure Synapse Link in Cosmos DB
- Create an analytical store container and insert sample data
- Connect Azure Synapse to Cosmos DB using Linked Services
- Query Cosmos DB data from:
  - Spark pool notebooks
  - Serverless SQL pool

## 📁 Structure

The lab was completed using the official Microsoft repo:  
👉 https://github.com/MicrosoftLearning/dp-203-azure-data-engineer

Relevant files and work were done under:  
dp-203/Allfiles/labs/14


## 📌 Key Steps

1. **Provision resources** using `setup.ps1` from Cloud Shell.
2. **Enable Synapse Link** in Azure Cosmos DB.
3. Create `AdventureWorks` database and `Sales` container with **Analytical Store** turned on.
4. Insert 3 sample documents manually via Data Explorer.
5. Open Synapse Studio and connect to Cosmos DB using **linked services**.
6. Use PySpark to:
   - Load data to a Spark DataFrame
   - Navigate nested JSON structures (`customerdetails`)
   - Create a logical table and query with Spark SQL
7. Use **Serverless SQL pool** and `OPENROWSET` to access Cosmos DB data.

## 📊 Sample Query Output

Using Spark SQL:

| id       | orderdate  | customername | product                     |
|----------|------------|---------------|-----------------------------|
| SO43701  | 2019-07-01 | Christy Zhu   | Mountain-100 Silver, 44     |
| SO43704  | 2019-07-01 | Julio Ruiz    | Mountain-100 Black, 48      |
| SO43707  | 2019-07-02 | Emma Brown    | Road-150 Red, 48            |

## ✅ Outcome

I successfully integrated Azure Cosmos DB with Azure Synapse Analytics and ran near-real-time analytics using both Spark and Serverless SQL.

---

##Secreenshots
![Screenshot 2025-04-14 at 17 41 01](https://github.com/user-attachments/assets/d01e3845-1f83-4841-953e-c40b8f178619)
![Screenshot 2025-04-14 at 17 40 38](https://github.com/user-attachments/assets/3f3b88f7-958f-4c98-b29d-8b9dc87a8491)
![Screenshot 2025-04-14 at 17 40 04](https://github.com/user-attachments/assets/12d8a9f3-85fb-4326-9580-39abd51266f8)
![Screenshot 2025-04-14 at 17 25 31](https://github.com/user-attachments/assets/918b280a-5333-49c6-bced-3cbf6e122e53)
![Screenshot 2025-04-14 at 17 23 53](https://github.com/user-attachments/assets/cde99b94-0d49-4e5f-95de-159a00939ff7)
![Screenshot 2025-04-14 at 17 19 10](https://github.com/user-attachments/assets/5f97a64a-4fbb-4778-b8a5-44c9f8289873)
![Screenshot 2025-04-14 at 17 18 19](https://github.com/user-attachments/assets/f8bd702e-6c6b-427c-acf2-1ecaef775b54)
![Screenshot 2025-04-14 at 17 17 33](https://github.com/user-attachments/assets/0faeaef9-75be-445c-9ba6-bdc20232852c)
![Screenshot 2025-04-14 at 17 15 39](https://github.com/user-attachments/assets/f4db60c7-b63b-4477-b709-e94b772ff4c5)
![Screenshot 2025-04-14 at 17 15 03](https://github.com/user-attachments/assets/be124208-36bd-4795-b6e5-693c40d3752f)
![Screenshot 2025-04-14 at 17 14 20](https://github.com/user-attachments/assets/b920004e-3834-41e8-832e-76d8cb9ca280)
![Screenshot 2025-04-14 at 17 10 22](https://github.com/user-attachments/assets/fadacba4-4c38-4175-ac71-3e763dac1e6c)
![Screenshot 2025-04-14 at 17 09 01](https://github.com/user-attachments/assets/7ec1939f-8b67-4e81-81b2-419041055cc9)
![Screenshot 2025-04-14 at 17 01 56](https://github.com/user-attachments/assets/05ad2b22-32bb-4d7c-8b28-8a3c1a87d0a6)
![Screenshot 2025-04-14 at 16 48 53](https://github.com/user-attachments/assets/4ad990bf-fb46-4767-af06-1a6aaf9136e2)



## 🧠 Skills Practiced

- Azure Synapse Analytics (Spark & Serverless SQL)
- Azure Cosmos DB configuration
- PySpark DataFrames and SQL
- JSON data querying
- Data integration across Azure services

## 🔗 References

- [Azure Synapse Link for Cosmos DB](https://learn.microsoft.com/azure/cosmos-db/synapse-link)
- [DP-203 GitHub Lab Repo](https://github.com/MicrosoftLearning/dp-203-azure-data-engineer)

