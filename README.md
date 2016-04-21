# hcc_testcase
- Karl Arao, OakTable, Oracle ACE, OCP-DBA, RHCE
- http://karlarao.wordpress.com


### The general workflow:

* First, setup the environment
    * 1_cr_table2.sh
    * 2_datagrow2.sh
* Then estimate the compression
    * hcc_estimate.sql
* Then create the actual HCC tables
    * hcc_tables.sql
    * hcc_tablespaces.sql
    * hcc_segments.sql
* Check the estimate vs real
    * hcc_validate.sql
* and validate the rows
    * hcc_comptype_rows.sql
    * hcc_comptype_all.sql
* Run some sample SQLs on HCC tables and instrument each run
    * run_stats_create.sql
    * hcc_test.sh
    * run_stats_hcc_query.sql
    * run_stats_query_all.sql
* You can also run some DML on the tables and validate the rows
* Lastly re-compress
