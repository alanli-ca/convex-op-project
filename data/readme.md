{\rtf1\ansi\ansicpg1252\cocoartf1561\cocoasubrtf200
{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\margl1440\margr1440\vieww10800\viewh8400\viewkind0
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0

\f0\fs24 \cf0 FOR TEST4, only 20 graphs per class are used\
\
probability_tests = \{\
    "test1": [0.1, 0.9],\
    "test2": [0.3, 0.7],\
    "test3": [0.4, 0.6],\
    "test4": [0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]\
\}\
\
graph_types = \{\
    "fast_gnp_random_graph": 1,\
    "watts_strogatz_graph": 2, # rewires existing edge with prob p\
    "newman_watts_strogatz_graph": 3, # adds new edge with prob p\
    "connected_watts_strogatz_graph": 4 # rewires existing edge with prob p, but ensures connected graph\
\}\
\
graph_parameters = \{\
    "graph_type": graph_types["connected_watts_strogatz_graph"],\
    "graphs_per_class": 100,\
    "num_nodes": 50, #569 in the Nature study\
    "knn": 6, # used in watts-strogatz graphs\
    "graph_edge_width": 0.1\
\}}