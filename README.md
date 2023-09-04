# iOS_store.cloudphotodb_Queries
Queries to use on the store.cloudphotodb database. Provides you with iCloud Photos Sync directions and other information

2023-9-3 Update - I have updated the queries for store.cloudphotodb based upon a community question. I had limited test store.cloudphotodb databases to use so please let me know if there appears to be any errors in the decoding.

Based on a small amount of recent testing I have created two new queries to identify more useful data from this database.

store.cloudphotodb - globals table contains data about the library

iOS##_store-cloudphotodb_Main_Query - idMapping, scopes, cloudCache, downloadQueue, statusCenter, remappedDeletes tables are included in this query.

iOS##_store-cloudphotodb_pushRepository_Query - pushRepository table is included in this query. This query can be used to identify original file names, file names, and other unique identifiers. Recommend reviewing the pushRepository.serializedRecord bplist for specific data.

iOS##_store-cloudphotodb_outgoingResourceANDResources_Query - outgoingResources and Resoureces tables are included in this query. This query will provide information about files being synced with iCloud. This will contain unique identifiers and other data that can be used to match up with files listed in other tables in store.cloudphotodb.
