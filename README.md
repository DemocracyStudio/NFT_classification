# NFT classification with visual feature extraction
This repository contains all the information, code and data about the NFT classification with visual feature extraction by computer vision, started as a group project at the Machine Learning degree of [opencampus.sh](https://opencampus.sh). Team mates are: Lennert Jessen, Julien Carbonnell.

### Project Description:
The recent increase of digital art and digitalization of historic artworks hosted in museums, combined with the improvement of machine learning techniques to train computers on achieving performative visual recognition tasks, allows us to envision large scale art classifiers for different purposes. The detection of authentic and fake paintings, the recommendation of similar artworks from a given one, As for our concern, we will try to use computer vision to identify what makes an NFT valuable or not. 

As a nascent market of $50B capitalization, NFT sales remain highly volatile and hardly predictable. We are wondering if NFTs values forecasting could benefit from a visual feature classification performed by artificial intelligence. We will use Convolutional Neural Networks pre-trained both on real-world images classification and on art classification. As the enhancement of the earlier improve the laster, we are expecting that NFT classification will benefit from transfer learning of previously trained models. However, our purpose will not be to detect the belonging on an NFT to a collection or an artist, but how much it would be valued on the market. 

A pitch deck is available [here](https://docs.google.com/presentation/d/1K-IZk7SBP9A4UM-96AAbhkHJ-ttUYWxnUfznlGXn_rY/edit?usp=sharing). 

### Datasets:
Our model aims to classify NFTs using visual features, which haven't been done so far, or at least no publication nor pre-trained model could be found on this topic. We will first train our model on existing NFT datasets publicly shared on Kaggle, before deploying it on a marketplace API. The following datasets of NFT images have been shared publicly on Kaggle:

Images data
- [Witches](https://www.kaggle.com/datasets/harrywang/crypto-coven) collected on opensea.com on April 22, 2022.
- [CryptoPunks](https://www.kaggle.com/datasets/tunguz/cryptopunks) collected on [larvalabs.com](https://larvalabs.com/cryptopunks) on October 8, 2021.
- [Bored Apes](https://www.kaggle.com/datasets/stanleyjzheng/bored-apes-yacht-club) collected on opensea.com (https://opensea.com) on July 14, 2021.
- [NFT art collection](https://www.kaggle.com/datasets/vepnar/nft-art-dataset) collected on [nftshowroom.com](https://nftshowroom.com/) on March 29, 2021.

### Protocol:
- Balance samples datasets in order to have same number of images for each collection. To avoid bias, select samples randomly within each collection. 
- Similarly, each sample images should be encoded in the same definition. We will reduce the size of thje larger images to the size of the smaller ones.
- Concatenate image data with last price of sale. 
- Ideas from the meeting on 27.05.22:
- Build a CNN to classify images. Let the computer pick the classification rather than giving a collections a priori.
- Train the CNN with the apes dataset and then test it on the other collections
- Maybe use transfer learning to train on the other collections
- We can use the AlexNet architecture
- Meeting on 30.06.22:
- Not use AlexNet since it needs labels. We will look for other models like k-means.

### Timeline:
- 3.6. Decide on a model. Finish data preparation.
- 10.6. Start building the model

### Literature:
2021
- [Compare the performance of the models in art classification](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0248414)
- [On Label-Efficient Computer Vision: Building Fast and Effective Few-Shot Image Classifiers](https://open.library.ubc.ca/soa/cIRcle/collections/ubctheses/24/items/1.0402554)
- [CLIP-Art: Contrastive Pre-training for Fine-Grained Art Classification](https://paperswithcode.com/paper/clip-art-contrastive-pre-training-for-fine-1)

2020
- [EfficientDet: Scalable and Efficient Object Detection](https://paperswithcode.com/paper/efficientdet-scalable-and-efficient-object)
- [Compounding the Performance Improvements of Assembled Techniques in a Convolutional Neural Network](https://paperswithcode.com/paper/compounding-the-performance-improvements-of)
- [Improved Few-Shot Visual Classification](https://paperswithcode.com/paper/improved-few-shot-visual-classification)

2015
- [Large-scale Classification of Fine-Art Paintings: Learning The Right Metric on The Right Feature](https://paperswithcode.com/paper/large-scale-classification-of-fine-art)

A literature review is available [here](https://docs.google.com/presentation/d/1C71zY-cyWRJ5eGu-7kWDVJnMXtFdfASyUyzi9TH5iU4/edit?usp=sharing).
