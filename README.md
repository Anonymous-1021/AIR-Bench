# AIR-Bench: Benchmarking Large Audio-Language Models via Generative Comprehension
official repository of [AIR-Bench: Benchmarking Large Audio-Language Models via Generative Comprehension](https://arxiv.org/pdf/2402.07729.pdf)

<p align="center">
    <br>
    <img src="Evaluation_Framework.pdf" width="750"/>
    <br>
</p>

# Download Benchmark

# Easy Evaluation
## Step1: Evaluate on Foundation Benchmark
### Inference your model on Foundation Benchmark
`python Inference_Foundation.py`
### [Optional] Alignment on Foundation Benmark
This is an optional step. This situation applies when your model cannot accurately answer ABCD and needs to be aligned with GPT.
We provide a script that can batch call GPT, you only need to do one thing: replace your own GPT call keys (MIT_SPIDER_TOKEN and MIT_SPIDER_URL).

`python align_in_foundation.py`

### Calculate score on Foundation Benchmark
`python score_foundation.py`

## Step2: Evaluate on Chat Benchmark
### Inference your model on Chat Benchmark
`python Inference_Chat.py`
### Calculate score on Chat Benchmark
`python score_chat.py`
