# llmsonmobile
📱 Mobile-Native GenAI at the Edge

Running LLMs, Vector Search, and RAG directly on iOS & Android

Solving GenAI concurrency and data-control challenges by pushing inference to the edge.

Why This Project Exists

Modern GenAI systems face a fundamental scalability issue:

LLMs typically generate ~100–200 tokens/sec per request

Handling hundreds or thousands of concurrent users requires expensive servers

Cloud dependency increases cost, latency, and data exposure

This project explores a different approach:

Distribute GenAI workloads across mobile devices instead of scaling servers.

What This Enables

✔ Native LLM inference on iOS & Android
✔ Mobile-native vector database & similarity search
✔ On-device RAG pipelines
✔ A custom Python runtime for mobile AI workflows

Together, these turn smartphones into distributed AI edge nodes.

Current Capabilities
🤖 Model Support

1B – 7B parameter models

Quantized & mixed-precision execution

Tested models include:

DeepSeek

Phi-3

Mistral

Gemma

LLaMA

Qwen

Dolphin

📊 Example Benchmark

4M vectors · 100 dimensions · 5-NN query

Device	Index Build	Query Time
iPhone 16 Pro	674 ms	75 ms
Moto G (~$50)	8.66 s	281 µs

Even low-cost Android devices deliver exceptional query latency once indexed.

Supported Platforms
Platform	Status
iOS	✅ Active
Android	✅ Active
Python (mobile)	✅ Working
RAG	🚧 In progress
