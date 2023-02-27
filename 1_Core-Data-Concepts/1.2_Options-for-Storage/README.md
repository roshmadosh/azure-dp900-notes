### Describe common formats for data files
1. comma/tab/space-delimited rows: plain-text files, good for structured data (e.g. CSV)
2. JSON: good for structured or semi-structureds data
3. XML: like JSON but more verbose
4. Binary Large Object (BLOB): files stored in binary, typically for unstructured data like photos, videos, etc.

Special file formats: 
- Avro: Row-based data where the header is saved as a JSON and the data is saved in binary. Used to compress data files.
- Optimized Row Columnar (ORC) format: Stores data in columns instead of rows. **Stripes** hold one or more columns, an index into the rows of the stripe, the data for the rows, and a footer with aggregate statistics for each column (e.g. sum, average).
- Parquet: Columnar data storage. Data separated into row groups that each contain "chunks" of data. The Parquet file contains metadata that helps easily locate the correct chunks for a given set of rows.  
  

### Describe types of databases
- **Relational Databases**: Used to store and query structured data using SQL.
- **Non-relational Databases**: DB management systems that don't apply a schema. The four most common types are:
  1. key-value
  2. document-based: specific type of key-value storage in which each value is a JSON document.
  3. columnar
  4. graph-based  

