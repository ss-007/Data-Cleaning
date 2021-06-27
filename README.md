# Data-Cleaning

All of my data cleaning can be done with Pandas, since the dataset is small enough and is just one table. In order to clean the data and ensure it is on a usable format for the end user I've performed the following operations:

- Replace all nan values with '' (empty strings), as it is easier to handle strings with Python.
- Ensure updateTime is of DATETIME type and then format it to YYYY-MM-DD
- Create FullAddress from columns street, city, zip and State only if they all are present, otherwise set the row to empty.
- Ensure that only Y or N are used in all bin columns, which are the products that are offered in the market. Any value that is not Y defaults to N.
- Using regex ensure that the columns Website, Facebook and Youtube follow a URL format.
- Ensure that Twitter uses @username format.
- Ensure that season date uses a MM/DD/YYYY to MM/DD/YYYY format and that its season time is present.
