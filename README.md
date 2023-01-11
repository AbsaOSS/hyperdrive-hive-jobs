    Copyright 2018 ABSA Group Limited
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
        http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

# hyperdrive-hive-jobs
Hyperdrive hive jobs helps with operations in Hive.


### Jobs
#### RepairHiveTable - performs `MSCK REPAIR TABLE database.table`
How to execute RepairHiveTable
```
spark-submit --class za.co.absa.hyperdrive.hive.jobs.RepairHiveTable /path/hyperdrive-hive-jobs.jar \
  hive.metastore.uris=uri1,uri2,uri3 \
  table=database.table
```