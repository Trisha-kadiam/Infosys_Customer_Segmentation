# Customer Segmentation

## Task 1: Data Cleaning Process
Data cleaning is a crucial step in preparing datasets for analysis. It involves identifying and correcting errors or inconsistencies in the data to ensure its quality and reliability.

### Customer Dataset
1. **Check for Duplicated Values**: Verified for duplicated `CustomerID` entries.
2. **Remove Redundant Columns**: Found the `Full Name` and deleted the `First Name` and `Last Name` columns.
3. **Handle Null Values**:
   - **Gender**: Replaced null values with the mode.
   - **Customer Segment**: Replaced null values with the mode.
   - **Preferred Payment Method**: Replaced null values with the mode.
   - **Education**: Replaced null values with the mode.
   - **Marital Status**: Replaced null values with the mode.
   - **Age**: Replaced null values with the average age.
   - **Feedback Rating**: Replaced null values with the average feedback rating.
   - **Purchase Frequency**: Replaced null values with `0`.
   - **Loyalty Points**: Replaced null values with `0`.
   - **Occupation**: Replaced null values with `Other`.
   - **Referred ID**: Replaced null values with `Unknown`.
   - **Last Purchase Date**: Replaced null values with the current date.
   - **Join Date**: Replaced null values with the `Last Purchase Date`.
   - **Account Creation Date**: Replaced null values with the `Join Date`.
4. **Remove Duplicated Emails**: Eliminated duplicate email entries to ensure unique customer records.
5. **Data Type Verification**: Checked all data types to ensure they match the expected formats. Changed any mismatched data types accordingly.

### Products Dataset
1. **Remove Unnecessary Columns**: Removed the `Dimensions`, `Weight`, and `Color` columns.
2. **Handle Null Values**:
   - **Warranty Period**: Replaced null values with `0`.
   - **Stock Quantity**: Replaced null values with `0`.
   - **Product Name**: Removed any blank rows.
   - **Category**: Replaced null values with the mode.
   - **Rating, Price, and Discounted Price**: Replaced null values with their average values.
   - **Release Date**: Replaced null values with the values from the `Update Date` column.
3. **Data Type Verification**: Checked all data types to ensure they match the expected formats.

### Regions Dataset
1. **Remove Unnecessary Columns**: Removed the `Total Customers` column.
2. **Data Type Verification**: Verified data types to ensure they match the expected formats.

### Transactions Dataset
1. **Remove Unnecessary Columns**: Removed the `OrderNotes` column.
2. **Handle Null Values**:
   - **Loyalty Points**: Replaced null values with `0`.
   - **Shipping Cost**: Replaced null values with `0`.
   - **Refunded Amount**: Replaced null values with `0`.
   - **Discount**: Replaced null values with `0`.
   - **Gift Card Amount**: Replaced null values with `0`.
   - **Product Rating**: Replaced null values with `0`.
   - **Transaction Status**: Replaced empty values with `Unknown`.
   - **Quantity, Total Amount, Price Per Unit**: Replaced null values with their average values.
   - **Region ID and Transaction Type**: Replaced null values with the mode.
   - **Delivery Date**: Replaced null values with values from the `Update Date` column.
   - **Shipping Date**: Replaced null values with values from the `Update Date` column.
   - **Transaction Date**: Replaced null values with values from the `Update Date` column.
