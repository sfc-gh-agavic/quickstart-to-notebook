# Dynamic Tables Demo - Task List

## Project Overview
Building a Snowflake Dynamic Tables demo using existing TPC-H sample data in `SFC_SAMPLE_DATA.TPCH_SF1` schema.

## Task Breakdown

### 1. Project Setup
- [ ] Set up project structure and Snowflake connection configuration
- [ ] Explore existing tables in SFC_SAMPLE_DATA.TPCH_SF1 schema (orders, customers, lineitem, etc.)
- [ ] Create demo database and schema for Dynamic Tables implementation

### 2. Dynamic Tables Implementation
- [ ] Create Dynamic Table with incremental refresh pattern using SFC_SAMPLE_DATA.TPCH_SF1 source tables
- [ ] Create Dynamic Table with full refresh strategy using SFC_SAMPLE_DATA.TPCH_SF1 source tables
- [ ] Build cascading pipeline dependencies between multiple Dynamic Tables

### 3. Demo Experience
- [ ] Create comprehensive notebook showcasing both incremental and full refresh patterns
- [ ] Add queries to monitor Dynamic Table refresh status and performance
- [ ] Test both pipeline examples with different LAG settings and refresh modes
- [ ] Document how to run the demo and explain the different patterns demonstrated

## Success Criteria
- ✅ One notebook demonstrating incremental and full refresh patterns
- ✅ 2 working pipeline examples with different LAG settings and refresh modes
- ✅ Uses existing SFC_SAMPLE_DATA.TPCH_SF1 tables as source data
- ✅ Shows cascading pipeline dependencies

## References
- [Snowflake Dynamic Tables Quickstart](https://quickstarts.snowflake.com/guide/getting_started_with_dynamic_tables/index.html)
- [Dynamic Tables Documentation](https://docs.snowflake.com/en/user-guide/dynamic-tables-about) 