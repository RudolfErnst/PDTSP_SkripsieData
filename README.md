# PDTSP_SkripsieData
Datasets for PDTSP used in project

# 5 different datasets for 5, 29, 63, 155, 250 customer requests
# Each dataset has the pick-up node as unequal rows/columns and associated drop-off node as equal rows/columns
# Last node is the starting/end node (depot)

# If the text file is not in a matrix form, it is necessary to transform textfile into a x * x matrix where x is the amount of nodes
# Matlab code to transform into distance matrix:

fileID = fopen('filename.txt','r');
formatspec = '%d %f';
sizeCcc = [#ofrequests, inf];

Distances = fscanf(fileID,formatspec,sizeCcc);

# REPLACE filename with textfile name and #ofrequests with the number of requests.
