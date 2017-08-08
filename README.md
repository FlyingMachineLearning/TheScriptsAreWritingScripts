# TheScriptsAreWritingScripts
Project 3 in the Udacity Intro to Deep Learning Nanodegree

There's weird issue happening where you can't use more than one RNN layer in Tensorflow. The workaround listed on doesn't Github work. 
https://github.com/tensorflow/tensorflow/issues/8191
There's another issue with MultiRNNCell that throws an error but that's listed in the Exception:
MultiRNNCell([BasicLSTMCell(...)] * num_layers), change to: MultiRNNCell([BasicLSTMCell(...) for _ in range(num_layers)])
