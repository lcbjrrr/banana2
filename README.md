| Feature | Delta Lake | Apache Iceberg | Notes |
| ----- | ----- | ----- | ----- |
| Schema Evolution | ✅ | ✅ | Both support add/rename/drop columns |
| Time Travel | ✅ | ✅ | Delta: by version/timestamp\<br\>Iceberg: by snapshot ID/timestamp |
| ACID Transactions | ✅ | ✅ | Both support atomic operations |
| Optimization | Z-Order | Z-Order & partition evolution | Iceberg offers more flexible partitioning |
| Metadata Format | Parquet \+ JSON | Avro (metadata) \+ JSON | Iceberg metadata is more compact |
| Table Format | Open specification | Open specification | Iceberg governed by Apache Foundation |
| Ecosystem Support | Databricks-centric | Multi-vendor | Iceberg has broader native support |
| Change Data Feed | ✅ | ✅ (via row-level deletes) | Delta's CDC is more mature |
| Streaming | Optimized | Supported | Delta has deeper streaming integration |

|  | [Use Snowflake as the catalog](https://docs.snowflake.com/en/user-guide/tables-iceberg#label-tables-iceberg-snowflake-as-catalog) | [Use an external catalog](https://docs.snowflake.com/en/user-guide/tables-iceberg#label-tables-iceberg-catalog-integration) |
| :---- | :---- | :---- |
| ***Read access*** | ✔ | ✔ |
| ***Write access*** | ✔ | ❌For Snowflake platform support, you can convert the table to use Snowflake as the catalog |
| ***Data and metadata storage*** | External volume (cloud storage) | External volume (cloud storage) |
| ***Snowflake platform support*** | ✔ | ❌ |
| ***Integrates with Snowflake Open Catalog*** | ✔ You can sync a Snowflake-managed table with Open Catalog to query a table using other compute engines | ✔ You can use Snowflake to query Iceberg tables managed by Open Catalog |
| ***Works with the Snowflake Catalog SDK*** | ✔ | ✔ |

