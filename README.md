#ANALYSIS OF THE SALES PREDICTION

This Sales data contains the Following Columns:

1. InvoiceNo	Invoice number; Unique identifier for a transaction.

2. StockCode	Product (item) code.

3. Description	Product name/description.

4. Quantity	Quantity of product purchased per transaction
.
5. InvoiceDate	Date and time of invoice creation.

6. UnitPrice	Price per unit of product.

7. CustomerID	Customer identifier (can be null).

8. Country	Country of customer. 

Initially, the CSV file containing the data had several missing values, missing values were handled properly by pandas,used forward fill and NA, the description attribute and the customer ID attributes were missing, so based on the necessity null values in Missing were filled with NA and the Customer ID was filled using Forward fill.

And then the total_sales were calculated by aggregating the unit price column.

with the unit price we used the ARIMA MODEL to forecast the Next 7 days Revenue.

The next Seven days dates and their mean revenue were plotted and stored for analysis

Tech Stack:

1. Pandas(To handle the Data)

2. Matplotlib (for creating plots)

3. statsmodel (To Load Arima)

4. ARIMA Model : This Model is both an auto regressive model and integrated - which handles flexible data points
                 and can be used for stock, finance and weather related forecast tasks.

