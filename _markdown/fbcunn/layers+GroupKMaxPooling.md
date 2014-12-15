

### GroupKMaxPooling.lua ###

Copyright 2004-present Facebook. All Rights Reserved.

<a name="fbcunn.GroupKMaxPooling.dok"></a>


## fbcunn.GroupKMaxPooling ##


Group k-max pooling performs pooling along a dimension of arbitrary length
(e.g. a sentence) down to a length of ${k}$.

Given a matrix where rows are words and columns are embedding dimensions, we
compute the ${L^2}$ norm of each word:

```
   o---------o
w1 |         | -> norm1
w2 |         | -> norm2
w3 |         | -> norm3
w4 |         | -> norm4
   o---------o
```

Group K-max pooling keeps the K words with largest norm and discards the
rest.



#### Undocumented methods ####

<a name="fbcunn.GroupKMaxPooling"></a>
 * `fbcunn.GroupKMaxPooling(k, k_dynamic)`
<a name="fbcunn.GroupKMaxPooling:updateOutput"></a>
 * `fbcunn.GroupKMaxPooling:updateOutput(input)`
<a name="fbcunn.GroupKMaxPooling:updateGradInput"></a>
 * `fbcunn.GroupKMaxPooling:updateGradInput(input, gradOutput)`
