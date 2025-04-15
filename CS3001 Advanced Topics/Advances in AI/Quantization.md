> compressing a LLM by converting weights and activation values of high precision data, usually 32-bit floating point (FP32) or 16-bit floating point (FP16), to a lower-precision data, like 8-bit integer (INT8).

LLMs require a lot of processing power and memory so we can sacrifice some (negligible) precision in favour of less processing requirements - balance 

pros of quantization
- faster inference - quicker calculations which reduces latency despite reducing accuracy
- efficiency
- better compatibility with integer operations to support older computers that don’t support floating point operations