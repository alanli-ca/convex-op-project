FOR TEST4, only 20 graphs per class are used

probability_tests:
"test1": [0.1, 0.9]
"test2": [0.3, 0.7]
"test3": [0.4, 0.6]
"test4": [0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]

graph_types:
"fast_gnp_random_graph": 1
"watts_strogatz_graph": 2
"newman_watts_strogatz_graph": 3
"connected_watts_strogatz_graph": 4

graph_parameters
"graph_type": graph_types["connected_watts_strogatz_graph"]
"graphs_per_class": 100
"num_nodes": 50
"knn": 6
"graph_edge_width": 0.1