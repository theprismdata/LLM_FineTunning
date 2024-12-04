# LLM FineTunning

Environment
Python 3.10
torch 2.5.1
cuda version : cu124
Howto run
가상 환경 생성
```commandline
python -m venv .venv 
```
가상 환경에 라이브러리 설치(Windows)
```commandline
.venv\Scripts\activate.bat
```
```commandline
사전 설치
triton 다운로드
https://huggingface.co/Kefasu/triton/blob/main/triton-2.1.0-cp310-cp310-win_amd64.whl

pip install "triton-2.1.0-cp310-cp310-win_amd64.whl"
pip install torch --index-url https://download.pytorch.org/whl/cu124
pip install xformers --index-url https://download.pytorch.org/whl/cu124
pip install "unsloth[cu124-torch251] @ git+https://github.com/unslothai/unsloth.git"
pip install -r requirements.txt
```

#### Case 1 FineTunning Llama3 with KDL Dataset
KDI-Llama3-FineTunning-OPDS.ipynb

#### Case 2 FineTunning Qwen2-0.5B with KDL Dataset
KDI-Qwen2-FineTunning-OPDS.ipynb

#### Case 3 Inference Qwen2-0.5B KDI 2014 Model
KDI-QWen2-inference.ipynb

#### Case 4 Inference Llama3 KDI 2014 Model
KDI-sLLM-Inference.ipynb

Chat GPT 비교

![image](https://github.com/user-attachments/assets/665dc2cd-0468-4393-a225-30935d0ae3b6)


