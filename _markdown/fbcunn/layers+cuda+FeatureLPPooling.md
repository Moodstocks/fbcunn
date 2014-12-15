

### FeatureLPPooling.lua ###

Copyright 2004-present Facebook. All Rights Reserved.

<a name="fbcunn.FeatureLPPooling.dok"></a>


## fbcunn.FeatureLPPooling ##


<a class="entityLink" href="https://github.com/facebook/fbcunn/blob/d84530ee7c84c5651f674d115a45e3ab8cbb39d2/layers/cuda/FeatureLPPooling.lua#L32">[src]</a>
<a name="fbcunn.FeatureLPPooling"></a>


### fbcunn.FeatureLPPooling(width, stride, power, batch_mode) ###


Possible inputs that we handle:

#### `batch_mode = false`
The dimensionality of the input chooses between the following modes:

```
[feature dim]
[feature dim][opt dim 1]
[feature dim][opt dim 1][opt dim 2]
```

#### `batch_mode = true`
The dimensionality of the input chooses between the following modes:
```
[batch dim][feature dim]
[batch dim][feature dim][opt dim 1]
[batch dim][feature dim][opt dim 1][opt dim 2]
```

The output has the same number of dimensions as the input, except the feature
dimension size is reduced to ((`input` - `width`) / `stride`) + 1



#### Undocumented methods ####

<a name="fbcunn.FeatureLPPooling:updateOutput"></a>
 * `fbcunn.FeatureLPPooling:updateOutput(input)`
<a name="fbcunn.FeatureLPPooling:updateGradInput"></a>
 * `fbcunn.FeatureLPPooling:updateGradInput(input, gradOutput)`
