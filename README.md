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
