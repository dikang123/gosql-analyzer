# Go SQL Query Analyzer

The tool for analyzing SQL Queries to improve on Database Performance in DBMSs written in Go.



# Algorithm Abstract

We are starting with the MySQL DBMS at the start;

```psuedocode
console = Prepare_Analyzer_Console()

if console is ready

	start: Q = Get_SQL_Query()

	if Q is valid in MySQL
		M = Analyze_Query()
		
		if Q can be optimized
			OQ = Optimize_Query()
			return OQ

		return M, Q

	else 
		Q is invalid in MySQL
		
	Enter a valid query
	goto start

else
	exit(console)
```

Meaning of the following letters in the pseudocode;
* M = Metrics of the Q (query)
* Q = Query
* OQ = Optimized Query



# Analyse_Query() method

This section analyzes the query and returns a bunch of metrics useful to determine how the query can be made efficient such as;

* Query Analyzer Table
* Query Response Time Index(QRTi)
* Response Statistics
* Example Query
* Explain Query
* Graphs

For more information, check the [MySQL Enterprise Monitor](https://www.mysql.com/products/enterprise/query.html).



# Research Links / Resources about the project

To fully understand and capture the main idea about this project, you need to look at some of these links below;
* [MySQL Enterprise Monitor](https://www.mysql.com/products/enterprise/query.html) - Resource
* [A Tool for Analyzing and Tuning Relational Database Applications: SQL Query Analyzer and Schema EnHancer (SQUASH)](https://www.researchgate.net/publication/221398010_A_Tool_for_Analyzing_and_Tuning_Relational_Database_Applications_SQL_Query_Analyzer_and_Schema_EnHancer_SQUASH) - Research Paper.
* [Optimizing Queries with EXPLAIN](https://dev.mysql.com/doc/refman/5.7/en/using-explain.html).
* [How to Optimize MySQL Queries with Query Profiler](https://www.youtube.com/watch?v=WixrenRiTTE).
* [Steps & Procedure to Use MSSQL Query Analyzer](http://j2eetutorials.50webs.com/use-mssql.html).
* [SQL Server Query Analyzer](http://www.hitsw.com/support/kbase/sql_servers/SQL2000/Query_analyzer.htm).
* [The Guru's Guide to Transact SQL](http://ccs1.hnue.edu.vn/hoanpt/DBMS/REF/thegurusguidetotransactsql2000.pdf).
* [PERFORMANCE TUNING IN MICROSOFT SQL SERVER DBMS](http://www.ijcsmc.com/docs/papers/June2015/V4I6KJ13.pdf).
* [Automatic Performance Diagnosis and Tuning in Oracle](http://cidrdb.org/cidr2005/papers/P07.pdf).
* [SQL Server Execution Plans](https://download.red-gate.com/ebooks/SQL/eBOOK_SQLServerExecutionPlans_2Ed_G_Fritchey.pdf).
* [Techniques for improving the performance of SQL queries under workspaces in the Data Service Layer](https://www.ibm.com/support/knowledgecenter/en/SSZLC2_7.0.0/com.ibm.commerce.developer.soa.doc/refs/rsdperformanceworkspaces.htm).
* [SQL Server Query Optimization Techniques - Tips for Writing Efficient and Faster Queries](http://www.ijsrp.org/research_paper_jun2012/ijsrp-June-2012-07.pdf).
* [Query Optimization Techniques in Microsoft SQL Server](http://www.dbjournal.ro/archive/16/16_4.pdf).
* [Improve Your Queries; Hints and Tips for Using SQL](http://www2.sas.com/proceedings/sugi29/270-29.pdf).


# Other SQL Analyzer Tools (both online and offline)
* [Data Pine SQL Analyzer tool for MySQL](https://www.datapine.com/sql-query-analyzer).
* [Solar Wind SQL Query Analyzer](http://www.solarwinds.com/solutions/sql-query-analyzer).
* [EverSQL - Free Plan](https://www.eversql.com/sql-query-optimizer/?type=free).
* [AQUAFOLD - SQL Queries & Analysis Tool](http://www.aquafold.com/aquadatastudio/query_analysis_tool.html?gclid=CjwKCAjwo4jOBRBmEiwABWNaMZkQrmAfzbF38Bj4NQlv8degdcmG8hq_uPWjyIyyn5NacaKuGAO3TBoClKwQAvD_BwE).



# Future features

* Add support for other DBMSs like Oracle, PostgreSQL etc.
