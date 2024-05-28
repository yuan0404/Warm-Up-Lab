## Name : 趙堉安

* About throughputs , please record the Tokens / Sec of Eval Time 

### Basic Challenge
| Throughputs (Tokens/sec) | CPU      | GPU      | 
| --------                 | -------- | -------- | 
| tinyllama-1.1b-chat-v0.3.Q4_K_M.gguf  | 10.15     | 102.53     |


### Medium Challenge
| Throughputs (Tokens/sec) | CPU      | GPU      | 
| --------                 | -------- | -------- | 
| tinyllama-1.1b-chat-v0.3.Q4_K_M.gguf  | 4.70     | 154.48     |
| TinyLlama-1.1B-Chat-v1.0-f16  | 4.60     | 72.44     |



### Advance Challenge
| Throughputs (Tokens/sec) | CPU      | GPU      | 
| --------                 | -------- | -------- | 
| tinyllama-1.1b-chat-v0.3.Q4_K_M.gguf  | 9.23     | 168.98     |
| TinyLlama-1.1B-Chat-v1.0-f16  | 5.21     | 72.93     |
| TinyLlama-1.1B-Chat-v1.0-Q8  | 5.76     | 83.90     |


### Advance Challenge

|                           | Accuracy  |
| --------                 | --------  |
| tinyllama-1.1b-chat-v0.3.Q4_K_M.gguf | 3/10     |
| TinyLlama-1.1B-Chat-v1.0-f16         | 2/10     |
| TinyLlama-1.1B-Chat-v1.0-Q8          | 1/10     |

### Questions
* What problems you encountered? How you solve it?
  1. Fail to use "-ngl", rebuild llama.cpp with "make LLAMA_CUDA=1".
  2. Fail to inference the "TinyLlama-1.1B-Chat-v0.3-GGUF" model without building llama.cpp with "make LLAMA_CURL=1", use "!wget" to inference the model.
  3. Log information output will make the answers of each model unintuitive, use "--log-disable" to disable the output of log.
* What you observed between CPU / GPU performance ?
  
  
* Will quantization or smaller-parameters model impact model accuracy or inference throughput ? If so , what's the variation?
  


