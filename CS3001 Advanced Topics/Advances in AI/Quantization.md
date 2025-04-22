> compressing a LLM by converting weights and activation values of high precision data, usually 32-bit floating point (FP32) or 16-bit floating point (FP16), to a lower-precision data, like 8-bit integer (INT8).

The two most common quantization cases are `float32 -> float16` and `float32 -> int8`.

![[Pasted image 20250421150434.png]]

what are the types of quantization
- linear quantization - mapping the range of floating-point values of the original weights to a range of fixed-point values evenly, using the high-precision data type for inference
- block-wise quantization - quantizing weights in smaller blocks rather than across the entire range, better handles variations within different parts of the model


when can quantization be performed 
- post-training quantization
	- quantizes after the LLM has been trained 
- quantization-aware training 
	- fine tune on data that can quantization can be done easily one e.g. including rounding or clipping the training data 
	- both the quantized and original weights are stores, the quantized version is used for inference but the unquantized version is updated during backpropagation
	- usually higher accuracy than PTQ


LLMs require a lot of processing power and memory so we can sacrifice some (negligible) precision in favour of less processing requirements - balance 

pros of quantization
- faster inference - quicker calculations which reduces latency despite reducing accuracy
- efficiency - reduced computational and memory costs of an inference 
- allows models to run on embedded devices that only support int types
- better compatibility with integer operations to support older computers that don’t support floating point operations

disadvantages 
- loss of accuracy (often negligible though)