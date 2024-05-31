# About the Holladn & Barrett data

1. Transaction data (sales_V1) 
  a. The folder contains sales data for H&B, covering the period 1 Jan 2018 – 21 April 2024. 
  b. The folder consists of 2,303 subfolders, one for each day from 1 Jan 2018 – 21 April 2024. Each sub-folder contains 16 excel files.
  c. H&B have provided sales data in slightly different formats pre and post 31 March 2021 due to a change in system. Below we summarise our understanding of the contents of the data provided for both periods.
  d. Data pre- 31 March 2021: 
      i. H&B have indicated that the data in this folder pre- 31 March 2021 is provided at the SKU/store/day level.  
      ii. Key variables include trading date, country, store ID, product SKU, product description, category, sales channel, quantity, base price, total price, VAT, and COGS. 
      iii. Does not contain information on payment method.
  e. Data post- 31 March 2021: 
      i. H&B have indicated that the data in this folder post- 31 March 2021 is provided at the transaction/SKU level.
      ii. Key variables trading date/time, country, store ID, product SKU, product description, category, sales channel, quantity, base price, total price, VAT, and COGS. 
      iii. Contains information on payment method.

2. Overheads (finance)
  a. The folder contains monthly overheads costs for H&B covering the period FY20 P1 – FY24 P6.
  b. The overheads costs data comes from two sources/systems: 
     i. Oracle EBS: FY20, FY21, FY22 (except Q4 for UK)
        1) Key variables include segment, period, currency, entered credit, entered debit.
        2) Countries can be identified by the variable ‘Segment 1’: UK = 303, Ireland = 309, Netherlands = 314, Belgium = 334.
     ii. Unit 4 ERP: FY22 Q4 for UK, FY23 and FY24 (H1)
        1) Key variables include transaction number, period, account description, cost centre, cost centre description, leg entity, transaction date, currency, amount.
        2) Countries can be identified by the variable ‘Leg Entity’: UK = HUK000, Ireland = HIE000, Netherlands = HNL000, Belgium = HBE000.
  c. Data is contained in the following sub-folders: 
     i.  UK Overheads Data (zipped): contains overheads costs for UK from FY21 P1 to FY23 P12.
     ii. New Data (zipped): contains overheads costs for
        1) Belgium, Netherlands, and Ireland from FY21 P1 – FY22 P12 (EUR – FY21 P1 – FY22 P12)
        2) UK from FY20 P1 – FY20 P12.
     iii. More New Data (zipped): contains overheads costs for 
        1) Belgium from FY23 P1 – FY24 P6 (Belgium FY23 P1 – FY24 P6).
        2) Ireland from FY23 P1 – FY24 P6 (Ireland FY23 P1 – FY24 P6).
        3) Netherlands from FY23 P1 – FY24 P6 (Netherlands FY23 P1 – FY24 P6).
        4) Belgium, Netherlands, and Ireland from FY20 P1 – FY20 P12 (EUR – FY20 P1 – FY20 P12).
        5) UK from FY24 P01 – FY24 P06. 
  d. For overheads costs data from the Oracle EBS system, we have removed three columns containing personally identifiable information. We will review in detail if any essential information in these columns can be retained upon cleaning and share updated files if necessary.
  e. For overheads cost data from the Unit 4 ERP system, we have removed a column containing further descriptions (in addition to the “Account Description” column) that also included personally identifiable information, e.g., the name of an individual claiming travel expenses.
