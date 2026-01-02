# KMPMLBench (Kotlin Multiplatform ML Benchmark)

A powerful, cross-platform benchmarking suite designed to evaluate the performance of various Deep Learning inference engines across **Mobile (Android & iOS)** and **Desktop (Windows, macOS, Linux)** using **Kotlin Multiplatform**.

## 🎯 Motivation
The ML landscape is fragmented. Developers often struggle to decide which engine to use: Should I stick with TFLite for ease of use, or integrate NCNN for raw performance?

**KMPMLBench** provides a unified "Lab" to test these scenarios with identical models and logic, minimizing the "overhead" of platform-specific implementations.

## 🚀 Supported Platforms & Engines

| Engine | Android | iOS | Desktop (JVM/Native) | Acceleration | Status |
| :--- | :---: | :---: | :---: | :--- | :--- |
| **ONNX Runtime** | 🏗️ | 🏗️ | 🏗️ | CoreML, DirectML, XNNPACK | In Progress |
| **TensorFlow Lite** | 📅 | 📅 | 📅 | NNAPI, CoreML, GPU | Planned |
| **NCNN** | 📅 | 📅 | 📅 | Vulkan, Metal | Planned |
| **MNN** | 📅 | 📅 | 📅 | OpenCL, Vulkan, Metal | Planned |
| **ExecuTorch** | 📅 | 📅 | 📅 | XNNPACK, CoreML | Planned |

## 🧠 Benchmarking Tasks (Planned)
While the project started with **Super-Resolution**, it is designed to be modular:

- [ ] **Super-Resolution:** ESPCN, FSRCNN, Real-ESRGAN.
- [ ] **Image Classification:** MobileNetV3, EfficientNet (Planned).
- [ ] **Object Detection:** YOLOv8-Nano (Planned).
- [ ] **On-device LLM:** Gemma 2B / Phi-2 (Experimental via ExecuTorch).

## 📊 Performance Metrics (Planned)
We measure more than just speed:
1. **Inference Latency:** Average time per execution (ms).
2. **Initialization Time:** Cold start vs. warm start (ms).
3. **Memory Peak:** Maximum RAM/VRAM usage (MB).
4. **Energy Consumption:** (Mobile only) Battery impact during prolonged tasks.
