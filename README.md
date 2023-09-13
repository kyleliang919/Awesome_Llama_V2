# Awesome_Llama_V2
An aggregated collection of llama_v2 s finetuned on different tasks/domains, sometimes they come with different name.
Quality verification is done manually and qualitatively, feel free to complain by submitting an issue or PR if you disagree.
Note that base llama 
# Llama_V2_7B

## Math
| Model Name                  |          Prompt Template            | Quality Verified  | Chat | Vocab Size |
|-----------------------------|-------------------------------------|-------------------|------|------------|
| [WizardLM/WizardMath-7B-V1.0](https://huggingface.co/WizardLM/WizardMath-7B-V1.0) |```Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:\n{instruction}\n\n### Response: Let's think step by step.``` | ✅ | ✅ | 32001 |

## Code (Python)
| Model Name                  |          Prompt Template            | Quality Verified  | Chat | Vocab Size |
|-----------------------------|-------------------------------------|-------------------|------|------------|
| [WizardLM/WizardCoder-Python-7B-V1.0](https://huggingface.co/WizardLM/WizardCoder-Python-7B-V1.0/tree/main) |```Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:\n{instruction}\n\n### Response:``` | ✅ | ✅ | 32001 |                     

## Language
| Model Name                  |          Prompt Template            | Quality Verified  | Chat | Vocab Size |
|-----------------------------|-------------------------------------|-------------------|------|------------|
| [elyza/ELYZA-japanese-Llama-2-7b](https://huggingface.co/elyza/ELYZA-japanese-Llama-2-7b) | ```<s>[INST] <<SYS>>\nあなたは誠実で優秀な日本人のアシスタントです。\n<</SYS>>\n\n{instruction} [/INST]"</s></details> ```| ✅ | ❌ | 32000 |
| [elyza/ELYZA-japanese-Llama-2-7b-instruct](https://huggingface.co/elyza/ELYZA-japanese-Llama-2-7b-instruct) | ```<s>[INST] <<SYS>>\nあなたは誠実で優秀な日本人のアシスタントです。\n<</SYS>>\n\n{instruction} [/INST]"</s></details> ```| ✅ | ✅ | 32000 |
| [elyza/ELYZA-japanese-Llama-2-7b-fast](https://huggingface.co/elyza/ELYZA-japanese-Llama-2-7b-fast) | ```<s>[INST] <<SYS>>\nあなたは誠実で優秀な日本人のアシスタントです。\n<</SYS>>\n\n{instruction} [/INST]"</s></details> ```| ✅ | ❌ | 45043 |
| [elyza/ELYZA-japanese-Llama-2-7b-fast-instruct](https://huggingface.co/elyza/ELYZA-japanese-Llama-2-7b-fast-instruct) | ```<s>[INST] <<SYS>>\nあなたは誠実で優秀な日本人のアシスタントです。\n<</SYS>>\n\n{instruction} [/INST]"</s></details> ```| ✅ | ✅ | 45043 |

## Code (SQL)
| Model Name                     |          Prompt Template            | Quality Verified  | Chat | Vocab Size |
|--------------------------------|-------------------------------------|-------------------|------| ---------- |
| [NumbersStation/nsql-llama-2-7B](https://huggingface.co/NumbersStation/nsql-llama-2-7B) |            N/A                      |        ❌         |   ❌ |  32000    |

## RapidAPI (toollama)
| Model Name                     |          Prompt Template            | Quality Verified  |  Chat | Vocab Size |
|--------------------------------|-------------------------------------|-------------------| ------| ---------- |
| ToolBench/ToolLLaMA-2-7b       |            N/A                      |        ✅         |   ❌ |  32000     |

*Note: "✅" indicates models whose quality has been verified and "❌" indicates models that haven't been verified.*
