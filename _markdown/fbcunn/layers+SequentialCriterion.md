

### SequentialCriterion.lua ###

Copyright 2004-present Facebook. All Rights Reserved.
Author: Michael Mathieu <myrhev@fb.com>

<a name="fbcunn.SequentialCriterion.dok"></a>


## fbcunn.SequentialCriterion ##


Combines a module and a criterion.

It is mainly thought for preprocessing, but trainable parameters
can be used if needed



#### Undocumented methods ####

<a name="fbcunn.SequentialCriterion"></a>
 * `fbcunn.SequentialCriterion(module, criterion)`
<a name="fbcunn.SequentialCriterion:parameters"></a>
 * `fbcunn.SequentialCriterion:parameters()`
<a name="fbcunn.SequentialCriterion:getParameters"></a>
 * `fbcunn.SequentialCriterion:getParameters()`
<a name="fbcunn.SequentialCriterion:updateOutput"></a>
 * `fbcunn.SequentialCriterion:updateOutput(input, target)`
<a name="fbcunn.SequentialCriterion:updateGradInput"></a>
 * `fbcunn.SequentialCriterion:updateGradInput(input, target)`
<a name="fbcunn.SequentialCriterion:accGradParameters"></a>
 * `fbcunn.SequentialCriterion:accGradParameters(input, target, scale)`
<a name="fbcunn.SequentialCriterion:accUpdateGradParameters"></a>
 * `fbcunn.SequentialCriterion:accUpdateGradParameters(input, target, scale)`
<a name="fbcunn.SequentialCriterion:updateParameters"></a>
 * `fbcunn.SequentialCriterion:updateParameters(learning_rate)`
<a name="fbcunn.SequentialCriterion:zeroGradParameters"></a>
 * `fbcunn.SequentialCriterion:zeroGradParameters()`
