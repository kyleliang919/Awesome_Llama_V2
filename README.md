# Awesome_Llama_V2
An aggregated collection of llama_v2 s finetuned on different tasks/domains, sometimes they come with different name and can not be properly filtered by huggingface models.
Quality verification is done manually and qualitatively, it's based on my personal opinion of whether the model is usable so bar could be rather low, feel free to complain by submitting an issue or PR if you disagree.

## Disclaimer: 
This list is neither conclusive nor comprehensive, since I am too lazy to include all the gazillons of lora adapted models, there might be more good and fun ones out there.

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
| [elyza/ELYZA-japanese-Llama-2-7b](https://huggingface.co/elyza/ELYZA-japanese-Llama-2-7b) | ```N/A ```| ✅ | ❌ | 32000 | Japanese |
| [elyza/ELYZA-japanese-Llama-2-7b-instruct](https://huggingface.co/elyza/ELYZA-japanese-Llama-2-7b-instruct) | ```<s>[INST] <<SYS>>\nあなたは誠実で優秀な日本人のアシスタントです。\n<</SYS>>\n\n{instruction} [/INST]"</s> ```| ✅ | ✅ | 32000 | Japanese |
| [elyza/ELYZA-japanese-Llama-2-7b-fast](https://huggingface.co/elyza/ELYZA-japanese-Llama-2-7b-fast) | ```N/A ```| ✅ | ❌ | 45043 | Japanese |
| [elyza/ELYZA-japanese-Llama-2-7b-fast-instruct](https://huggingface.co/elyza/ELYZA-japanese-Llama-2-7b-fast-instruct) | ```<s>[INST] <<SYS>>\nあなたは誠実で優秀な日本人のアシスタントです。\n<</SYS>>\n\n{instruction} [/INST]"</s> ```| ✅ | ✅ | 45043 | Japanese |
| [kfkas/Llama-2-ko-7b-Chat](https://huggingface.co/kfkas/Llama-2-ko-7b-Chat) | ```아래는 작업을 설명하는 명령어입니다. 요청을 적절히 완료하는 응답을 작성하세요.\n\n### 명령어:\n{x}\n\n### 응답:```| ✅ | ❌ | 46336 | Korean |
| [beomi/llama-2-ko-7b](https://huggingface.co/beomi/llama-2-ko-7b) | ```N/A``` | ✅ | ✅ | 46336 | Korean |
| [LinkSoul/Chinese-Llama-2-7b](https://huggingface.co/LinkSoul/Chinese-Llama-2-7b) | ```[INST] <<SYS>>\nYou are a helpful, respectful and honest assistant. Always answer as helpfully as possible, while being safe.  Your answers should not include any harmful, unethical, racist, sexist, toxic, dangerous, or illegal content. Please ensure that your responses are socially unbiased and positive in nature.\n\nIf a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. If you don't know the answer to a question, please don't share false information.\n<</SYS>>\n\n{} [/INST]``` | ✅ | ✅ | 32000 | Chinese |
| [FlagAlpha/Atom-7B-Chat](https://huggingface.co/FlagAlpha/Atom-7B-Chat) | ``` <s>Human: {prompt}\n</s><s>Assistant: ```| ✅ | ✅ | 65000 | Chinese |
| [flozi00/Llama-2-7b-german-assistant-v3](https://huggingface.co/flozi00/Llama-2-7b-german-assistant-v3) | ```### User:{prompt}\n### Assistant:``` | ✅ | ✅ | 32000 | German |
| [LeoLM/leo-hessianai-7b-chat](https://huggingface.co/LeoLM/leo-hessianai-7b-chat) | ``` <\|im_start\|>system Dies ist eine Unterhaltung zwischen einem intelligenten, hilfsbereitem KI-Assistenten und einem Nutzer. Der Assistent gibt ausführliche, hilfreiche und ehrliche Antworten.<\|im_end\|> <\|im_start\|>user\n{prompt}<\|im_end\|>\n<\|im_start\|>assistant\n ```| ✅ | ✅ | 32128 | German |
| [LeoLM/leo-hessianai-7b-chat-bilingual](https://huggingface.co/LeoLM/leo-hessianai-7b-chat-bilingual) | ``` <\|im_start\|>system Dies ist eine Unterhaltung zwischen einem intelligenten, hilfsbereitem KI-Assistenten und einem Nutzer. Der Assistent gibt ausführliche, hilfreiche und ehrliche Antworten.<\|im_end\|> <\|im_start\|>user\n{prompt}<\|im_end\|>\n<\|im_start\|>assistant\n ``` | ✅ | ✅ | 32128 | German and English |
| [caracena/llamav2-spanish-alpaca](https://huggingface.co/caracena/llamav2-spanish-alpaca) | ```Unkonwn``` | ❌ | ❌ | 32000 | Spanish |


## Tools (APIs)
| Model Name                     |          Prompt Template            | Quality Verified  |  Chat | Vocab Size | Tool |
|--------------------------------|-------------------------------------|-------------------| ------| ---------- | ------|
| [ToolBench/ToolLlaMA-2-7b](https://huggingface.co/ToolBench/ToolLLaMA-2-7b) | ```System:{system prompt}\nUser:{prompt}\nAssistant:``` | ✅ | ✅ | 32000 | RapidAPI |

## Astronomy
| Model Name                     |          Prompt Template            | Quality Verified  |  Chat | Vocab Size |
|--------------------------------|-------------------------------------|-------------------| ------| ---------- |
| [universeTBD/astrollama](https://huggingface.co/universeTBD/astrollama/tree/main)     |    ```N/A``` | ❌ | ❌ | 32000 |

## Mental Health???
| Model Name                     |          Prompt Template            | Quality Verified  |  Chat | Vocab Size |
|--------------------------------|-------------------------------------|-------------------| ------| ---------- |
| [klyang/MentaLLaMA-chat-7B](https://huggingface.co/klyang/MentaLLaMA-chat-7B)     |    ```Consider this post:{post}Question:{question}Answer:``` | ✅ | ✅ | 32000 |

*Note: "✅" indicates models whose quality has been verified and "❌" indicates models that haven't been verified either due to being out side of my domain expertise or my laziness, it's not indicative of the actual quality of the model. (for example, I don't read Korean)*
