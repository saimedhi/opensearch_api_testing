1. `GET https://localhost:9200/_plugins/_knn/stats`


{
    "_nodes": {
        "total": 1,
        "successful": 1,
        "failed": 0
    },
    "cluster_name": "docker-cluster",
    "circuit_breaker_triggered": false,
    "model_index_status": null,
    "nodes": {
        "k9AHEEapRhK_CrKyE4cm-Q": {
            "graph_memory_usage_percentage": 0.0,
            "graph_query_requests": 0,
            "graph_memory_usage": 0,
            "cache_capacity_reached": false,
            "load_success_count": 0,
            "training_memory_usage": 0,
            "indices_in_cache": {},
            "script_query_errors": 0,
            "hit_count": 0,
            "knn_query_requests": 0,
            "total_load_time": 0,
            "miss_count": 0,
            "knn_query_with_filter_requests": 0,
            "training_memory_usage_percentage": 0.0,
            "lucene_initialized": false,
            "graph_index_requests": 0,
            "faiss_initialized": false,
            "load_exception_count": 0,
            "training_errors": 0,
            "eviction_count": 0,
            "nmslib_initialized": false,
            "script_compilations": 0,
            "script_query_requests": 0,
            "graph_stats": {
                "merge": {
                    "current": 0,
                    "total": 0,
                    "total_time_in_millis": 0,
                    "current_docs": 0,
                    "total_docs": 0,
                    "total_size_in_bytes": 0,
                    "current_size_in_bytes": 0
                },
                "refresh": {
                    "total": 0,
                    "total_time_in_millis": 0
                }
            },
            "graph_query_errors": 0,
            "indexing_from_model_degraded": false,
            "graph_index_errors": 0,
            "training_requests": 0,
            "script_compilation_errors": 0
        }
    }
}


2. With timeout query param `GET https://localhost:9200/_plugins/_knn/stats?timeout=60ms`


{
    "_nodes": {
        "total": 1,
        "successful": 1,
        "failed": 0
    },
    "cluster_name": "docker-cluster",
    "circuit_breaker_triggered": false,
    "model_index_status": null,
    "nodes": {
        "k9AHEEapRhK_CrKyE4cm-Q": {
            "graph_memory_usage_percentage": 0.0,
            "graph_query_requests": 0,
            "graph_memory_usage": 0,
            "cache_capacity_reached": false,
            "load_success_count": 0,
            "training_memory_usage": 0,
            "indices_in_cache": {},
            "script_query_errors": 0,
            "hit_count": 0,
            "knn_query_requests": 0,
            "total_load_time": 0,
            "miss_count": 0,
            "knn_query_with_filter_requests": 0,
            "training_memory_usage_percentage": 0.0,
            "lucene_initialized": false,
            "graph_index_requests": 0,
            "faiss_initialized": false,
            "load_exception_count": 0,
            "training_errors": 0,
            "eviction_count": 0,
            "nmslib_initialized": false,
            "script_compilations": 0,
            "script_query_requests": 0,
            "graph_stats": {
                "merge": {
                    "current": 0,
                    "total": 0,
                    "total_time_in_millis": 0,
                    "current_docs": 0,
                    "total_docs": 0,
                    "total_size_in_bytes": 0,
                    "current_size_in_bytes": 0
                },
                "refresh": {
                    "total": 0,
                    "total_time_in_millis": 0
                }
            },
            "graph_query_errors": 0,
            "indexing_from_model_degraded": false,
            "graph_index_errors": 0,
            "training_requests": 0,
            "script_compilation_errors": 0
        }
    }
}


3. with node-id path param `GET https://localhost:9200/_plugins/_knn/k9AHEEapRhK_CrKyE4cm-Q/stats?timeout=60ms`


{
    "_nodes": {
        "total": 1,
        "successful": 1,
        "failed": 0
    },
    "cluster_name": "docker-cluster",
    "circuit_breaker_triggered": false,
    "model_index_status": null,
    "nodes": {
        "k9AHEEapRhK_CrKyE4cm-Q": {
            "graph_memory_usage_percentage": 0.0,
            "graph_query_requests": 0,
            "graph_memory_usage": 0,
            "cache_capacity_reached": false,
            "load_success_count": 0,
            "training_memory_usage": 0,
            "indices_in_cache": {},
            "script_query_errors": 0,
            "hit_count": 0,
            "knn_query_requests": 0,
            "total_load_time": 0,
            "miss_count": 0,
            "knn_query_with_filter_requests": 0,
            "training_memory_usage_percentage": 0.0,
            "lucene_initialized": false,
            "graph_index_requests": 0,
            "faiss_initialized": false,
            "load_exception_count": 0,
            "training_errors": 0,
            "eviction_count": 0,
            "nmslib_initialized": false,
            "script_compilations": 0,
            "script_query_requests": 0,
            "graph_stats": {
                "merge": {
                    "current": 0,
                    "total": 0,
                    "total_time_in_millis": 0,
                    "current_docs": 0,
                    "total_docs": 0,
                    "total_size_in_bytes": 0,
                    "current_size_in_bytes": 0
                },
                "refresh": {
                    "total": 0,
                    "total_time_in_millis": 0
                }
            },
            "graph_query_errors": 0,
            "indexing_from_model_degraded": false,
            "graph_index_errors": 0,
            "training_requests": 0,
            "script_compilation_errors": 0
        }
    }
}

4. with node-id, stat path params
`GET https://localhost:9200/_plugins/_knn/k9AHEEapRhK_CrKyE4cm-Q/stats/cache_capacity_reached,load_success_count,knn_query_requests?timeout=60ms`


{
    "_nodes": {
        "total": 1,
        "successful": 1,
        "failed": 0
    },
    "cluster_name": "docker-cluster",
    "nodes": {
        "k9AHEEapRhK_CrKyE4cm-Q": {
            "cache_capacity_reached": false,
            "load_success_count": 0,
            "knn_query_requests": 0
        }
    }
}

5.with stat path param
`GET https://localhost:9200/_plugins/_knn/stats/cache_capacity_reached,load_success_count,knn_query_requests?timeout=60ms`

{
    "_nodes": {
        "total": 1,
        "successful": 1,
        "failed": 0
    },
    "cluster_name": "docker-cluster",
    "nodes": {
        "k9AHEEapRhK_CrKyE4cm-Q": {
            "cache_capacity_reached": false,
            "load_success_count": 0,
            "knn_query_requests": 0
        }
    }
}




