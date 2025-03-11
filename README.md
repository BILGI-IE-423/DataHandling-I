## Exercise 1: Working with Microbiome Data in Pandas

### Task 1: Importing the Data
- Import the dataset **microbiome.csv** using `pandas` and save it as `mb`.
- Display the first 5 rows of the dataset.

### Task 2: Using a Composite Index
- Import the dataset again.
- This time, set a **composite index** using the columns **Patient** and **Taxon**.
- Display the first 5 rows of the dataset.

### Task 3: Skipping Specific Rows
- Import the dataset while **skipping rows** 3, 4, and 6.
- Display the first 5 rows of the dataset.

### Task 4: Importing a Limited Number of Rows
- Import **only 4 rows** from the dataset.
- Display the imported data.

---

## Exercise 2: Handling Missing Data and Importing Excel Files

### Task 1: Recognizing Missing Data
- Import the dataset **microbiome_missing.csv** and display the first 10 rows.
- Observe how Pandas automatically recognizes `NA` and empty fields as missing values.

### Task 2: Checking for Missing Values
- Use Pandas to check for missing values in the dataset.
- Display the first 10 rows of the dataset with missing value indicators.

### Task 3: Importing Excel Data
- Import an Excel file **microbiome_MID2.xls**.
- Read the sheet named **"Sheet 1"** without using headers.
- Display the first 5 rows of the imported data.
