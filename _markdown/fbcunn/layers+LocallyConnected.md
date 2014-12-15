

### LocallyConnected.lua ###

Copyright 2004-present Facebook. All Rights Reserved.

<a name="fbcunn.LocallyConnected.dok"></a>


## fbcunn.LocallyConnected ##

LocallyConnected layer

See https://code.google.com/p/cuda-convnet/wiki/LayerParams#Locally-connected_layer_with_unshared_weights



#### Undocumented methods ####

<a name="fbcunn.LocallyConnected"></a>
 * `fbcunn.LocallyConnected(nInputPlane, iW, iH, nOutputPlane, kW, kH,
                                 dW, dH)`
<a name="fbcunn.LocallyConnected:outputSize"></a>
 * `fbcunn.LocallyConnected:outputSize()`
<a name="fbcunn.LocallyConnected:reset"></a>
 * `fbcunn.LocallyConnected:reset(stdv)`
<a name="fbcunn.LocallyConnected:updateOutput"></a>
 * `fbcunn.LocallyConnected:updateOutput(input)`
<a name="fbcunn.LocallyConnected:updateGradInput"></a>
 * `fbcunn.LocallyConnected:updateGradInput(input, gradOutput)`
<a name="fbcunn.LocallyConnected:accGradParameters"></a>
 * `fbcunn.LocallyConnected:accGradParameters(input, gradOutput, scale)`
