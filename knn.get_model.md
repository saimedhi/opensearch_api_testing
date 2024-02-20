1. with no model_id (model_id is required)

`GET https://localhost:9200/_plugins/_knn/models`

{
    "error": "no handler found for uri [/_plugins/_knn/models] and method [GET]"
}

2. with model_id 

`GET https://localhost:9200/_plugins/_knn/models/HfitVXrMS2exmCZifhNQ4w`

{
    "model_id": "HfitVXrMS2exmCZifhNQ4w",
    "model_blob": "",
    "state": "failed",
    "timestamp": "2024-02-20T20:30:22.095387634Z",
    "description": "My model",
    "space_type": "l2",
    "dimension": 2,
    "engine": "faiss"
}
