# Awesome AI/ML Software Tools for Developers [![Awesome](https://awesome.re/badge.svg)]

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](CONTRIBUTING.md)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg?style=flat-square)](LICENSE)
[![Awesome Lint](https://img.shields.io/badge/checked%20with-awesome--lint-blue.svg?style=flat-square)](https://github.com/sindresorhus/awesome-lint)
[![Last Commit](https://img.shields.io/github/last-commit/sudo-su-coffee/awesome-ml-tools?style=flat-square)](https://github.com/sudo-su-coffee/awesome-ml-tools/commits/main)
[![Stars](https://img.shields.io/github/stars/sudo-su-coffee/awesome-ml-tools?style=flat-square)](https://github.com/sudo-su-coffee/awesome-ml-tools/stargazers)

> A practical, self-hostable, and AWS/Azure-portable curated list of **180 tools** covering the complete AI/ML delivery path — from idea to production.

AI/ML development is no longer only about training a model. A usable product also needs data collection, labeling, retrieval, prompts, agents, evaluation, privacy, model serving, billing, observability, CI/CD, and a reliable user experience. The challenge is choosing enough software to move quickly without creating an unmaintainable platform.

This list follows a practical **FOSS-first** philosophy: prefer focused and composable tools, keep data and model artifacts portable, use standard APIs, avoid unnecessary platform complexity, and introduce GPUs or Kubernetes only when the workload justifies them.

> **The fastest path is not "use every AI tool."** Start with one model, one dataset, one evaluation set, one API, and one observable deployment. Add components when a real bottleneck appears.

## Contents

- [Legend](#legend)
- [How to Use This List](#how-to-use-this-list)
- [AI Application Platforms and Chat Interfaces](#ai-application-platforms-and-chat-interfaces)
- [Agent Frameworks and Orchestration](#agent-frameworks-and-orchestration)
- [Local Model Runtimes and Model Clients](#local-model-runtimes-and-model-clients)
- [RAG, Vector Search, and Retrieval](#rag-vector-search-and-retrieval)
- [Dataset Creation, Labeling, and Data Quality](#dataset-creation-labeling-and-data-quality)
- [Classical ML and Deep Learning Foundations](#classical-ml-and-deep-learning-foundations)
- [Fine-Tuning, Alignment, and Distributed Training](#fine-tuning-alignment-and-distributed-training)
- [Experiment Tracking, MLOps, and Pipelines](#experiment-tracking-mlops-and-pipelines)
- [Model Serving and Inference Optimization](#model-serving-and-inference-optimization)
- [AI Evaluation, Tracing, Safety, and Observability](#ai-evaluation-tracing-safety-and-observability)
- [Voice, Speech, and Audio AI](#voice-speech-and-audio-ai)
- [Computer Vision, OCR, Documents, and Multimodal AI](#computer-vision-ocr-documents-and-multimodal-ai)
- [Synthetic Data, Privacy, Governance, and AI Security](#synthetic-data-privacy-governance-and-ai-security)
- [Git, CI/CD, Kubernetes, and AI Infrastructure](#git-cicd-kubernetes-and-ai-infrastructure)
- [Productization, AI Operations, and Platform Integration](#productization-ai-operations-and-platform-integration)
- [MVP-to-Production Paths](#mvp-to-production-paths)
- [Git-Connected AI Development Loop](#git-connected-ai-development-loop)
- [AWS and Azure Migration](#aws-and-azure-migration)
- [AI/ML Production Checklist](#aiml-production-checklist)
- [Contributing](#contributing)
- [License](#license)

## Legend

| Label | Meaning |
|---|---|
| 🟢 **Now** | Usually practical for an MVP or a small team. |
| 🟡 **Evaluate** | Useful when a concrete problem appears; validate complexity and fit first. |
| 🔵 **Production** | Appropriate when throughput, latency, reliability, or operational requirements justify it. |
| 🟣 **Later** | Powerful but usually requires clusters, GPUs, complex operations, or a larger team. |
| ⚠️ **License check** | Review current license, model license, edition, trademark, and hosted-service terms before resale or white-labeling. |
| **Application/Platform** | A deployable project or service. |
| **Framework/Library** | A component used inside your application or training pipeline. |

## How to Use This List

The catalog is deliberately split by responsibility. Choose one or two tools from a category, not the entire category. A small team may need only eight to twelve tools for its first product. Every tool has a direct link, a short purpose, a type, and a suggested adoption stage.

---

## AI Application Platforms and Chat Interfaces

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 1 | [Open WebUI](https://openwebui.com/) | Self-hosted chat interface for local and remote models | Application | 🟢 Now |
| 2 | [LibreChat](https://www.librechat.ai/) | Multi-provider conversational AI interface | Application | 🟢 Now |
| 3 | [AnythingLLM](https://anythingllm.com/) | Private document chat and knowledge assistants | Application | 🟢 Now |
| 4 | [Dify](https://dify.ai/) | Visual LLM apps, workflows, and chatbots | Platform | 🟢 Now |
| 5 | [Flowise](https://flowiseai.com/) | Visual LLM flows and agent prototypes | Platform | 🟢 Now |
| 6 | [Langflow](https://www.langflow.org/) | Visual orchestration for LLM applications | Platform | 🟢 Now |
| 7 | [Rasa](https://rasa.com/) | Controlled conversational assistants and intent workflows | Platform | 🟢 Now |
| 8 | [Onyx](https://www.onyx.app/) | Enterprise search and knowledge assistant | Application | 🟡 Evaluate |
| 9 | [Khoj](https://khoj.dev/) | Self-hosted personal knowledge assistant | Application | 🟢 Now |
| 10 | [Jan](https://jan.ai/) | Local-first desktop AI assistant | Application | 🟢 Now |
| 11 | [PrivateGPT](https://github.com/zylon-ai/private-gpt) | Private document question answering | Application | 🟡 Evaluate |
| 12 | [LobeChat](https://lobehub.com/) | Open-source AI chat and agent workspace | Application | 🟢 Now |

**[⬆ back to top](#contents)**

## Agent Frameworks and Orchestration

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 13 | [LangChain](https://www.langchain.com/) | Chains, tool calls, retrieval, and agents | Framework | 🟢 Now |
| 14 | [LlamaIndex](https://www.llamaindex.ai/) | Data connectors, indexing, and RAG | Framework | 🟢 Now |
| 15 | [Haystack](https://haystack.deepset.ai/) | Search, RAG, pipelines, and LLM applications | Framework | 🟢 Now |
| 16 | [Semantic Kernel](https://learn.microsoft.com/semantic-kernel/) | AI orchestration, plugins, memory, and tools | Framework | 🟡 Evaluate |
| 17 | [AutoGen](https://microsoft.github.io/autogen/) | Multi-agent conversations and task orchestration | Framework | 🟡 Evaluate |
| 18 | [CrewAI](https://www.crewai.com/) | Role-based multi-agent workflows | Framework | 🟡 Evaluate |
| 19 | [DSPy](https://dspy.ai/) | Programmatic prompt and LM-pipeline optimization | Framework | 🟡 Evaluate |
| 20 | [PydanticAI](https://ai.pydantic.dev/) | Typed Python agents and tool calling | Framework | 🟢 Now |
| 21 | [Letta](https://www.letta.com/) | Stateful agents and long-term memory | Platform | 🟡 Evaluate |
| 22 | [smolagents](https://huggingface.co/docs/smolagents/) | Lightweight code and tool-using agents | Framework | 🟢 Now |
| 23 | [OpenHands](https://openhands.dev/) | Software-engineering agents for repositories and tools | Application | 🟡 Evaluate |
| 24 | [Browser Use](https://browser-use.com/) | Browser automation for AI agents | Framework | 🟡 Evaluate |

**[⬆ back to top](#contents)**

## Local Model Runtimes and Model Clients

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 25 | [Ollama](https://ollama.com/) | Local model download and inference | Runtime | 🟢 Now |
| 26 | [LocalAI](https://localai.io/) | OpenAI-compatible local model API | Server | 🟢 Now |
| 27 | [LM Studio](https://lmstudio.ai/) | Desktop local model execution and API serving | Application | 🟢 Now |
| 28 | [llama.cpp](https://github.com/ggml-org/llama.cpp) | Portable CPU/GPU inference runtime | Runtime | 🟢 Now |
| 29 | [vLLM](https://vllm.ai/) | High-throughput LLM serving | Server | 🔵 Production |
| 30 | [Text Generation Inference](https://github.com/huggingface/text-generation-inference) | Production text-generation serving | Server | 🔵 Production |
| 31 | [SGLang](https://github.com/sgl-project/sglang) | Efficient LLM and multimodal serving | Server | 🔵 Production |
| 32 | [MLC LLM](https://mlc.ai/mlc-llm/) | Deploy LLMs across local and edge hardware | Runtime | 🟡 Evaluate |
| 33 | [MLX](https://github.com/ml-explore/mlx) | Machine learning framework for Apple Silicon | Framework | 🟢 Now (Mac) |
| 34 | [GPT4All](https://www.nomic.ai/gpt4all) | Private local chat and model execution | Application | 🟢 Now |
| 35 | [KoboldCpp](https://github.com/LostRuins/koboldcpp) | Local GGUF model server and UI | Application | 🟡 Evaluate |
| 36 | [Text Generation WebUI](https://github.com/oobabooga/text-generation-webui) | Local model experimentation interface | Application | 🟡 Evaluate |

**[⬆ back to top](#contents)**

## RAG, Vector Search, and Retrieval

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 37 | [Qdrant](https://qdrant.tech/) | Vector search and semantic retrieval | Server | 🟢 Now |
| 38 | [Weaviate](https://weaviate.io/) | Vector search and AI retrieval | Server | 🟡 Evaluate |
| 39 | [Milvus](https://milvus.io/) | Distributed vector database | Server | 🔵 Production |
| 40 | [Chroma](https://www.trychroma.com/) | Local-first embeddings and vector search | Database | 🟢 Now |
| 41 | [LanceDB](https://lancedb.com/) | Embedded vector and multimodal data search | Database | 🟡 Evaluate |
| 42 | [pgvector](https://github.com/pgvector/pgvector) | Vector similarity inside PostgreSQL | Database extension | 🟢 Now |
| 43 | [Vespa](https://vespa.ai/) | Large-scale search, ranking, and serving | Platform | 🔵 Production |
| 44 | [OpenSearch](https://opensearch.org/) | Search, analytics, and vector retrieval | Platform | 🟡 Evaluate |
| 45 | [Elasticsearch](https://www.elastic.co/elasticsearch/) | Search, analytics, and vector retrieval | Platform | 🟡 Evaluate |
| 46 | [R2R](https://r2r-docs.sciphi.ai/) | RAG ingestion, search, and retrieval APIs | Platform | 🟡 Evaluate |
| 47 | [txtai](https://neuml.github.io/txtai/) | Semantic search and language-model workflows | Framework | 🟡 Evaluate |
| 48 | [Vald](https://vald.vdaas.org/) | Cloud-native distributed vector search | Platform | 🟣 Later |

**[⬆ back to top](#contents)**

## Dataset Creation, Labeling, and Data Quality

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 49 | [DVC](https://dvc.org/) | Git-like versioning for datasets and models | Platform | 🟢 Now |
| 50 | [Label Studio](https://labelstud.io/) | Text, image, audio, document, and LLM annotation | Application | 🟢 Now |
| 51 | [CVAT](https://www.cvat.ai/) | Computer-vision annotation and datasets | Application | 🟢 Now |
| 52 | [FiftyOne](https://voxel51.com/fiftyone/) | Inspect, curate, search, and evaluate vision data | Application | 🟡 Evaluate |
| 53 | [Roboflow](https://roboflow.com/) | Vision dataset preparation and deployment | Platform | 🟡 Evaluate |
| 54 | [Hugging Face Datasets](https://huggingface.co/docs/datasets/) | Load, transform, and share datasets | Framework | 🟢 Now |
| 55 | [lakeFS](https://lakefs.io/) | Git-like branching for data lakes | Platform | 🟣 Later |
| 56 | [Pachyderm](https://www.pachyderm.com/) | Data versioning and reproducible pipelines | Platform | 🟣 Later |
| 57 | [Great Expectations](https://greatexpectations.io/) | Dataset validation and quality expectations | Framework | 🟢 Now |
| 58 | [Cleanlab](https://cleanlab.ai/) | Find label errors and improve dataset quality | Framework | 🟡 Evaluate |
| 59 | [DataHub](https://datahubproject.io/) | Metadata catalog, lineage, and data discovery | Platform | 🟣 Later |
| 60 | [OpenMetadata](https://open-metadata.org/) | Metadata, governance, discovery, and lineage | Platform | 🟣 Later |

**[⬆ back to top](#contents)**

## Classical ML and Deep Learning Foundations

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 61 | [PyTorch](https://pytorch.org/) | Deep-learning model training | Framework | 🟢 Now |
| 62 | [TensorFlow](https://www.tensorflow.org/) | Model training and deployment | Framework | 🟡 Evaluate |
| 63 | [JAX](https://jax.readthedocs.io/) | High-performance numerical computing and ML | Framework | 🟡 Evaluate |
| 64 | [scikit-learn](https://scikit-learn.org/) | Classical ML and preprocessing | Framework | 🟢 Now |
| 65 | [XGBoost](https://xgboost.readthedocs.io/) | Gradient-boosted models for tabular data | Framework | 🟢 Now |
| 66 | [LightGBM](https://lightgbm.readthedocs.io/) | Efficient gradient boosting | Framework | 🟢 Now |
| 67 | [CatBoost](https://catboost.ai/) | Gradient boosting with categorical features | Framework | 🟢 Now |
| 68 | [Keras](https://keras.io/) | High-level deep-learning API | Framework | 🟢 Now |
| 69 | [fastai](https://www.fast.ai/) | Practical deep-learning training | Framework | 🟢 Now |
| 70 | [statsmodels](https://www.statsmodels.org/) | Statistical models and inference | Framework | 🟢 Now |
| 71 | [Prophet](https://facebook.github.io/prophet/) | Time-series forecasting | Framework | 🟡 Evaluate |
| 72 | [RAPIDS](https://rapids.ai/) | GPU-accelerated data science | Framework | 🟣 Later |

**[⬆ back to top](#contents)**

## Fine-Tuning, Alignment, and Distributed Training

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 73 | [Transformers](https://huggingface.co/docs/transformers/) | Use and fine-tune language, vision, and audio models | Framework | 🟢 Now |
| 74 | [TRL](https://huggingface.co/docs/trl/) | Transformer reinforcement learning and alignment | Framework | 🟡 Evaluate |
| 75 | [Unsloth](https://unsloth.ai/) | Memory-efficient LLM fine-tuning | Framework | 🟡 Evaluate |
| 76 | [Axolotl](https://github.com/axolotl-ai-cloud/axolotl) | Configuration-driven LLM fine-tuning | Tool | 🟡 Evaluate |
| 77 | [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory) | Fine-tune and align language models | Tool | 🟡 Evaluate |
| 78 | [PEFT](https://huggingface.co/docs/peft/) | Parameter-efficient fine-tuning | Framework | 🟢 Now |
| 79 | [DeepSpeed](https://www.deepspeed.ai/) | Distributed and memory-efficient training | Framework | 🟣 Later |
| 80 | [Composer](https://github.com/mosaicml/composer) | Efficient neural-network training methods | Framework | 🟡 Evaluate |
| 81 | [OpenRLHF](https://github.com/OpenRLHF/OpenRLHF) | RLHF and preference-training workflows | Framework | 🟣 Later |
| 82 | [LitGPT](https://github.com/Lightning-AI/litgpt) | Train and fine-tune language models | Framework | 🟡 Evaluate |
| 83 | [torchtune](https://pytorch.org/torchtune/) | PyTorch-native LLM fine-tuning | Framework | 🟡 Evaluate |
| 84 | [Colossal-AI](https://www.colossalai.org/) | Distributed training and inference | Framework | 🟣 Later |

**[⬆ back to top](#contents)**

## Experiment Tracking, MLOps, and Pipelines

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 85 | [MLflow](https://mlflow.org/) | Experiment tracking, model registry, and AI lifecycle | Platform | 🟢 Now |
| 86 | [Kubeflow](https://www.kubeflow.org/) | Kubernetes ML pipelines and training | Platform | 🟣 Later |
| 87 | [ClearML](https://clear.ml/) | Experiment management and ML orchestration | Platform | 🟡 Evaluate |
| 88 | [Metaflow](https://metaflow.org/) | Reproducible data-science workflows | Platform | 🟡 Evaluate |
| 89 | [Dagster](https://dagster.io/) | Data and asset-oriented pipelines | Platform | 🟡 Evaluate |
| 90 | [Apache Airflow](https://airflow.apache.org/) | Scheduled data and ML pipelines | Platform | 🟢 Now (when needed) |
| 91 | [Flyte](https://flyte.org/) | Reproducible scalable workflow orchestration | Platform | 🟣 Later |
| 92 | [ZenML](https://www.zenml.io/) | MLOps framework connecting experiments and deployment | Framework | 🟡 Evaluate |
| 93 | [Polyaxon](https://polyaxon.com/) | ML experimentation and orchestration | Platform | 🟣 Later |
| 94 | [Feast](https://feast.dev/) | Feature store for training and online inference | Platform | 🟣 Later |
| 95 | [Aim](https://aimstack.io/) | Open-source experiment tracking | Platform | 🟢 Now |
| 96 | [TensorBoard](https://www.tensorflow.org/tensorboard) | Training metrics and model visualization | Application | 🟢 Now |

**[⬆ back to top](#contents)**

## Model Serving and Inference Optimization

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 97 | [KServe](https://kserve.github.io/website/) | Kubernetes-native model serving | Platform | 🟣 Later |
| 98 | [Seldon Core](https://www.seldon.io/solutions/open-source-projects/core) | Model deployment and inference graphs | Platform | 🟣 Later |
| 99 | [BentoML](https://www.bentoml.com/) | Package and deploy models as APIs | Platform | 🟢 Now |
| 100 | [Ray Serve](https://docs.ray.io/en/latest/serve/) | Distributed model and Python service serving | Platform | 🟣 Later |
| 101 | [NVIDIA Triton](https://developer.nvidia.com/triton-inference-server) | Multi-framework GPU model serving | Server | 🔵 Production |
| 102 | [MLServer](https://mlserver.org/) | Standardized model inference server | Server | 🟡 Evaluate |
| 103 | [TorchServe](https://pytorch.org/serve/) | PyTorch model serving | Server | 🟡 Evaluate |
| 104 | [TorchX](https://pytorch.org/torchx/) | Distributed ML job launching | Framework | 🟣 Later |
| 105 | [OpenVINO](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) | Inference optimization across hardware | Runtime | 🟡 Evaluate |
| 106 | [ONNX Runtime](https://onnxruntime.ai/) | Cross-platform model inference | Runtime | 🟢 Now |
| 107 | [Apache TVM](https://tvm.apache.org/) | Compiler stack for ML deployment | Framework | 🟣 Later |
| 108 | [TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM) | Optimized NVIDIA LLM inference | Runtime | 🔵 Production |

**[⬆ back to top](#contents)**

## AI Evaluation, Tracing, Safety, and Observability

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 109 | [Langfuse](https://langfuse.com/) | LLM traces, prompts, evaluations, experiments, and cost | Platform | 🟢 Now |
| 110 | [Phoenix](https://phoenix.arize.com/) | LLM tracing and evaluation | Platform | 🟢 Now |
| 111 | [Promptfoo](https://www.promptfoo.dev/) | Prompt/model tests and red teaming | Tool | 🟢 Now |
| 112 | [Ragas](https://docs.ragas.io/) | RAG evaluation metrics and test sets | Framework | 🟢 Now |
| 113 | [DeepEval](https://deepeval.com/) | LLM testing and evaluation | Framework | 🟡 Evaluate |
| 114 | [Evidently](https://www.evidentlyai.com/) | Data quality, drift, and ML monitoring | Platform | 🟡 Evaluate |
| 115 | [TruLens](https://www.trulens.org/) | Evaluate and trace LLM applications | Framework | 🟡 Evaluate |
| 116 | [Giskard](https://www.giskard.ai/) | Test ML/LLM models for quality and risk | Platform | 🟡 Evaluate |
| 117 | [OpenLLMetry](https://github.com/traceloop/openllmetry) | OpenTelemetry instrumentation for LLM apps | Framework | 🟢 Now |
| 118 | [Agenta](https://agenta.ai/) | Prompt experimentation, evaluation, and tracing | Platform | 🟡 Evaluate |
| 119 | [Helicone](https://www.helicone.ai/) | LLM observability, logging, and cost tracking | Platform | 🟡 Evaluate |
| 120 | [NeMo Guardrails](https://github.com/NVIDIA/NeMo-Guardrails) | Programmable conversational guardrails | Framework | 🟡 Evaluate |

**[⬆ back to top](#contents)**

## Voice, Speech, and Audio AI

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 121 | [Pipecat](https://github.com/pipecat-ai/pipecat) | Real-time voice and multimodal conversational agents | Framework | 🟢 Now |
| 122 | [LiveKit Agents](https://livekit.io/agents) | Real-time voice and multimodal agents over WebRTC | Platform | 🟡 Evaluate |
| 123 | [Vocode](https://vocode.dev/) | Voice-based conversational applications | Framework | 🟡 Evaluate |
| 124 | [Whisper](https://github.com/openai/whisper) | Speech-to-text transcription | Model/tool | 🟢 Now |
| 125 | [faster-whisper](https://github.com/SYSTRAN/faster-whisper) | Efficient Whisper inference | Model/tool | 🟢 Now |
| 126 | [Vosk](https://alphacephei.com/vosk/) | Offline speech recognition | Runtime | 🟡 Evaluate |
| 127 | [Piper](https://github.com/rhasspy/piper) | Local text-to-speech | Runtime | 🟡 Evaluate |
| 128 | [Silero](https://github.com/snakers4/silero-models) | Speech and voice-activity models | Model/tool | 🟡 Evaluate |
| 129 | [Coqui TTS](https://github.com/coqui-ai/TTS) | Text-to-speech and voice-model tooling | Framework | 🟡 Evaluate |
| 130 | [OpenVoice](https://github.com/myshell-ai/OpenVoice) | Voice cloning and controllable speech | Model/tool | 🟡 Evaluate |
| 131 | [Kokoro](https://github.com/hexgrad/kokoro) | Lightweight open text-to-speech model | Model/tool | 🟡 Evaluate |
| 132 | [SpeechBrain](https://speechbrain.github.io/) | Speech and audio research toolkit | Framework | 🟡 Evaluate |

**[⬆ back to top](#contents)**

## Computer Vision, OCR, Documents, and Multimodal AI

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 133 | [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR) | OCR and document extraction | Toolkit | 🟢 Now |
| 134 | [Tesseract](https://github.com/tesseract-ocr/tesseract) | Open-source OCR engine | Engine | 🟢 Now |
| 135 | [docTR](https://mindee.github.io/doctr/) | Deep-learning document text recognition | Framework | 🟡 Evaluate |
| 136 | [Surya](https://github.com/datalab-to/surya) | OCR, layout analysis, and reading order | Toolkit | 🟡 Evaluate |
| 137 | [Marker](https://github.com/datalab-to/marker) | Convert PDFs and documents to structured Markdown | Toolkit | 🟢 Now |
| 138 | [Unstructured](https://unstructured.io/) | Document parsing and ingestion pipelines | Platform | 🟢 Now |
| 139 | [LayoutLM](https://huggingface.co/docs/transformers/model_doc/layoutlm) | Document understanding models | Framework/model | 🟡 Evaluate |
| 140 | [Detectron2](https://github.com/facebookresearch/detectron2) | Computer-vision detection and segmentation | Framework | 🟡 Evaluate |
| 141 | [Ultralytics YOLO](https://github.com/ultralytics/ultralytics) | Real-time object detection and vision models | Framework | 🟢 Now ⚠️ License check |
| 142 | [OpenCV](https://opencv.org/) | Computer vision and image processing | Framework | 🟢 Now |
| 143 | [MMDetection](https://github.com/open-mmlab/mmdetection) | OpenMMLab detection toolbox | Framework | 🟡 Evaluate |
| 144 | [GroundingDINO](https://github.com/IDEA-Research/GroundingDINO) | Open-vocabulary object detection | Model/tool | 🟡 Evaluate |

**[⬆ back to top](#contents)**

## Synthetic Data, Privacy, Governance, and AI Security

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 145 | [SDV](https://sdv.dev/) | Synthetic tabular, relational, and time-series data | Framework | 🟡 Evaluate |
| 146 | [Synthea](https://synthetichealth.github.io/synthea/) | Synthetic patient data generation | Application | 🟡 Evaluate |
| 147 | [ydata-synthetic](https://github.com/ydataai/ydata-synthetic) | Synthetic data generation methods | Framework | 🟡 Evaluate |
| 148 | [Synthcity](https://github.com/vanderschaarlab/synthcity) | Synthetic data and privacy research | Framework | 🟡 Evaluate |
| 149 | [Twinify](https://github.com/computationalprivacy/twinify) | Privacy-preserving synthetic data | Framework | 🟡 Evaluate |
| 150 | [SmartNoise](https://smartnoise.org/) | Differential privacy tooling | Platform | 🟣 Later |
| 151 | [OpenDP](https://opendp.org/) | Differential privacy framework | Framework | 🟣 Later |
| 152 | [Microsoft Presidio](https://microsoft.github.io/presidio/) | PII detection and anonymization | Platform | 🟢 Now |
| 153 | [garak](https://github.com/NVIDIA/garak) | LLM vulnerability scanning | Tool | 🟢 Now |
| 154 | [LLM Guard](https://llm-guard.com/) | Input/output scanners for LLM security | Framework | 🟡 Evaluate |
| 155 | [Guardrails AI](https://www.guardrailsai.com/) | Validation and safety guardrails | Framework | 🟡 Evaluate |
| 156 | [DeepTeam](https://www.confident-ai.com/deepteam) | LLM red teaming and safety testing | Tool | 🟡 Evaluate |

**[⬆ back to top](#contents)**

## Git, CI/CD, Kubernetes, and AI Infrastructure

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 157 | [Docker](https://www.docker.com/) | Reproducible packaging for models and services | Infrastructure | 🟢 Now |
| 158 | [Podman](https://podman.io/) | Daemonless OCI container workflows | Infrastructure | 🟡 Evaluate |
| 159 | [GitLab](https://about.gitlab.com/) | Git hosting, CI/CD, registry, and security pipelines | Platform | 🟢 Now |
| 160 | [Forgejo](https://forgejo.org/) | Lightweight self-hosted Git forge | Platform | 🟢 Now |
| 161 | [Woodpecker CI](https://woodpecker-ci.org/) | Open-source container-based CI/CD | Platform | 🟢 Now |
| 162 | [Jenkins](https://www.jenkins.io/) | Extensible build, test, and release automation | Platform | 🟡 Evaluate |
| 163 | [Argo CD](https://argo-cd.readthedocs.io/) | GitOps continuous delivery for Kubernetes | Platform | 🟣 Later |
| 164 | [K3s](https://k3s.io/) | Lightweight Kubernetes for cloud VMs and edge | Platform | 🟣 Later |
| 165 | [OpenTofu](https://opentofu.org/) | Infrastructure as code for AWS, Azure, and GCP | Infrastructure | 🟢 Now |
| 166 | [MinIO](https://min.io/) | S3-compatible model and dataset object storage | Infrastructure | 🟡 Evaluate |
| 167 | [JupyterHub](https://jupyter.org/hub) | Multi-user notebook environments | Platform | 🟢 Now (teams) |
| 168 | [NVIDIA GPU Operator](https://docs.nvidia.com/datacenter/cloud-native/gpu-operator/latest/) | GPU drivers and workloads in Kubernetes | Platform | 🟣 Later |

**[⬆ back to top](#contents)**

## Productization, AI Operations, and Platform Integration

| # | Tool | What it helps with | Type | Stage |
|---:|---|---|---|---|
| 169 | [Supabase](https://supabase.com/) | Application database, Auth, APIs, Storage, and Realtime | Platform | 🟢 Now |
| 170 | [Appwrite](https://appwrite.io/) | Backend services for Auth, Storage, Functions, and Realtime | Platform | 🟢 Now (alternative) |
| 171 | [LiteLLM](https://www.litellm.ai/) | Unified model gateway, routing, budgets, and fallbacks | Platform | 🟢 Now |
| 172 | [n8n](https://n8n.io/) | Visual integration and AI workflow automation | Platform | 🟢 Now ⚠️ License check |
| 173 | [Novu](https://novu.co/) | Notification workflows for AI products and SaaS | Platform | 🟢 Now |
| 174 | [PostHog](https://posthog.com/) | Product analytics, experiments, and feature flags | Platform | 🟢 Now |
| 175 | [Chatwoot](https://www.chatwoot.com/) | Customer support and omnichannel conversations | Platform | 🟢 Now |
| 176 | [Libredesk](https://github.com/abhinavxd/libredesk) | Lightweight self-hosted support desk | Application | 🟢 Now |
| 177 | [listmonk](https://listmonk.app/) | Self-hosted newsletters and mailing lists | Application | 🟢 Now |
| 178 | [Formbricks](https://formbricks.com/) | Surveys, feedback, and product research | Platform | 🟢 Now |
| 179 | [Appsmith](https://www.appsmith.com/) | Internal tools and admin panels | Platform | 🟢 Now |
| 180 | [OpenTelemetry](https://opentelemetry.io/) | Vendor-neutral traces, metrics, and logs | Standard/tooling | 🟢 Now |

**[⬆ back to top](#contents)**

---

## MVP-to-Production Paths

### 1. Private Document Chatbot

Start with [Open WebUI](https://openwebui.com/), [Dify](https://dify.ai/), or a small [LlamaIndex](https://www.llamaindex.ai/)/[Haystack](https://haystack.deepset.ai/) service; use [pgvector](https://github.com/pgvector/pgvector) or [Qdrant](https://qdrant.tech/); use [Ollama](https://ollama.com/) or a hosted model; record traces with [Langfuse](https://langfuse.com/); and create a small [Promptfoo](https://www.promptfoo.dev/) or [Ragas](https://docs.ragas.io/) evaluation set. This is enough for a useful document assistant without Kubeflow or a large agent platform.

### 2. Customer-Support Assistant

Use [Libredesk](https://github.com/abhinavxd/libredesk) or [Chatwoot](https://www.chatwoot.com/) for the human support surface, [Rasa](https://rasa.com/)/[Dify](https://dify.ai/)/[LangChain](https://www.langchain.com/) for the assistant, a retrieval system for product documentation, a model gateway for routing, and explicit escalation to a human. Store tenant, user, conversation, tool, and consent metadata. Do not let a support agent issue refunds or change account data without server-side authorization and confirmation.

### 3. Voice Agent

Use [LiveKit](https://livekit.io/agents) or [Pipecat](https://github.com/pipecat-ai/pipecat) for realtime transport, [Whisper](https://github.com/openai/whisper) or [faster-whisper](https://github.com/SYSTRAN/faster-whisper) for speech-to-text, an LLM gateway for reasoning, [Piper](https://github.com/rhasspy/piper) or a hosted TTS provider for speech, and [Langfuse](https://langfuse.com/)/[OpenTelemetry](https://opentelemetry.io/) for tracing. Add interruption handling, timeouts, call recording policy, and human handoff before calling it production-ready.

### 4. Classical ML Product

Use pandas or DuckDB for data preparation, [scikit-learn](https://scikit-learn.org/)/[XGBoost](https://xgboost.readthedocs.io/)/[LightGBM](https://lightgbm.readthedocs.io/)/[CatBoost](https://catboost.ai/) for a baseline, [DVC](https://dvc.org/) for data and model versioning, [MLflow](https://mlflow.org/) for experiments, [Great Expectations](https://greatexpectations.io/) for data checks, and [BentoML](https://www.bentoml.com/) or a small API for serving. This path is usually cheaper and easier to operate than fine-tuning a large language model.

### 5. Fine-Tuned Language Model

Use [Transformers](https://huggingface.co/docs/transformers/), Datasets, [PEFT](https://huggingface.co/docs/peft/), [Unsloth](https://unsloth.ai/)/[Axolotl](https://github.com/axolotl-ai-cloud/axolotl) or [torchtune](https://pytorch.org/torchtune/), [DVC](https://dvc.org/), [MLflow](https://mlflow.org/), a held-out evaluation set, and a GPU runner. Confirm data rights and model-license compatibility before training or redistributing the result. Serve with [vLLM](https://vllm.ai/), [BentoML](https://www.bentoml.com/), [SGLang](https://github.com/sgl-project/sglang), or another inference server only after measuring the workload.

### 6. Production MLOps

Use Git, [DVC](https://dvc.org/), object storage, [MLflow](https://mlflow.org/), a CI system, containerized training, [OpenTelemetry](https://opentelemetry.io/), a model server, and a rollback procedure. Add [Kubeflow](https://www.kubeflow.org/), [Flyte](https://flyte.org/), [KServe](https://kserve.github.io/website/), [Feast](https://feast.dev/), [K3s](https://k3s.io/), GPU Operator, or a feature store only when reproducibility, multi-user scheduling, or scale demands them.

**[⬆ back to top](#contents)**

## Git-Connected AI Development Loop

A practical team loop is:

1. Store application code, prompts, evaluation cases, and pipeline definitions in Git.
2. Store large datasets and model artifacts in DVC-backed object storage rather than ordinary Git history.
3. Run formatting, unit tests, data checks, prompt tests, security scans, and a small evaluation suite in CI.
4. Record the commit, dataset version, model version, configuration, hardware, metrics, latency, and cost for each meaningful run.
5. Build a versioned container and deploy it to a development environment.
6. Review traces, failures, user feedback, and evaluation regressions.
7. Promote through a feature flag or approval gate, then keep rollback artifacts available.

This loop is often more valuable than starting with a large MLOps platform.

**[⬆ back to top](#contents)**

## AWS and Azure Migration

A self-hosted AI system can move to AWS or Azure when its containers, artifacts, data, secrets, and operational configuration are portable. The migration includes more than application images.

| Concern | Portable Boundary | AWS Examples | Azure Examples |
|---|---|---|---|
| Model API | `ModelGateway` or `InferenceService` | ECS/EKS, EC2 GPU, Batch, SageMaker endpoint | Container Apps/AKS, GPU VM, Batch, Azure ML endpoint |
| Dataset/model artifacts | DVC plus `ArtifactStore` | S3, EFS, FSx | Blob Storage, Azure Files |
| Experiment tracking | MLflow API and artifact store | S3/RDS/EC2 | Blob/PostgreSQL/VM |
| Vector search | Qdrant/pgvector/OpenSearch interface | EC2/EKS/OpenSearch | AKS/VM/Azure AI Search adapter |
| Training | Containerized entrypoint | EC2 GPU, Batch, EKS | GPU VM, Batch, AKS |
| Secrets | Environment-independent secret interface | Secrets Manager/SSM | Key Vault |
| CI/CD | Git and container pipeline | GitLab Runner, ECS/EKS | GitLab Runner, Container Apps/AKS |
| Observability | OpenTelemetry | CloudWatch or self-hosted backends | Azure Monitor or self-hosted backends |
| Infrastructure | OpenTofu modules | AWS provider | Azure provider |

Keep provider-specific SDKs at the infrastructure edge. Do not spread AWS or Azure types through product, model, or training modules. Model weights, prompts, evaluation data, vector indexes, and secrets all need an export and restore plan.

**[⬆ back to top](#contents)**

## AI/ML Production Checklist

A model or agent is not production-ready merely because it returns good answers in a notebook. Establish:

- [ ] Data provenance and permission checks
- [ ] Tenant isolation
- [ ] Input validation and output validation
- [ ] Rate limits, timeouts, and cost budgets
- [ ] Prompt-injection defenses
- [ ] Human escalation paths
- [ ] Structured logs, traces, and metrics
- [ ] Backup procedures and rollback artifacts

Additional checks by domain:

- **Agents** — restrict tool permissions and validate every tool argument.
- **RAG** — retain source references and measure retrieval quality.
- **Voice systems** — test interruption, silence, accents, latency, recordings, and handoff.
- **Classical ML** — monitor drift and label quality.
- **All AI systems** — define what happens when the model is unavailable or wrong.

> ⚠️ Review the current license and commercial terms of every tool and every model before using it in a customer-facing SaaS, agency template, managed service, or white-label product.

**[⬆ back to top](#contents)**

## Contributing

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first. This list follows the [awesome-lint](https://github.com/sindresorhus/awesome-lint) format — one PR per addition, alphabetized within a category where practical, no self-promotion without disclosure.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related or neighboring rights to this work. See [LICENSE](LICENSE) for details.
