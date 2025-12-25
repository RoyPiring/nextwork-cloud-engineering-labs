<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# How to Use DeepSeek

**Project Link:** [View Project](http://learn.nextwork.org/projects/ai-llm-deepseek)

**Author:** Roy Piring Jr  
**Email:** rpiringhawaii@gmail.com

---

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/ai-llm-deepseek_kkkkkkkk)

---

## Introducing Today's Project!

This project evaluates DeepSeek as an alternative large language model and validates local execution using Ollama and Chatbox. The focus is on comparing local and hosted LLM workflows under practical operational constraints.

### Tools and concepts

The system uses DeepSeek for model evaluation, Ollama for local model orchestration, and ChatGPT as a comparison baseline. The purpose is to assess capability, latency, and operational control differences rather than individual tool features.

### Project reflection

The implementation was completed within a constrained time window and focused on validating local model execution paths.

The primary integration risk was ensuring Ollama served models consistently for repeatable inference. The outcome confirmed DeepSeek is viable within defined constraints but not a drop-in replacement for hosted models.

---

## Exploring DeepSeek

DeepSeek is a general-purpose language model positioned as an alternative to hosted OpenAI services. It supports comparable prompt-driven tasks but differs in deployment and operational assumptions.

Web-based usage introduces data residency, availability, and network dependency risks. Local installation or API-based access reduces these risks by retaining execution and data control within the user environment.

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/ai-llm-deepseek_aaaaaaaa)

---

## Ollama and DeepSeek R1

Ollama is an open-source platform designed to manage and run language models locally. Its architecture prioritizes local execution, transparency, and independence from external service availability.

Ollama focuses on local models, while OpenAI operates as a hosted subscription service. There is no shared model compatibility between the two platforms, which affects portability and evaluation methodology.

DeepSeek R1 models were downloaded and served locally through Ollama to enable offline inference. Local execution reduced network dependency and improved response consistency. Terminal output exposed limited model reasoning metadata during execution.

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/ai-llm-deepseek_gggggggg)

---

## DeepSeek R1 Sizes

DeepSeek R1 is available in 7B, 14B, and 68B parameter variants. Model size directly impacts reasoning depth, memory consumption, and compute requirements.

Model selection must align with available CPU, RAM, and GPU resources. Smaller models prioritize stability and responsiveness, while larger models increase output quality at the cost of higher resource utilization.

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/ai-llm-deepseek_iiiiiiii)

---

## Chatbox

Chatbox was installed as a local client interface and configured to connect to Ollama for serving DeepSeek models. This setup enabled rapid prompt testing and side-by-side comparison with other LLMs.

Two DeepSeek R1 model sizes were evaluated using identical prompts. The larger model produced acceptable outputs but exhibited slower response times, illustrating expected performance tradeoffs between latency and model capacity.

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/ai-llm-deepseek_kkkkkkkk)

---

## Temperature Settings

Temperature controls response variability during text generation. Higher values increase randomness, while lower values emphasize determinism and consistency.

Identical prompts were executed across multiple temperature settings to observe behavioral differences. Responses were also compared against OpenAI outputs to evaluate coherence and stability.

High-temperature outputs exhibited increased randomness and reduced logical structure. Low-temperature outputs demonstrated more consistent and predictable reasoning patterns.

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/ai-llm-deepseek_aregearg)

---

## DeepSeek vs. OpenAI

DeepSeek R1 and OpenAI models were evaluated using prompt-based tests covering creative writing, code generation, factual recall, and reasoning tasks. Results varied by task type and complexity.

In script generation tasks, OpenAI models produced more consistent structure and fewer errors. DeepSeek delivered faster responses but showed reduced accuracy in complex scenarios.

Model selection depends on tolerance for error, cost constraints, and latency requirements rather than raw capability alone.

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/ai-llm-deepseek_dfgbewrwq3)

---

## Token Efficiency

OpenAI access required API authentication for programmatic usage, enabling text generation and analysis workflows. Token usage varied based on temperature and prompt complexity.

Higher temperature settings in OpenAI increased creativity but reduced accuracy and relevance due to broader token sampling.

DeepSeek produced comparable outputs using fewer tokens under similar prompts. Lower token consumption improves cost efficiency and throughput in constrained or local execution environments.

![Image](http://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/ai-llm-deepseek_aagerergerg)

---
