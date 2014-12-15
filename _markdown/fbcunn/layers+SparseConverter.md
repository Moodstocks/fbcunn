<a name="fbcunn.SparseConverter.dok"></a>


## fbcunn.SparseConverter ##

Copyright 2004-present Facebook. All Rights Reserved.

<a class="entityLink" href="https://github.com/facebook/fbcunn/blob/d84530ee7c84c5651f674d115a45e3ab8cbb39d2/layers/SparseConverter.lua#L14">[src]</a>
<a name="fbcunn.SparseConverter"></a>


### fbcunn.SparseConverter(fconv,bconv,dim,thresh) ###


Parameters:
* `fconv` - conversion to perform in fprop, either 'StoD','DtoS' or nil
* `bconv` - conversion to perform in bprop, either 'StoD','DtoS' or nil
* `dim` - number of dimensions
* `thresh` - threshold for sparsifying (0 by default)



#### Undocumented methods ####

<a name="fbcunn.SparseConverter:updateOutput"></a>
 * `fbcunn.SparseConverter:updateOutput(input)`
<a name="fbcunn.SparseConverter:updateGradInput"></a>
 * `fbcunn.SparseConverter:updateGradInput(input, gradOutput)`
