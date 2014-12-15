

### HSM.lua ###

Copyright 2004-present Facebook. All Rights Reserved.
Author: Michael Mathieu <myrhev@fb.com>

<a name="fbcunn.HSM.dok"></a>


## fbcunn.HSM ##

Hierarchical soft max with minibatches.

<a class="entityLink" href="https://github.com/facebook/fbcunn/blob/d84530ee7c84c5651f674d115a45e3ab8cbb39d2/layers/HSM.lua#L24">[src]</a>
<a name="fbcunn.HSM"></a>


### fbcunn.HSM(mapping, input_size, unk_index) ###


Parameters:
* `mapping` is a table (or tensor) with `n_classes` elements,
    such that `mapping[i]` is a table with 2 elements.
    * `mapping[i][1]` : index (1-based) of the cluster of class `i`
    * `mapping[i][2]` : index (1-based) of the index within its cluster of class `i`
*  `input_size` is the number of elements of the previous layer
*  `unk_index` is an index that is ignored at test time (not added to the
    loss). It can be disabled by setting it to 0 (not nil).
    It should only be used uring testing (since during training,
    it is not disabled in the backprop (TODO) )


<a class="entityLink" href="https://github.com/facebook/fbcunn/blob/d84530ee7c84c5651f674d115a45e3ab8cbb39d2/layers/HSM.lua#L226">[src]</a>
<a name="fbcunn.HSM:updateGradInput"></a>


### fbcunn.HSM:updateGradInput(input, target) ###

Note: call this function at most once after each call `updateOutput`,
or the output will be wrong (it uses `class_score` and `cluster_score`
as temporary buffers)

<a class="entityLink" href="https://github.com/facebook/fbcunn/blob/d84530ee7c84c5651f674d115a45e3ab8cbb39d2/layers/HSM.lua#L270">[src]</a>
<a name="fbcunn.HSM:accGradParameters"></a>


### fbcunn.HSM:accGradParameters(input, target, scale, direct_update) ###

If `direct_update` is set, the parameters are directly updated (not the
gradients). It means that the gradient tensors (like `cluster_grad_weight`)
are not used. scale must be set to the negative learning rate
(`-learning_rate`). `direct_update` mode is much faster.
Before calling this function you have to call `HSM:updateGradInput` first.


#### Undocumented methods ####

<a name="fbcunn.HSM:clone"></a>
 * `fbcunn.HSM:clone(...)`
<a name="fbcunn.HSM:check_mapping"></a>
 * `fbcunn.HSM:check_mapping(mapping)`
<a name="fbcunn.HSM:get_n_class_in_cluster"></a>
 * `fbcunn.HSM:get_n_class_in_cluster(mapping)`
<a name="fbcunn.HSM:parameters"></a>
 * `fbcunn.HSM:parameters()`
<a name="fbcunn.HSM:getParameters"></a>
 * `fbcunn.HSM:getParameters()`
<a name="fbcunn.HSM:reset"></a>
 * `fbcunn.HSM:reset(weight_stdv, bias_stdv)`
<a name="fbcunn.HSM:updateOutput"></a>
 * `fbcunn.HSM:updateOutput(input, target)`
<a name="fbcunn.HSM:updateOutputCPU"></a>
 * `fbcunn.HSM:updateOutputCPU(input, target)`
<a name="fbcunn.HSM:updateOutputCUDA"></a>
 * `fbcunn.HSM:updateOutputCUDA(input, target)`
<a name="fbcunn.HSM:updateGradInputCPU"></a>
 * `fbcunn.HSM:updateGradInputCPU(input, target)`
<a name="fbcunn.HSM:updateGradInputCUDA"></a>
 * `fbcunn.HSM:updateGradInputCUDA(input, target)`
<a name="fbcunn.HSM:backward"></a>
 * `fbcunn.HSM:backward(input, target, scale)`
<a name="fbcunn.HSM:updateParameters"></a>
 * `fbcunn.HSM:updateParameters(learning_rate)`
<a name="fbcunn.HSM:zeroGradParameters"></a>
 * `fbcunn.HSM:zeroGradParameters()`
<a name="fbcunn.HSM:zeroGradParametersClass"></a>
 * `fbcunn.HSM:zeroGradParametersClass(input, target)`
