# Digit Classification with MNIST Dataset

The Modified National Institute of Standards and Technology (MNIST) dataset is a large set of 70,000 images of handwritten digits. This dataset was created by modifying the original NIST’s dataset. The original NIST’s dataset contained digits handwritten by American Census Bureau employees for training while the testing set contained digits written by High School students, this made the dataset inappropriate for Machine Learning. So the dataset was modified such that the training and testing set contained digits written by Census Bureau employees and High School students.

Here I have used MNIST database for handwritten digits and classified numbers from 0 to 9 using **Support Vector Machine(SVM)**.

### About Dataset

The data files [train.csv]() and [test.csv]() contain gray-scale images of hand-drawn digits, from zero through nine.

Each image is 28 pixels in height and 28 pixels in width, for a total of 784 pixels in total. Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel, with higher numbers meaning darker. This pixel-value is an integer between 0 and 255, inclusive.

The training data set, (train.csv), has 785 columns. The first column, called "label", is the digit that was drawn by the user. The rest of the columns contain the pixel-values of the associated image.

Each pixel column in the training set has a name like pixelx, where x is an integer between 0 and 783, inclusive. To locate this pixel on the image, suppose that we have decomposed x as x = i * 28 + j, where i and j are integers between 0 and 27, inclusive. Then pixelx is located on row i and column j of a 28 x 28 matrix, (indexing by zero).

Visually, if we omit the "pixel" prefix, the pixels make up the image like this:
<pre>
000 001 002 003 ... 026 027
028 029 030 031 ... 054 055
056 057 058 059 ... 082 083
 |   |   |   |  ...  |   |
728 729 730 731 ... 754 755
756 757 758 759 ... 782 783 
</pre>

The test data set, (test.csv), is the same as the training set, except that it does not contain the "label" column.
