
##multiply the arrays u and v element-wise and compute their dot product

u = np.arange(0, 5, .5)
v = np.arange(5, 10, .5)
elementWise = u * v
dotProduct = u.dot(v)

from numpy.linalg import inv

A = np.matrix([[1,2,3,4],[5,6,7,8]]

## Multiply A by A transpose
AAt = A * np.matrix.transpose(A)

## Invert AAt with np.linalg.inv()
AAtInv = np.linalg.inv(AAt)

## The last three elements of features
lastThree = features[-3:]

## Create a DenseVector consisting of the values [3.0, 4.0, 5.0]
myDenseVector = DenseVector([3.0, 4.0, 5.0])
## Calculate the dot product between the two vectors.
denseDotProduct = myDenseVector.dot(numpyVector)
