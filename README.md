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

---

## Exercise 3: Indexing, Querying, and Filtering in Pandas

### Task 1: Setting Index and Describing Data
- Import the dataset **baseball.csv** and set the `id` column as the index.
- Display the first 5 rows.
- Use the `describe()` method to summarize the dataset.

### Task 2: Checking Index Uniqueness
- Check whether the index is unique.

### Task 3: Creating a New Index
- Create a new index by combining **player** and **year** columns.
- Assign this index to a new DataFrame and check if the index is unique.

### Task 4: Identifying Non-Unique Indexes
- Find duplicate values in the index and display them.

### Task 5: Accessing Data Using Labels
- Select data using `loc` for a specific player-year combination.
- Use slicing with labels to retrieve a range of rows.

### Task 6: Creating a Unique Index
- Create a new unique index by combining **player**, **team**, and **year**.
- Assign this as the index and check for uniqueness.

### Task 7: Indexing and Slicing
- Perform NumPy-style indexing to retrieve the first three rows.
- Use `iloc` to retrieve rows and specific column slices.

### Task 8: Querying Data
- Use `query` to filter the DataFrame where **ab** (at-bats) is greater than 500.
- Use a variable (`min_ab = 500`) in a query by referencing it with `@`.

### Task 9: Filtering Data Using `isin`
- Use the `isin` method on **baseball** to find all players who played for the **Los Angeles Dodgers (LAN)** or the **San Francisco Giants (SFN)**.
- Count how many records contain these values.

---

## Exercise 4: Hierarchical Indexing, Operations, Sorting, and Calculating OBP

### Task 1: Hierarchical Indexing
- Create a hierarchical index using **year**, **team**, and **player**.
- Check if the index is unique.
- Retrieve **Julio Franco (`francju01`)** who played for the **Atlanta Braves (`ATL`) in 2007** using this hierarchical index.

### Task 2: Performing Operations on DataFrames
- Create two `Series` objects representing **home runs in 2006** and **home runs in 2007**.
- Set the index to the **player** column.
- Add these two Series together to calculate **two-year home run totals**.
- Display the first 20 results.
- Identify the players that appear in **both years**.

### Task 3: Handling Missing Data in Operations
- Use the `add` method with `fill_value=0` to replace missing values with **zero** in the two-year home run totals.
- Display the first 20 results.

### Task 4: Sorting Data
- Sort the dataset by index in **ascending order** and display the first 5 rows.
- Sort the dataset by index in **descending order** and display the first 5 rows.
- Sort **columns** in ascending order.
- Sort the `baseball` dataset by **home runs (hr)** in descending order and display the top 10 players.
- Sort by **stolen bases (`sb`)** in descending order and **caught stealing (`cs`)** in ascending order.

### Task 5: Calculating On-Base Percentage (OBP)
- Compute the **On-Base Percentage (OBP)** for each player using the formula:

  $$obp = \frac{h + bb + hbp}{ab + bb + hbp + sf}$$

- Add a new column **`obp`** to the `baseball` DataFrame.
- Ensure that if the denominator is **zero**, the OBP is set to **0.0**.
- Return the ordered series of **OBP values**.
