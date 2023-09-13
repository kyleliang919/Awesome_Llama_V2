# Awesome_Llama_V2
An aggregated collection of llama_v2 s finetuned on different tasks/domains, sometimes they come with different name and can not be properly filtered by huggingface models.
Quality verification is done manually and qualitatively, it's based on my personal opinion of whether the model is usable so bar could be rather low, feel free to complain by submitting an issue or PR if you disagree.
Note that base llama 
# Finetuned Llama_V2_7B

## Math
| Model Name                  |          Prompt Template            | Quality Verified  | Chat | Vocab Size |
|-----------------------------|-------------------------------------|-------------------|------|------------|
| [WizardLM/WizardMath-7B-V1.0](https://huggingface.co/WizardLM/WizardMath-7B-V1.0) |```Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:\n{instruction}\n\n### Response: Let's think step by step.``` | ✅ | ✅ | 32001 |
| [TIGER-Lab/MAmmoTH-7B](https://huggingface.co/TIGER-Lab/MAmmoTH-7B) | ```Unknown``` | ❌ | ❌ | 32001 |
## Coding
| Model Name                  |          Prompt Template            | Quality Verified  | Chat | Vocab Size | Language | 
|-----------------------------|-------------------------------------|-------------------|------|------------|----------|
| [WizardLM/WizardCoder-Python-7B-V1.0](https://huggingface.co/WizardLM/WizardCoder-Python-7B-V1.0/tree/main) |```Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:\n{instruction}\n\n### Response:``` | ✅ | ✅ | 32001 | Python |
| [NumbersStation/nsql-llama-2-7B](https://huggingface.co/NumbersStation/nsql-llama-2-7B) | ```N/A``` | ❌ | ❌ | 32000 | SQL |
| [TIGER-Lab/MAmmoTH-Coder-7B](https://huggingface.co/TIGER-Lab/MAmmoTH-Coder-7B) | ```Unknown``` | ❌ | ❌ | 32017 | General |

                  

## Language
| Model Name                  |          Prompt Template            | Quality Verified  | Chat | Vocab Size | Language | 
|-----------------------------|-------------------------------------|-------------------|------|------------|----------|
| [elyza/ELYZA-japanese-Llama-2-7b](https://huggingface.co/elyza/ELYZA-japanese-Llama-2-7b) | ```<s>[INST] <<SYS>>\nあなたは誠実で優秀な日本人のアシスタントです。\n<</SYS>>\n\n{instruction} [/INST]"</s></details> ```| ✅ | ❌ | 32000 | Japanese |
| [elyza/ELYZA-japanese-Llama-2-7b-instruct](https://huggingface.co/elyza/ELYZA-japanese-Llama-2-7b-instruct) | ```<s>[INST] <<SYS>>\nあなたは誠実で優秀な日本人のアシスタントです。\n<</SYS>>\n\n{instruction} [/INST]"</s></details> ```| ✅ | ✅ | 32000 | Japanese |
| [elyza/ELYZA-japanese-Llama-2-7b-fast](https://huggingface.co/elyza/ELYZA-japanese-Llama-2-7b-fast) | ```<s>[INST] <<SYS>>\nあなたは誠実で優秀な日本人のアシスタントです。\n<</SYS>>\n\n{instruction} [/INST]"</s></details> ```| ✅ | ❌ | 45043 | Japanese |
| [elyza/ELYZA-japanese-Llama-2-7b-fast-instruct](https://huggingface.co/elyza/ELYZA-japanese-Llama-2-7b-fast-instruct) | ```<s>[INST] <<SYS>>\nあなたは誠実で優秀な日本人のアシスタントです。\n<</SYS>>\n\n{instruction} [/INST]"</s></details> ```| ✅ | ✅ | 45043 | Japanese |
| [kfkas/Llama-2-ko-7b-Chat](https://huggingface.co/kfkas/Llama-2-ko-7b-Chat) | ```아래는 작업을 설명하는 명령어입니다. 요청을 적절히 완료하는 응답을 작성하세요.\n\n### 명령어:\n{x}\n\n### 응답:```| ✅ | ❌ | 46336 | Korean |
| [LinkSoul/Chinese-Llama-2-7b](https://huggingface.co/LinkSoul/Chinese-Llama-2-7b) | ```[INST] <<SYS>>\nYou are a helpful, respectful and honest assistant. Always answer as helpfully as possible, while being safe.  Your answers should not include any harmful, unethical, racist, sexist, toxic, dangerous, or illegal content. Please ensure that your responses are socially unbiased and positive in nature.\n\nIf a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. If you don't know the answer to a question, please don't share false information.\n<</SYS>>\n\n{} [/INST]``` | ✅ | ✅ | 32000 | Chinese |
| [flozi00/Llama-2-7b-german-assistant-v3](https://huggingface.co/flozi00/Llama-2-7b-german-assistant-v3) | ```### User:{prompt}\n### Assistant:``` | ✅ | ✅ | 32000 | German |


## Tools (APIs)
| Model Name                     |          Prompt Template            | Quality Verified  |  Chat | Vocab Size | Tool |
|--------------------------------|-------------------------------------|-------------------| ------| ---------- | ------|
| [ToolBench/ToolLlaMA-2-7b](https://huggingface.co/ToolBench/ToolLLaMA-2-7b) | ```N/A``` | ✅ | ❌ | 32000 | RapidAPI |

*Note: "✅" indicates models whose quality has been verified and "❌" indicates models that haven't been verified either due to being out side of my domain expertise or my laziness, it's not indicative of the actual quality of the model. (for example, I don't read Korean)*
