# ADF-Pipeline_snowflake2adls

Native Snowflake connector
The native Snowflake connector for ADF currently supports these main activities:

Copy activity
Lookup activity
Script activity
The Copy activity is the main workhorse in an ADF pipeline. Its job is to copy data from one data source (called a source) to another data source (called a sink). The Copy activity provides more than 90 different connectors to data sources, including Snowflake. Snowflake can be used both as a source or a sink in the Copy activity. With this activity you can ingest data from almost any data source into Snowflake with ease. For the complete list of supported data sources, see the ADF Copy activities supported source/sink matrix table.

The second activity to consider in ADF is the Lookup activity. The Lookup activity is able to retrieve a small number of records from any of the supported data sources in ADF. The primary purpose of the Lookup activity is to read metadata from configuration files and tables, which can then be used in subsequent activities to create dynamic, metadata-driven pipelines. While you are able to call a stored procedure from the Lookup activity, Microsoft does not recommend that you use the Lookup activity to call a stored procedure to modify data. If you are trying to execute a stored procedure to modify data, then consider the Script activity, discussed next.

The third activity to consider in ADF is the new Script activity. This newly released Script activity in ADF provides the much anticipated capability to run a series of SQL commands against Snowflake. And importantly, this activity can be used to execute data manipulation language (DML) statements and data definition language (DDL) statements, as well as execute stored procedures. This gives users the flexibility to transform data they have loaded into Snowflake while pushing all the compute into Snowflake. It’s with this new activity that customers are now able to create end-to-end pipelines with Snowflake. For an announcement of the new Script activity, including a nice comparison of the Lookup and Script activities, see the ADF team’s recent blog post.
![image](https://github.com/rafiuddin999/ADF-Pipeline_snowflake2adls/assets/120626762/a8c1da08-8c34-4664-af57-d74b70817f56)
1. Browse to the Manage tab in your Azure Data Factory or Synapse workspace and select Linked Services, then click New:
![image](https://github.com/rafiuddin999/ADF-Pipeline_snowflake2adls/assets/120626762/1b0f1881-4ee4-4570-890d-325ad104ea24)
2. Search for Snowflake and select the Snowflake connector.
3. ![image](https://github.com/rafiuddin999/ADF-Pipeline_snowflake2adls/assets/120626762/e3dcd781-cf36-4e9c-9f6d-14b7f2f39fa8)

![image](https://github.com/rafiuddin999/ADF-Pipeline_snowflake2adls/assets/120626762/c665967a-3461-45f6-9cba-0dc25ca6e325)


![image](https://github.com/rafiuddin999/ADF-Pipeline_snowflake2adls/assets/120626762/b8dc7ea2-d4b8-4097-9287-35a0d1569baa)
