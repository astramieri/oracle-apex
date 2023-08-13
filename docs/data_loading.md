# APEX Data Loading

You can add the data loading capability to an application by creating a **Data Load Definition** and then a **Data Load Page**. 

## Data Load Definition

A Data Load Definition comprises:
- data load definition
- data profile
- data profile columns

Data can be loaded either to an existing table in your schema or to a collection. For each data profile column, you can define a scale expression, SQL query lookups, or transformation rules.

Key Features:
- file type supported: CSV, XLSX, XML, JSON
- column mapping occurs at design time
- flexible column mappings based on simple names or regexp
- data conversion with transformation rules or lookup queries
- easy workflow: upload the file, verify the preview, and load data
- configure data loading to append, merge or replace data (with/without Error Handling)
- APEX_DATA_LOADING PL/SQL API available for custom processing
- maximum number of columns to load is 300

## Data Loading page

A Data Loading Page consists of a single page with a Native Data loading page process, which enables users to upload data from a file or copy and paste, preview the data, and then upload the data.

**NOTE**. Data Load Wizard is not designed or intended to load hundreds of thousands of rows of data.

## Data Loading Options

- Easy to use graphical interface
- Supports CSV, XLSX, TXT, XML or JSON files) or Copy and Paste (supports ONLY comma or tab delimited data)
- Loads/unloads tables only, one table at a time
- Access only to schema of logged-in user
- No data filtering on upload