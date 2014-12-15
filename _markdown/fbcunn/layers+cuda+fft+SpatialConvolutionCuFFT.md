<a name="fbcunn.SpatialConvolutionCuFFT.dok"></a>


## fbcunn.SpatialConvolutionCuFFT ##

Copyright 2004-present Facebook. All Rights Reserved.


#### Undocumented methods ####

<a name="fbcunn.SpatialConvolutionCuFFT"></a>
 * `fbcunn.SpatialConvolutionCuFFT(nInputPlane, nOutputPlane,
                                        kW, kH, dW, dH, debug, printDebug)`
<a name="fbcunn.SpatialConvolutionCuFFT:reset"></a>
 * `fbcunn.SpatialConvolutionCuFFT:reset(stdv)`
<a name="fbcunn.SpatialConvolutionCuFFT:updateOutput"></a>
 * `fbcunn.SpatialConvolutionCuFFT:updateOutput(input)`
<a name="fbcunn.SpatialConvolutionCuFFT:explorePerformance"></a>
 * `fbcunn.SpatialConvolutionCuFFT:explorePerformance(input, batches,
      inputs, planes, inputRows, inputCols, kernelRows, kernelCols)`
<a name="fbcunn.SpatialConvolutionCuFFT:cleanupBuffers"></a>
 * `fbcunn.SpatialConvolutionCuFFT:cleanupBuffers(input)`
<a name="fbcunn.SpatialConvolutionCuFFT:updateGradInput"></a>
 * `fbcunn.SpatialConvolutionCuFFT:updateGradInput(input, gradOutput)`
<a name="fbcunn.SpatialConvolutionCuFFT:accGradParameters"></a>
 * `fbcunn.SpatialConvolutionCuFFT:accGradParameters(input, gradOutput, scale)`
