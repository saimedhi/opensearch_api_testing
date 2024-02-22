1. Without model_id

```
 Post https://localhost:9200/_plugins/_knn/models/_train 


  body  {
        "training_index": "my-index",
        "training_field": "my_vector1",
        "dimension": 2,
        "max_training_vector_count": 1200,
        "search_size": 100,
        "description": "My model",
        "method": {
            "name":"ivf",
            "engine":"faiss",
            "space_type": "l2",
            "parameters":{
                "nlist":128,
                "encoder":{
                    "name":"pq",
                    "parameters":{
                        "code_size":8
                    }
                }
            }
        }
    }
```

{
    "model_id": "S56iHcluS1-d1L1_Fw3e9Q"
}

2. Without model_id and with preference query_param working fine.

3.  With model_id

```
 Post https://localhost:9200/_plugins/_knn/models/model1/_train 


  body  {
        "training_index": "my-index",
        "training_field": "my_vector1",
        "dimension": 2,
        "max_training_vector_count": 1200,
        "search_size": 100,
        "description": "My model",
        "method": {
            "name":"ivf",
            "engine":"faiss",
            "space_type": "l2",
            "parameters":{
                "nlist":128,
                "encoder":{
                    "name":"pq",
                    "parameters":{
                        "code_size":8
                    }
                }
            }
        }
    }
```

{
    "model_id": "model1"
}


