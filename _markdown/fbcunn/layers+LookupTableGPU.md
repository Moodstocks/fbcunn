

### LookupTableGPU.lua ###

Copyright 2004-present Facebook. All Rights Reserved.
Author: Michael Mathieu <myrhev@fb.com>

<a name="fbcunn.LookupTableGPU.dok"></a>


## fbcunn.LookupTableGPU ##


Fast lookup table, supporting both CPU and GPU modes.


<a class="entityLink" href="https://github.com/facebook/fbcunn/blob/d84530ee7c84c5651f674d115a45e3ab8cbb39d2/layers/LookupTableGPU.lua#L19">[src]</a>
<a name="fbcunn.LookupTableGPU"></a>


### fbcunn.LookupTableGPU(nInput, nOutput, featuresInDim2) ###


If `featuresInDim2` is `true`, an input of dimension `batchSize` ${\times}$ `N` will produce an output of size `batchSize` ${\times}$ `nOutput`
${\times}$ `N`. If it is set to `false` (default) it will produce an output
of size `batchSize` ${\times}$ `N` ${\times}$ `nOutput`.


<a class="entityLink" href="https://github.com/facebook/fbcunn/blob/d84530ee7c84c5651f674d115a45e3ab8cbb39d2/layers/LookupTableGPU.lua#L42">[src]</a>
<a name="fbcunn.LookupTableGPU:updateOutput"></a>


### fbcunn.LookupTableGPU:updateOutput(input) ###

input should be a 1d (size N) or 2d (size batchSize x N)
tensor of byte or long on CPU, cudaTensor on GPU.
It contains the indices of the lookup.


#### Undocumented methods ####

<a name="fbcunn.LookupTableGPU:reset"></a>
 * `fbcunn.LookupTableGPU:reset(stdv)`
<a name="fbcunn.LookupTableGPU:parameters"></a>
 * `fbcunn.LookupTableGPU:parameters()`
<a name="fbcunn.LookupTableGPU:updateGradInput"></a>
 * `fbcunn.LookupTableGPU:updateGradInput(input, gradOutput)`
<a name="fbcunn.LookupTableGPU:accGradParameters"></a>
 * `fbcunn.LookupTableGPU:accGradParameters(input, gradOutput, scale)`
