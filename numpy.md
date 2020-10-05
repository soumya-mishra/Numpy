``import numpy as np 
`
np.arange(15).reshape(3, 5)
x = np.array([[1, 2, 3], [4, 5, 6]], np.int32)
x.dtype
np.ndarray(shape=(2,2), dtype=float, order='F')
y = np.zeros([2,2])
a.ndim
a.shape
a.size
a.dtype
a.itemsize
a.data
np.empty( (2,3) ) 
np.ones( (2,3,4), dtype=np.int16 )  
np.linspace( 0, 2, 9 )  -- 9 no from 0 to 2
a.sum()
a.min() | b.min(axis=1) 
a.max()
b.sum(axis=0) 
b.cumsum(axis=1)  -  cumulative sum in each row

np.exp(B)
np.sqrt(B)
np.add(B, C)

a[2:5]
a[:6:2]
a[ : :-1] 
a = array([[1, 2, 3],
       	   [4, 5, 6]])

Ooutput: array([[4, 5, 6],
       		[1, 2, 3]])
x.flatten()  -->array([1, 2, 3, 4, 5, 6])

for element in b.flat:
	print(element)

a.ravel()  # returns the array, flattened
a.T -  transpose

reshape() - returns argument with modified shape
resize() - modifies the array itself

np.vstack((a,b))
np.hstack((a,b))

np.column_stack
np.row_stack

np.hsplit(a,3)

a.view() - shallow copy
a.copy()  -  deep copy

np.eye(2, dtype=int) -  1 in diagonal
array([[1, 0],
       [0, 1]])

np.logspace(2.0, 3.0, num=4)  - no in Log scale
array([ 100.        ,  215.443469  ,  464.15888336, 1000.        ])


x = [[0, 1, 2],
       [3, 4, 5]]

np.zeros_like(x)
array([[0, 0, 0],
       [0, 0, 0]]

conversion:
np.astype(int)

np.squeeze - Remove an axis from a
np.swapaxes -  
np.take,
a = [4, 3, 5, 7, 6, 8]
indices = [0, 1, 4]
np.take(a, indices)
array([4, 3, 6])

np.all()
np.any()
np.where()
np.where(x < y, x, 10 + y)

np.argmax(),
np.argmin(),
np.argsort()

np.ptp() -  peak to peak : Range of values (maximum - minimum) along an axis.
x = np.array([[4, 9, 2, 10],
              [6, 9, 7, 12]])
np.ptp(x) # 12-2 =10
np.ptp(x,axis=1)
array([8, 6])

np.sort()

Basic Statistics:
cov, mean, std, var

np.linalg.*
np.linalg.svd()

