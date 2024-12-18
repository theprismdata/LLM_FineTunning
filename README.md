# LLM FineTunning

Environment
Python 3.10
torch 2.5.1
cuda version : cu124
Howto run

## Method 1 Local 환경
Docker 사용
```
docker run -it --gpus all -p 8888:8888 -v .\:/workspace --name pytorch-llm-finetunning hongjoong/pytorch-llm-finetunning:latest
```
CONTAINER에서 Jupyter notebook 실행
```commandline
==========
== CUDA ==
==========

CUDA Version 12.4.1

Container image Copyright (c) 2016-2023, NVIDIA CORPORATION & AFFILIATES. All rights reserved.

This container image and its contents are governed by the NVIDIA Deep Learning Container License.
By pulling and using the container, you accept the terms and conditions of this license:
https://developer.nvidia.com/ngc/nvidia-deep-learning-container-license

A copy of this license is made available in this container at /NGC-DL-CONTAINER-LICENSE for your convenience.
root@671e6fe7dde8:/workspace# jupyter notebook --ip=0.0.0.0 --port=8888 --allow-root
```

#### Case 1 FineTunning Llama3 with KDI Dataset
docker에서
```commandline
KDI-Llama3-FineTunning-OPDS-Colab.ipynb
```
#### Case 2 FineTunning Qwen2-0.5B with KDI Dataset
KDI-Qwen2-FineTunning-OPDS.ipynb

#### Case 3 Inference Qwen2-0.5B KDI 2014 Model
KDI-QWen2-inference.ipynb

#### Case 4 Inference Llama3 KDI 2014 Model
KDI-sLLM-Inference.ipynb

## Method 2 Colab 환경
Colab에서
```commandline
KDI-Llama3-FineTunning-OPDS-Colab.ipynb
```

#### model download 
huggingface-cli download unsloth/llama-3-8b-bnb-4bit   --local-dir unsloth/llama-3-8b-bnb-4bit
