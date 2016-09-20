
<h1> MNIST Dataset Loader C++ </h1><br>

<b> About MNIST: </b> <br>
http://yann.lecun.com/exdb/mnist/ <br>
Yann LeCun (Courant Institute, NYU), Corinna Cortes (Google Labs, New York) <br>
and Christopher J.C. Burges (Microsoft Research, Redmond) <br>
<br>
The MNIST database of handwritten digits, has a training set of 60,000 examples, <br>
and a test set of 10,000 examples. It is a subset of a larger set available from NIST. <br>
The digits have been size-normalized and centered in a fixed-size image (28x28) <br>
<br>
It is a good database for people who want to try learning techniques <br>
and pattern recognition methods on real-world data while spending minimal <br> 
efforts on preprocessing and formatting. <br>

<b> About the Loader </b><br>
This is a short C++ programm to parse the MNIST Dataset. <br>
(which is one of the most popular datasets to train neural networks)

- All four MNIST data files are needed (training images + labels / test images + labels)
- Path to those files is passed in the constructor
- The class has two containers (trainingData & testData) that hold the 60.000 & 10.000 digits
- The pixel data of each digit is stored in a vector (784 doubles, one for each pixel)
- Printout function, to verify that the digits + labels are parsed correctly
