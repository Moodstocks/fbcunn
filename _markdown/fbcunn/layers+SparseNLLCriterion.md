

### SparseNLLCriterion.lua ###

Copyright 2004-present Facebook. All Rights Reserved.
Author: Michael Mathieu <myrhev@fb.com>

<a name="fbcunn.SparseNLLCriterion.dok"></a>


## fbcunn.SparseNLLCriterion ##

Sparse ClassNLL criterion

<a class="entityLink" href="https://github.com/facebook/fbcunn/blob/d84530ee7c84c5651f674d115a45e3ab8cbb39d2/layers/SparseNLLCriterion.lua#L18">[src]</a>
<a name="fbcunn.SparseNLLCriterion"></a>


### fbcunn.SparseNLLCriterion(K) ###


Parameters:
* `K` : number of non-zero elements of the target
* `do`_target_check : checks whether the target is a
   probability vector (default true)
* `sizeAverage` : divides the error by the size of the minibatch


<a class="entityLink" href="https://github.com/facebook/fbcunn/blob/d84530ee7c84c5651f674d115a45e3ab8cbb39d2/layers/SparseNLLCriterion.lua#L38">[src]</a>
<a name="fbcunn.SparseNLLCriterion:updateOutput"></a>


### fbcunn.SparseNLLCriterion:updateOutput(input, target) ###


`target` should be a table containing two tensors :

```
target = {targetP, targetIdx}
```

where `targetP` are the probabilities associated to the indices `targetIdx`
we assume `targetIdx` doesn't have twice the same number in the same sample.



#### Undocumented methods ####

<a name="fbcunn.SparseNLLCriterion:updateGradInput"></a>
 * `fbcunn.SparseNLLCriterion:updateGradInput(input, target)`
