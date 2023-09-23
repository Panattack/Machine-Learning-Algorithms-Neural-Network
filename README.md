# Machine-Learning-Algorithms-Neural-Network

## Part A (60%)
Implement in Java or C++ or Python (or other language that
the tutors will allow you) two or three (depending on
whether your team has two or three members) by the following learning algorithms so that they can be used to rank texts
into two (unrelated) categories (e.g. positive/negative opinion)

• Naïve Bayes classifier, multivariate Bernoulli form or
  polynomial form.

• ID3, optionally with sawing or early extension termination
  of every tree.

• Random Forest using ID3 or its variant (eg where
  will produce trees that will not exceed a maximum depth,
  which will be given as a hyper-parameter) to produce the trees.

Each text should be represented by a vector of properties with values
0 or 1, which will indicate which vocabulary words the text contains.
The vocabulary should include the m most frequent words of
of training data, first skipping the n most frequent and the k most
rare words of the training data, where m, n, k will be hyperparameters. Optionally you can add a selection of properties
through information gain calculation (or through other means) to
naive Bayes classifier. Others
algorithms already incorporate feature selection methods.

Demonstrate the learning capabilities of your implementations using
the 'Large Movie Review Dataset', which is known
and as "IMDB dataset" (see https://ai.stanford.edu/~amaas/data/sentiment/,
https://keras.io/api/datasets/imdb/). You should include in the report
your results of the experiments you will perform with your implementations
in this data set, showing (at least):
• learning curves and corresponding tables showing the
  percentage of correctness (accuracy) in the training data (training 
  data, which have been used each time) and control (test data)
  function of the number of training examples that
  are used in each repetition of the experiment
• corresponding curves and tables with accuracy results
  (precision), recall, F1 for one of the two categories,
  as a function of the number of training examples.

## Part B' (20%)
Compare the performance of your implementations with theirs
performance of other available implementations (e.g. Weka or Scikit-learn)
of the same learning algorithms that you implemented in part A' or others
learning algorithms (e.g. MLPs implementations of Scikit-learn),
constructing the same curves and tables as in Part A'. I will
need you to compare with at least two or three available implementations of learning algorithms.
You should use the same representations of the texts as in
Part A (feature vectors with values ​​of 0 or 1 that will indicate which words
of vocabulary appear in the text or not, with the same vocabulary as in
Part A'). Here, too, you can use ready-made implementations of text preprocessing and property selection, as well as ready-made
libraries for constructing curve charts.

## Part C' (20%)
Compare the results of Parts A' and B' with the
results of a rolling window MLP and/or an RNN, which will
implement in Tensorflow/Keras, representing the words with nests
word embeddings. Construct the same curves here as well
tables, as in parts A and B. Also construct curves that to
show the change in error (loss) in the training examples
and growth, depending on the number of seasons.
