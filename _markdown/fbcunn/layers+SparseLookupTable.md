

### SparseLookupTable.lua ###

Copyright 2004-present Facebook. All Rights Reserved.

<a name="fbcunn.SparseLookupTable.dok"></a>


## fbcunn.SparseLookupTable ##


Sparse lookup table. Similar to the regular LookupTable.lua module, 
except for the following differences:

1. The outputs are in sparse format.
2. The inputs are pairs (i,w), so the output corresponding to index i
is scaled by w.
3. The indices are fixed, i.e. during a parameter update only the nonzero 
coefficents are updated. This is to avoid having to create new indices, 
which is expensive and may result in the weights no longer being sparse.


<a class="entityLink" href="https://github.com/facebook/fbcunn/blob/d84530ee7c84c5651f674d115a45e3ab8cbb39d2/layers/SparseLookupTable.lua#L23">[src]</a>
<a name="fbcunn.SparseLookupTable"></a>


### fbcunn.SparseLookupTable(indices,sparseGrad) ###


Parameters:
* `indices` is a 2D matrix of indices which will be nonzero.
* `sparseGrad` indicates whether incoming gradients will be sparse or dense.



#### Undocumented methods ####

<a name="fbcunn.SparseLookupTable:reset"></a>
 * `fbcunn.SparseLookupTable:reset(stdv)`
<a name="fbcunn.SparseLookupTable:updateOutput"></a>
 * `fbcunn.SparseLookupTable:updateOutput(input)`
<a name="fbcunn.SparseLookupTable:accUpdateGradParameters"></a>
 * `fbcunn.SparseLookupTable:accUpdateGradParameters(input, gradOutput,lr)`
