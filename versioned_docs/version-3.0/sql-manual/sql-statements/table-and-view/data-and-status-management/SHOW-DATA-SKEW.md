---
{
"title": "SHOW DATA SKEW",
"language": "en"
}
---

<!-- 
Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
distributed with this work for additional information
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.
-->



## Description

This statement is used to view the data skew of a table or a partition.

grammar:

`SHOW DATA SKEW FROM [db_name.]tbl_name [PARTITION (p1)];`



1. Only one partition must be specified. For non-partitioned tables, the partition name is the same as the table name.
2. The result will show row count and data volume of each bucket under the specified partition, and the proportion of the data volume of each bucket in the total data volume.

## Example

1. View the data skew of the table

   ` SHOW DATA SKEW FROM db1.test PARTITION(p1);`

## Keywords

SHOW, DATA, SKEW

