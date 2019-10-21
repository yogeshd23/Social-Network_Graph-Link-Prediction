# Social-Network_Graph-Link-Prediction

Problem statement:
Given a directed social graph, have to predict missing links to recommend users (Link Prediction in graph)<br>

Data Overview<br>
Taken data from facebook's recruting challenge on kaggle https://www.kaggle.com/c/FacebookRecruiting
data contains two columns source and destination eac edge in graph<br>

- Data columns (total 2 columns):  <br>
- source_node         int64  <br>
- destination_node    int64  <br>
Mapping the problem into supervised learning problem:<br>
Generated training samples of good and bad links from given directed graph and for each link got some features like no of followers, is he followed back, page rank, katz score, adar index, some svd fetures of adj matrix, some weight features etc. and trained ml model based on these features to predict link.<br>

Some reference papers and videos :<br>
https://www.cs.cornell.edu/home/kleinber/link-pred.pdf<br>
https://www3.nd.edu/~dial/publications/lichtenwalter2010new.pdf<br>
https://kaggle2.blob.core.windows.net/forum-message-attachments/2594/supervised_link_prediction.pdf<br>
https://www.youtube.com/watch?v=2M77Hgy17cg<br>


Business objectives and constraints:<br>
No low-latency requirement.<br>
Probability of prediction is useful to recommend ighest probability links<br>
Performance metric for supervised learning:<br>
Both precision and recall is important so F1 score is good choice<br>
Confusion matrix<br>
