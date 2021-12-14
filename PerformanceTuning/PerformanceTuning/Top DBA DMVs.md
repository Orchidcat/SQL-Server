```SQL
-- List of all DMOs (DMVs & DMFs)

SELECT name,

 type,

 type_desc

FROM sys.system_objects so

WHERE so.name LIKE 'dm_%'

ORDER BY so.name;
```

Execution

[sys.dm_exec_connections](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-exec-connections-transact-sql) = Established connection  
[sys.dm_exec_sessions](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-exec-sessions-transact-sql) = Authenticated sessions  
[sys.dm_exec_requests](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-exec-requests-transact-sql) = Current requests

Execution (query related)

[sys.dm_exec_cached_plans](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-exec-cached-plans-transact-sql) = Cached execution plans  
[sys.dm_exec_query_plan](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-exec-query-plan-transact-sql) = Show plan for a given cached plan_handle  
[sys.dm_exec_query_stats](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-exec-query-stats-transact-sql) = Query performance stats  
[sys.dm_exec_sql_text](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-exec-sql-text-transact-sql) = SQL text given a sql_handle

Index

[sys.dm_db_index_physical_stats](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-db-index-physical-stats-transact-sql) = Index size and fragmentation  
[sys.dm_db_index_usage_stats](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-db-index-usage-stats-transact-sql) = index usage via the query optimizer  
[sys.dm_db_missing_index_details](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-db-missing-index-details-transact-sql) = Discover missing indexes

OS

[sys.dm_os_performance_counters](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-os-performance-counters-transact-sql) = List of all SQL Server performance counters and values  
[sys.dm_os_schedulers](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-os-schedulers-transact-sql) = Detect CPU pressure  
[sys.dm_os_waiting_tasks](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-os-waiting-tasks-transact-sql) = Tasks waiting on resources  
[sys.dm_os_wait_stats](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-os-wait-stats-transact-sql) = All waits types and stats

I/O

[sys.dm_io_virtual_file_stats](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-io-virtual-file-stats-transact-sql) = I/O stats for data and log files  
[sys.dm_io_pending_io_requests](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-io-pending-io-requests-transact-sql) = Pending I/O requests

CLR

[sys.dm_clr_loaded_assemblies](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-clr-loaded-assemblies-transact-sql) = Loaded assemblies  
[sys.dm_clr_tasks](https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-clr-tasks-transact-sql) = CLR related tasks