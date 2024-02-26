# Instacart Consumer Segmentation

## Objective :
The goal of this project is to classify instacart consumer based on RFM analysis and their purchasing behaviour.

### 1 What is RFM Analysis ? 
RFM stands for Recency, Frequency, and Monetary value, each corresponding to some key customer trait. These RFM metrics are important indicators of a customer’s behavior because frequency and monetary value affects a customer’s lifetime value, and recency affects retention, a measure of engagement.

* the more recent the purchase, the more responsive the customer is to promotions
* the more frequently the customer buys, the more engaged and satisfied they are
* monetary value differentiates heavy spenders from low-value purchasers

<img width="734" alt="Screenshot 2024-02-26 at 11 23 31 AM" src="https://github.com/anasq30/consumer_segmentation/assets/108400927/7a045a87-b346-44b0-9faf-0b0d9e3deabb">


### Steps for Segmentation using K-Means Clustering.

* Feature engineered the data to give it a RFM structure and performed log transform to remove skewness from the data.
* Calculated **silhouette score** and visualize the same by plotting a elbow plot to determine the number of clusters.

### Silhouette score
Silhouette score compares the distance between any given datapoint and the center of its assigned cluster to the distance between that datapoint and the centers of other clusters.  we want this value to be low, meaning our clusters are tighter and also farther from each other in the vector space.

<img width="562" alt="Screenshot 2024-02-26 at 11 32 52 AM" src="https://github.com/anasq30/consumer_segmentation/assets/108400927/a4e04708-741f-4f84-85e1-e9b2b557739b">

As we can see the lowest value of silhouette score is **0.453** which determines that there are 3 types of consumers. 

<img width="381" alt="Screenshot 2024-02-26 at 11 39 06 AM" src="https://github.com/anasq30/consumer_segmentation/assets/108400927/ba471ff8-1efe-4d95-86bb-4493e8da6694">
**Elbow Plot**


## Conclusion :

 * Determined that cluster 0 are most frequent consumers, cluster 1 are occasional consumers and cluster 2 are rare consumers. It implies Instacart should develop marketing strategies to attract consumers belonging to cluster 2 & 3.



