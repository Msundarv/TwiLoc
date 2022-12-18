# TwiLoc - Location Prediction Using Tweets

TwiLoc investigates the feasibility of geographically locating Twitter users based solely on tweet content. We are trying to locate a user using their tweet content by understanding the dialect differences across geographies through deep learning techniques. We are not using any other external information to locate the user. This project provides an approach to augment existing systems that locate users.

<p align="center"> <img src="http://msundarv.com/images/twitterloc/1.jpg"  width="25%" height="25%" > </p>

## Prerequisites

Requires Python 3.x.

Here's is the list of libraries required for this project

- [NumPy](https://www.numpy.org/)
- [Pandas](https://pandas.pydata.org/)
- [NLTK](https://www.nltk.org/)
- [Scikit-learn](https://scikit-learn.org/)
- [Keras](https://keras.io/)

[GloVe](https://nlp.stanford.edu/projects/glove/) is used for obtaining vector representations for words.

## Dataset

- [GeoText](http://www.cs.cmu.edu/~ark/GeoText/) - Geo-tagged Microblog Corpus is the primary dataset for TwiLoc. All the results and hyperparameter tunings are based on this dataset.

- Accuracy can be enhanced further by using massive datasets like [UTGeo2011](http://www.cs.utexas.edu/~roller/research/kd/corpus/README.txt) can also be used to train.

Reverse geocoding can be done using services provided by [MapQuest]( http://www.mapquest.com).

## Pre-trained models

| Model        | Accuracy (%)          | 
| ------------- |:-------------:|
| [CNN](http://msundarv.com/docs/TwiLoc/Pre-trained%20Models/cnn1d-best.hdf5)      | 57.43 |
| [GRU](http://msundarv.com/docs/TwiLoc/Pre-trained%20Models/gru-best.hdf5)      | 56.35      | 
| [LSTM](http://msundarv.com/docs/TwiLoc/Pre-trained%20Models/lstm-best.hdf5) | 55.54      | 
| [MLP](http://msundarv.com/docs/TwiLoc/Pre-trained%20Models/mlp-best.hdf5) | 50.59      | 


Note: Please read the [report](https://github.com/Msundarv/TwiLoc/blob/master/Report.pdf) for more detailed information regarding the experiment's result.

## References

- Eisenstein J., O'Connor B., Smith N A., Xing E P. 2010. [A Latent Variable Model for Geographic Lexical Variation](https://dl.acm.org/citation.cfm?id=1870782). In Proceedings of the Conference on Empirical Methods in Natural Language Processing.
- Liu J., Inkpen D. 2015. [Estimating User Location in Social Media with Stacked Denoising Autoencoders](https://www.researchgate.net/publication/301405397_Estimating_User_Location_in_Social_Media_with_Stacked_Denoising_Auto-encoders). Proceedings of the 1st Workshop on Vector Space Modeling for Natural Language Processing.
- Yin W., Kann K., Yu M., Hinrich S. 2017. [Comparative Study of CNN and RNN for Natural Language Processing](https://arxiv.org/abs/1702.01923). arXiv:1702.01923.

## Authors

- [Sundar V](http://msundarv.com/)
- [Gogula Krishnan](https://sg.linkedin.com/in/gogulak)
