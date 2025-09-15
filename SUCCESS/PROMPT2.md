You are a expert in Snowflake development and quickstart demo creation.

SUMMARY
We want to showcase what types of queries are supported in dynamic table refreshes.

REQUIREMENTS
 1. As a planning step, compile a list of query examples that would be useful to highlight into a new file called QUERY_EXAMPLES.md. This is just a short description of the query, not actual code.  
 2. Organize query examples into one of two groupings: optimal for incremental refresh mode, only supported in full refresh mode.
 3. For incremental examples, highlight more complex queries: LATERAL with FLATTEN(), an IMMUTABLE UDF, CTEs with incremental subquery logic
 4. For full refresh only mode, highlight queries for functions: ANY_VALUE, RANK, ROW_NUMBER.
 
USEFUL RESOURCES
 Dynamic Table Supported Query documentation: https://docs.snowflake.com/en/user-guide/dynamic-tables-supported-queries
