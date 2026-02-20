llmsonmobile
📱 Mobile-Native GenAI at the Edge
<p align="center"> <img src="images/ipad_pro_vs_iphone16.jpg" width="800"/> </p>

Running LLMs, Vector Search, and RAG directly on iOS & Android

Solving GenAI concurrency and data-control challenges by pushing inference to the edge.

Why This Project Exists

Modern GenAI systems face a fundamental scalability problem:

LLMs typically generate ~100–200 tokens/sec per request

Supporting hundreds or thousands of concurrent users requires costly servers

Cloud dependency increases latency, operational cost, and data exposure

This project explores a different approach:

Distribute GenAI workloads across mobile devices instead of scaling servers.

What This Enables

✔ Native LLM inference on iOS & Android
✔ Mobile-native vector database & similarity search
✔ On-device RAG pipelines
✔ A custom Python runtime for mobile AI workflows

Together, these capabilities turn smartphones into distributed AI edge nodes.

Native Libraries Included

This repository includes prebuilt native binaries required for on-device inference across supported architectures.

📦 Android (ARM64)
libs/android/arm64-v8a/libc++_shared.so
libs/android/arm64-v8a/libllama.so


libllama.so – Core LLM inference engine

libc++_shared.so – Required C++ runtime dependency

Target ABI:

arm64-v8a

🍎 iOS (Device)
libs/ios/device/Llama.framework/Info.plist
libs/ios/device/Llama.framework/Llama
libs/ios/device/default.metallib
libs/ios/device/libllama.dylib
libs/ios/device/libllama_cpu.a
libs/ios/device/libllama_gpu.a


Llama.framework – Native inference framework

default.metallib – Metal GPU shaders

libllama_cpu.a – CPU backend

libllama_gpu.a – GPU backend (Metal)

libllama.dylib – Dynamic runtime

🍎 iOS (Simulator)
libs/ios/simulator/Llama.framework/Info.plist
libs/ios/simulator/Llama.framework/Llama
libs/ios/simulator/libllama.a
libs/ios/simulator/libllama.dylib


Provides simulator-compatible builds for development and testing.

LLMs on Mobile
<p align="center"> <img src="images/gemma-3-1b-it-f16.jpg" width="600"/> </p> <p align="center"> <img src="images/gemma-3-270m-Q8_0.jpg" width="600"/> </p>
🤖 Model Support

1B – 7B parameter models

Quantized and mixed-precision execution

Tested models include:

DeepSeek

Phi-3

Mistral

Gemma

LLaMA

Qwen

Dolphin

Vector Database & Search
<p align="center"> <img src="images/vector_db_search.jpg" width="700"/> </p>

Fast native vector indexing and similarity search running directly on mobile hardware, without server round-trips.

Performance Benchmarks
Vector Search Benchmark

4M vectors · 100 dimensions · 5-NN query

Device	Index Build	Query Time
iPhone 16 Pro	674 ms	75 ms
Moto G (~$50)	8.66 s	281 µs

Even low-cost Android devices deliver exceptional query latency once indexed.

Token Throughput (iPhone 16 Pro)
<p align="center"> <img src="images/iphonepro_tokens_sec.jpg" width="650"/> </p>
CPU vs GPU Execution (iPhone 16 Pro)
<p align="center"> <img src="images/iphonepro_cpu_vs_gpu.jpg" width="650"/> </p>
Supported Platforms
Platform	Status
iOS	✅ Active
Android	✅ Active
Python (mobile)	✅ Working
RAG	🚧 In progress
Takeaway

Mobile platforms are now capable of running serious GenAI workloads — including LLM inference, vector search, and Python-based workflows.

By shifting inference to the edge, we can:

Reduce server-side concurrency pressure

Improve latency and privacy

Enable cost-effective, scalable GenAI systems

The edge is ready.

⭐ If this project resonates with you, consider starring the repo or opening an issue to collaborate.
