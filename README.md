# PortfolioProjectSQL
In the provided code, you are performing various data cleaning operations in SQL. Here's a breakdown of the operations and the SQL skills utilized:

Standardize Date Format:

Using the CONVERT function to convert the SaleDate column to the Date data type.
Populate Property Address data:

Selecting records from the NashvilleHousing table where PropertyAddress is null.
Ordering the results by ParcelID.
Dealing with NULL:

Joining the NashvilleHousing table with itself on ParcelID to find matching records.
Using the ISNULL function to replace null values in PropertyAddress with the corresponding value from another record.
Breaking out Address into Individual Columns:

Using string functions like SUBSTRING and CHARINDEX to split the PropertyAddress column into separate columns for address, city, and state.
Splitting Owner Address into three separate columns:

Using the PARSENAME function to split the OwnerAddress column into separate columns for street, city, and state.
Change Y and N to Yes and No in "Sold as Vacant" field:

Using a CASE statement to replace 'Y' with 'Yes' and 'N' with 'No' in the SoldAsVacant column.
Remove Duplicates:

Utilizing the ROW_NUMBER() function with the PARTITION BY clause to assign row numbers to duplicates based on multiple columns.
Selecting rows with row_num greater than 1 to identify and exclude duplicates from the results.
Delete Unused Columns:

Using the ALTER TABLE statement with the DROP COLUMN clause to remove the columns OwnerAddress, TaxDistrict, PropertyAddress, and SaleDate from the NashvilleHousing table.


In summary, the SQL skills demonstrated in the provided code include data type conversion, string manipulation, NULL handling, data extraction, conditional statements, duplicate removal, and column deletion.
