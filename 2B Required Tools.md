# **Required Tools**
### **dbSync**

Installation instructions can be found [here](https://github.com/IntersectMBO/cardano-db-sync/blob/master/doc/docker.md).

Ensure dbSync and the PostgreSQL database are running, and the database is synchronized past 10 pm UTC on the 23rd of August 2023.  

*Note: IF your dbSync is not synchronized to at least this date, the results from running a snapshot will be inaccurate.  This is because the snapshot is taken at a time when a rollback on the blockchain is impossible to affect the snapshot data, and therefore it's fully reproducible and stable.  This is guaranteed by placing one full Epoch between the registration deadline and the earliest the final snapshot can be taken.*

### **Catalyst Snapshot Tools**
Snapshot tools are from the [Catalyst Core github repo](https://github.com/input-output-hk/catalyst-core). Clone the repo and then build the necessary tools.

### **Building the tools**
**snapshot_tool:**
>cargo build -r -p voting_tools_rs

**catalyst-toolbox:**
>cargo build -r -p catalyst-toolbox
