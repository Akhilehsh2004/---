# ---
SEA-LION v4 is a 27B parameter multilingual &amp; multimodal AI model co-developed by AI Singapore &amp; Google. Optimized for Southeast Asian languages while supporting Hindi &amp; English, it leads benchmarks under 200B params with state-of-the-art text+vision reasoning, efficient FP4/FP8 deployment, and enterprise-ready tools.


Here is a **powerful, professional README.md intro** for SEA-LION v4, combining the latest features, vision, benchmarks, and developer info:

***

# SEA-LION v4: Multilingual & Multimodal AI Powerhouse for Southeast Asia

**SEA-LION v4** is a breakthrough open-source AI model from AI Singapore and Google, built on the Gemma 3 architecture with 27B parameters. Designed to propel Southeast Asian innovation, it excels in regional languages—Tamil, Malay, Burmese, Filipino, Thai, Vietnamese, Indonesian—while matching global models in English, Hindi, and other major tongues. SEA-LION v4 is the #1 model under 200B parameters on the SEA-HELM benchmark and ranks top-5 worldwide, rivaling models 3–10x larger in efficiency and capability.[1][2][3]

## Why Choose SEA-LION v4

- **Multilingual Mastery:** Unmatched support for Southeast Asian languages, plus broad global coverage for diverse applications.[2][3]
- **Multimodal Intelligence:** Advanced text + vision capabilities, document comprehension, visual Q&A, and image-grounded reasoning.[3][4]
- **Efficient & Portable:** FP4/FP8 quantization enables fast inference on consumer laptops (32GB RAM), making state-of-the-art AI truly accessible.[5][6][2]
- **Enterprise Ready:** Structured outputs (JSON), agentic function calling for direct workflow integration, with safe and secure alignment for responsible deployments.[4][1]
- **Open Source & Commercially Usable:** Available under a permissive license on Hugging Face, Google Cloud, AWS, Kaggle, NVIDIA NIM, and more.[2][3]
- **Extensive Context Handling:** Supports up to 128K token context—ideal for long documents, multilingual materials, and complex dialogues.[7][3][4]

## Benchmarks

- Ranks #1 on SEA-HELM for models under 200B parameters, outperforming larger open and closed models in Southeast Asian languages and tasks.[3][2]
- Places among the global top five models for multimodal and multilingual reasoning, matching or surpassing models 3–10x larger.[2]

## Quick Start

```python
from transformers import AutoModelForCausalLM, AutoTokenizer
tokenizer = AutoTokenizer.from_pretrained("aisingapore/Gemma-SEA-LION-v4-27B-IT", trust_remote_code=True)
model = AutoModelForCausalLM.from_pretrained("aisingapore/Gemma-SEA-LION-v4-27B-IT", trust_remote_code=True)
prompt = "Translate to Vietnamese: Artificial Intelligence transforms Southeast Asia."
tokens = tokenizer(prompt, return_tensors="pt")
output = model.generate(tokens["input_ids"], max_new_tokens=64)
print(tokenizer.decode(output, skip_special_tokens=True))
```


## Vision

SEA-LION v4 bridges the digital equity gap for over 600 million people in Southeast Asia, setting a new standard for inclusive, efficient, and open AI—empowering both local and global innovation.[1][2]

***




