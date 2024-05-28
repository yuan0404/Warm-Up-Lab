## Name : 趙堉安

* About throughputs , please record the Tokens / Sec of Eval Time 

### Basic Challenge
| Throughputs (Tokens/sec) | CPU      | GPU      | 
| --------                 | -------- | -------- | 
| tinyllama-1.1b-chat-v0.3.Q4_K_M.gguf  | 9.67     | 164.04     |


### Medium Challenge
| Throughputs (Tokens/sec) | CPU      | GPU      | 
| --------                 | -------- | -------- | 
| tinyllama-1.1b-chat-v0.3.Q4_K_M.gguf  | 8.78     | 158.30     |
| TinyLlama-1.1B-Chat-v1.0-f16  | 5.20     | 71.12     |



### Advance Challenge
| Throughputs (Tokens/sec) | CPU      | GPU      | 
| --------                 | -------- | -------- | 
| tinyllama-1.1b-chat-v0.3.Q4_K_M.gguf  | 7.32     | 164.21     |
| TinyLlama-1.1B-Chat-v1.0-f16  | 4.21     | 87.33     |
| TinyLlama-1.1B-Chat-v1.0-Q8  | 6.66     | 100.80     |


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
  


