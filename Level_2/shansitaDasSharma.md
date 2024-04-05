# 🎻 Music Genre Clustering

> Level 2

### 🧮 Algorithm / Model Architecture

I decided to take a twist on the standard K-Means procedure by first reducing the dimensionality of data using a Autoencoder then performing clustering on the compressed representation. The idea was to combat the issue that clustering faces through the [curse of dimensionality](https://en.wikipedia.org/wiki/Curse_of_dimensionality), wherein it's performance suffers at higher dimensional of inputs.

By first training an [autoencoder](https://www.tensorflow.org/tutorials/generative/autoencoder), I reduced the dimensionality from 8 (8 primary audio features defined previously) to 5 (selected through manual trials). The encoder compresses the data to only retain the vital features. After this, K-Means performs clustering based on this compressed data to assign classes to each of the tracks.

This approach is effective for identifying patterns and similarities within large datasets, as it is capable of simplifying the information while preserving the key characteristics of the data, enabling more efficient clustering and analysis.

Here is a figure from a paper that also proposes a similar procedure that I found afterwards. While the paper defines a deeper neural network, I choose to use fewer layers to prevent overfitting.

![Model architecture example](../assets/model_architecture.png)  
_"Lu, Si, and Ruisi Li. "DAC: Deep Autoencoder-based Clustering, a General Deep Learning Framework of Representation Learning." Portland State University."_

### 📚 Resources Utilized

> _"Lu, Si, and Ruisi Li. "DAC: Deep Autoencoder-based Clustering, a General Deep Learning Framework of Representation Learning." Portland State University." [\[link\]](https://arxiv.org/pdf/2102.07472.pdf)_
>
> FMA Dataset [\[github\]](https://github.com/mdeff/fma/tree/master?tab=readme-ov-file)
>
> Other genre clustering projects: [\[1\]](https://www.kaggle.com/code/shabanamir/unsupervised-ml-project-music-clustering) [\[2\]](https://medium.com/latinxinai/discovering-descriptive-music-genres-using-k-means-clustering-d19bdea5e443)

### Additional information

Other models I tried using before settling on the Autoencoder-K Means architecture are the following:

- DBSCAN
- Autoencoder-DBSCAN
- K Means
- CNN

### 🎁 Level 2 bonus tasks attempted:

- [x] using Python
- [x] detailed explanations on why you chose your algorithm
- [x] code comments (up to the grader's discretion)
