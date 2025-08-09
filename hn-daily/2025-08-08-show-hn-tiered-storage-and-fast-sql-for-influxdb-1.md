# Show HN: Tiered storage and fast SQL for InfluxDB 1.x/2.x

**Posted by ignaciovdk on 2025-08-08**

If you’ve run InfluxDB at scale, you know the pain: retention policies often mean discarding valuable history, while keeping everything incurs huge hardware and license costs.

We built ExyData Historian to address this problem.

## What it does

- Automatically exports old InfluxDB 1.x/2.x data to compressed Parquet files stored in S3 or MinIO
- Keeps recent data "hot" in InfluxDB, moving older data to cheaper storage
- Enables fast SQL queries on archived data using Apache Arrow and DuckDB
- Provides a unified interface and API to query all data seamlessly — no hot/cold boundary for users

## Why it matters

- Reduces storage costs by 70–80%
- Ensures historical queries are as fast or faster than querying InfluxDB directly
- Eliminates manual exports, query rewrites, and downtime

## Who’s using it now?

InfluxDB Enterprise customers, large OSS instances, telcos, and logistics companies are testing it today.

We help you reduce your enterprise licensing costs by shrinking your InfluxDB cluster. You can keep your existing InfluxDB running while Historian works alongside it, moving historical data to inexpensive storage and enhancing your analytics capabilities.

We’d love feedback from anyone managing large InfluxDB deployments.