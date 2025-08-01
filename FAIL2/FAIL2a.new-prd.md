# PRD: Dynamic Tables Demo System

## Executive Summary

We are building a simple demo that replicates Snowflake's Dynamic Tables functionality. This system will showcase the complete spectrum of Dynamic Tables capabilities including **incremental refresh patterns**, **full refresh strategies**, **cascading pipeline dependencies** in a notebook experience.

The demo will use the TPC-H dataset as outlined in the quickstart.

**Key Business Impact:**
- **Demonstrates Modern Pipeline Patterns**: Shows both incremental (cost-efficient, real-time) and full refresh (accuracy-focused, batch) approaches

**Success Metrics:**
- One notebook for incremental and full refresh patterns on Dynamic Tables
- 2 working pipeline examples with different LAG settings and refresh modes

Use this quickstart for coding examples: @https://quickstarts.snowflake.com/guide/getting_started_with_dynamic_tables/index.html?index=..%2F..index#0 
Use this docuementation for reference: https://docs.snowflake.com/en/user-guide/dynamic-tables-about

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