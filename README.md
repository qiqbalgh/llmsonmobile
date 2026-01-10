# llmsonmobile
Mobile-Native GenAI: LLMs, Vector Search & RAG at the Edge

This project explores running modern GenAI workloads directly on mobile devices (iOS & Android) — including LLM inference, vector database search, and RAG — as a scalable alternative to centralized AI servers.

🚀 Motivation

Most GenAI systems face a concurrency scalability problem:

LLMs typically generate 100–200 tokens/sec per request

Scaling to hundreds or thousands of users requires massive server resources

Cloud dependency introduces cost, latency, and data-control concerns

Our approach:
👉 Push inference and retrieval to the edge using mobile devices.

📱 What This Project Does

Runs LLMs natively on iOS and Android

Implements mobile-native vector databases & search

Enables on-device RAG pipelines

Provides a custom Python runtime for mobile AI workflows

This turns phones into distributed AI nodes, offloading concurrency from servers.

✅ Current Capabilities

LLMs supported (1B–7B parameters):

DeepSeek

Phi-3

Mistral

Gemma

LLaMA

Qwen

Dolphin

Performance

Up to ~100 tokens/sec (device/model dependent)

Fast native vector search on iOS & Android

Platform Support

iOS (Metal / CoreML where applicable)

Android (CPU / NNAPI paths)

Python runtime on mobile

🧩 Use Cases

Offline GenAI applications

Privacy-preserving inference

Edge RAG systems

Field visualization & analytics

Distributed AI concurrency

Cost-sensitive AI deployments

🛠️ Project Status

✅ LLM inference on mobile

✅ Vector DB + search

🚧 RAG pipelines

🚧 Developer SDKs

🚧 Packaging & docs

See the Roadmap
 for details.

🤝 Who This Is For

Mobile developers

AI engineers

Edge computing researchers

Startups building privacy-first AI

Anyone interested in on-device GenAI

📬 Get Involved

If you’re interested in:

Collaborating

Testing on new devices

Porting models

Building real-world apps

👉 Open an issue, submit a PR, or connect.

Let’s push the boundaries of mobile-native AI.
