# Dynamic Table Query Examples

## Optimal for Incremental Refresh Mode

### Basic Incremental Operations
1. **Simple Aggregations** - Basic SUM, COUNT, AVG operations on streaming data
2. **Filter Operations** - WHERE clauses filtering on timestamp or ID columns
3. **Simple Joins** - INNER and LEFT JOINs between tables with proper join keys
4. **UNION Operations** - Combining similar datasets with UNION ALL

### Complex Incremental Operations
5. **LATERAL with FLATTEN()** - Parsing nested JSON/VARIANT data using LATERAL FLATTEN to extract array elements
6. **CTEs with Incremental Logic** - Common Table Expressions that build incremental transformations step by step
7. **IMMUTABLE UDF Usage** - Custom user-defined functions marked as IMMUTABLE for consistent deterministic results
8. **Window Functions (Incremental-Safe)** - LAG, LEAD, FIRST_VALUE, LAST_VALUE over partitioned data
9. **Time-Based Aggregations** - GROUP BY with date/time functions for rolling calculations
10. **Incremental Deduplication** - ROW_NUMBER() OVER (PARTITION BY key ORDER BY timestamp) for latest records

## Only Supported in Full Refresh Mode

### Non-Deterministic Functions
11. **ANY_VALUE Aggregations** - Selecting arbitrary values from grouped data where order is not guaranteed
12. **RANK Functions** - RANK() and DENSE_RANK() operations that depend on complete dataset ordering
13. **ROW_NUMBER Global Ordering** - ROW_NUMBER() without proper partitioning that requires full dataset scan

### Complex Analytics
14. **Percentile Functions** - PERCENTILE_CONT, PERCENTILE_DISC requiring full dataset analysis
15. **Cross-Partition Analytics** - Window functions that span across all data without proper partitioning
16. **Recursive CTEs** - WITH RECURSIVE operations that require iterative processing of complete dataset
17. **Non-Incremental Aggregations** - Complex statistical functions like STDDEV, VARIANCE over entire dataset
18. **Global Ranking Operations** - Operations requiring knowledge of complete dataset for accurate ranking
19. **Cross-Table Dependencies** - Queries with complex interdependencies that cannot be incrementally computed
20. **Non-Monotonic Calculations** - Operations where adding new data can change historical results