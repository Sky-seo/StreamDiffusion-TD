# StreamDiffusion-TD
2) python@3.11 설치
brew install python@3.11


설치 끝나고:
python3.11 --version

2️⃣ 새 venv311 만들고 그걸로만 작업하기

이제 진짜로 StreamDiffusion용 깨끗한 환경을 만들자.

cd "/Users/seohaneul/Desktop/Fall25/StreamDiffusion/StreamDiffusion"
python3.11 -m venv venv311
source venv311/bin/activate


그 다음 확인:

python --version
which python


예상 출력:

Python 3.11.x
/Users/seohaneul/Desktop/Fall25/StreamDiffusion/StreamDiffusion/venv311/bin/python


이렇게 나오면 이제부터는 3.13이랑 완전히 분리된 상태야.

3️⃣ venv311 안에서 기본 세팅
python -m pip install --upgrade pip setuptools wheel


그리고 StreamDiffusion 요구 버전에 맞게:

pip install "diffusers==0.24.0"
pip install "streamdiffusion==0.1.1"


필요하다면 나중에:

pip install "transformers==4.35.0" "huggingface-hub<1.0,>=0.34.0" "accelerate==0.25.0"
