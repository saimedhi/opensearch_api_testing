1. Using GET 

`GET https://localhost:9200/_plugins/_knn/models/_search`

```
{
    "took": 6,
    "timed_out": false,
    "_shards": {
        "total": 1,
        "successful": 1,
        "skipped": 0,
        "failed": 0
    },
    "hits": {
        "total": {
            "value": 4,
            "relation": "eq"
        },
        "max_score": 1.0,
        "hits": [
            {
                "_index": ".opensearch-knn-models",
                "_id": "S56iHcluS1-d1L1_Fw3e9Q",
                "_score": 1.0,
                "_source": {
                    "engine": "faiss",
                    "space_type": "l2",
                    "description": "My model",
                    "model_id": "S56iHcluS1-d1L1_Fw3e9Q",
                    "state": "failed",
                    "dimension": 2,
                    "timestamp": "2024-02-21T00:04:09.691400710Z"
                }
            },
            {
                "_index": ".opensearch-knn-models",
                "_id": "model1",
                "_score": 1.0,
                "_source": {
                    "engine": "faiss",
                    "space_type": "l2",
                    "description": "My model",
                    "model_id": "model1",
                    "state": "failed",
                    "dimension": 2,
                    "timestamp": "2024-02-22T21:57:12.848772887Z"
                }
            }
        ]
    }
}
```
2. Using POST


`https://localhost:9200/_plugins/_knn/models/_search`

same result as above. 

3. Search with query in body working fine.
4. Tested that all below search query params are working for this API.

analyzer,analyze_wildcard,ccs_minimize_roundtrips,default_operator,df,explain,stored_fields,docvalue_fields,from,ignore_unavailable,ignore_throttled,allow_no_indices,expand_wildcards,lenient,preference,q,routing,scroll,search_type,size,sort,_source,_source_excludes,_source_includes,terminate_after,stats,suggest_field,suggest_mode,suggest_size,suggest_text,timeout,track_scores,track_total_hits,allow_partial_search_results,typed_keys,version,seq_no_primary_term,request_cache,batched_reduce_size,max_concurrent_shard_requests,pre_filter_shard_size,rest_total_hits_as_int

