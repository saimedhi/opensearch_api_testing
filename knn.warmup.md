1. index is mandatory

`GET https://localhost:9200/_plugins/_knn/warmup`

{
    "error": "no handler found for uri [/_plugins/_knn/warmup] and method [GET]"
}

2. With index

`GET https://localhost:9200/_plugins/_knn/warmup/my-index-knn1`
{
    "_shards": {
        "total": 2,
        "successful": 1,
        "failed": 0
    }
}
