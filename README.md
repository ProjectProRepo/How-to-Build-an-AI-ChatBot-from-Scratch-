# How to Build an AI ChatBot from Scratch?

This repository demonstrates how to build an AI chatbot using the Mistral-7B model with the CTransformers library in Python. The chatbot allows users to interact with the model using Panel's ChatInterface.

## Features
- Loads the **Mistral-7B-Instruct** model using ctransformers
- Supports both **synchronous** and **asynchronous** inference
- Implements a chatbot UI using **Panel**
- **Streams responses** for a better user experience
- **GPU acceleration** support

## Project Modules
### 1. Model Loading and Initialization
This module is responsible for loading the **Mistral-7B-Instruct** model using ctransformers. It ensures the model is initialized with the appropriate configuration, such as setting **GPU layers** for acceleration.

### 2. Asynchronous and Synchronous Inference
The chatbot supports both **synchronous** and **asynchronous** processing. The synchronous method generates responses in a blocking manner, while the asynchronous approach allows **streaming responses** token-by-token for a smoother user experience.

### 3. Chatbot Interface
The chatbot interface is built using **Panel's ChatInterface**. This module manages user interactions, sending queries to the model, and displaying responses in a chat-style format.

### 4. Response Streaming
To provide a seamless user experience, the chatbot **streams responses** rather than waiting for full text generation. This improves responsiveness, especially for longer answers.

### 5. GPU Optimization
The chatbot allows configuration of **GPU layers** for faster inference. This module detects system capabilities and adjusts settings to optimize performance.

## Notes
- If using a **GPU**, adjust `gpu_layers` for **optimal performance**.
- Be careful when running large models, as they can be **memory-intensive**.

For a detailed description of the code and the steps involved, refer to this [How to Build an AI ChatBot from Scratch?](https://www.projectpro.io/article/how-to-build-an-ai-chatbot-from-scratch/1078) blog.

