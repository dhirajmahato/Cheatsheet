## NumPy - Numerical Python
NumPy enables fast computation in Python, the underlying implementation is in C hence it's blazing fast. The Key feature of NumPy is the **ndarray** object. The data type should be homogenous, that is the array should contain elements of **single data type.**

#### Array
```
arr = np.array([1, 2, 3, 4])
arr2d = np.array([[1, 2, 3], [4, 5, 6]])
```

#### Array Properties
```
arr.shape      # (4,)  → 1D array with 4 elements
arr2d.shape    # (2,3) → 2 rows, 3 columns

arr.dtype      # data type (e.g., int64, float64)
```

#### Useful functions
```
np.zeros((2,3))      # 2x3 matrix of zeros
np.ones((2,2))       # 2x2 matrix of ones
np.arange(0,10,2)    # [0 2 4 6 8]
np.linspace(0,1,5)   # [0.   0.25 0.5 0.75 1.0]
np.eye(3)            # Identity matrix (3x3)
```

#### Operations - imp - noloop need as numpy array is vectorised
```
arr = np.array([1, 2, 3])
arr + 10          # [11, 12, 13]
arr * 2           # [2, 4, 6]
arr ** 2          # [1, 4, 9]
np.sqrt(arr)      # [1.0, 1.414, 1.732]
```
#### indexing and silicing
```
arr2d = np.array([[10,20,30], [40,50,60]])

arr2d[0,1]      # 20 (row 0, column 1)
arr2d[:,1]      # [20,50] (all rows, column 1)
arr2d[1,:]      # [40,50,60] (row 1, all columns)
```

#### Aggregations
```
arr.sum()         # sum of all elements
arr.mean()        # average
arr.max()         # maximum
arr.min()         # minimum
arr.std()         # standard deviation
```

#### Random
```
arr = np.arange(1,7)     # [1,2,3,4,5,6]
arr.reshape(2,3)         # [[1,2,3],[4,5,6]]
```















src: https://nbviewer.org/github/maykulkarni/Machine-Learning-Notebooks/blob/master/00.%20NumPy%20Basics/1.%20NumPy%20Basics.ipynb
