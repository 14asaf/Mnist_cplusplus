
MNIST Dataset Loader
========

This is a tiny C++ programm to parse the MNIST Dataset (which is one of the most popular datasets to train neural networks). Just include the "MNIST.h" header file in you're source and look at the example usage in "main.cpp".

About [MNIST](http://yann.lecun.com/exdb/mnist/)
--------

The MNIST database of handwritten digits, has a training set of 60,000 examples, and a test set of 10,000 examples. It is a subset of a larger set available from NIST. The digits have been size-normalized and centered in a fixed-size image (28x28). It is a good database for people who want to try learning techniques and pattern recognition methods on real-world data while spending minimal efforts on preprocessing and formatting.

Interface
--------

Struct MNISTchar
* the std::vector "pixelData" stores the 784 (28x28) pixel color values
* the std::vector "output" stores the expected output (e.g: expected = 5 / output vec = 0,0,0,0,0,1,0,0,0,0)
* the number "label" stores the expected output (handwritten digit) as int

Class MNIST
* The constructor needs the base path to all the MNIST files (requiring them to be in the same dir)
* The public std::vector "trainingData" holds the training set of 60.000 handwritten digits
* The public std::vector "testData" holds the testing set of 10.000 handwritten digits
* The public function "testPrintout" takes a start + end position and prints out all the trainingData digits in bewteen
