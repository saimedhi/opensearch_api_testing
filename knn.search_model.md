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


