# CLTV Estimation with BGNBD & GG and Sending Results to Remote Server
CLTV estimation is probabilistic lifetime value estimation with time projection.
First, we calculate the "conditional expected number of transaction" value using the BG/NBD model.
Then we calculate the "conditional expected average profit" value with Gamma Gamma Submodel.
Finally, we combine these values to obtain the CLTV value.

![young_old](https://user-images.githubusercontent.com/33136610/147093557-9ebb9dea-e1e7-4ab2-b3dc-ec396170ec50.png)

### Business Problem
An e-commerce site wants a forward projection for customer actions according to the CLTV values of its customers.
With the dataset you have, is it possible to identify the customers who can generate the most monetary value within 1-month or 6-month time periods?

### Dataset Story
The dataset named Online Retail II includes the sales of a UK-based online store between 01/12/2009 - 09/12/2011.
The product catalog of this company includes souvenirs. They can also be considered as promotional items.
There is also information that most of its customers are wholesalers.

### Variables
InvoiceNo - Invoice Number(If this code starts with C, it means that the operation has been cancelled) / StockCode - Product Code(Unique number for each product) /
Description - Product Name / Quantity - Number of Products(It shows how many of each product on the invoices have been sold) / InvoiceDate - Invoice Date / 
Unit Price - Invoice Price(Sterlin) / CustomerID - Unique Customer Number / Country - Country Name
