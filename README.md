# VIoTGPT
Code of AAAI2025 Paper [《VIoTGPT: Learning to Schedule Vision Tools in LLMs towards Intelligent Video Internet of Things》](https://arxiv.org/abs/2312.00401). 

Video Internet of Things (VIoT) has shown full potential in collecting an unprecedented volume of video data. How to schedule the domain-specific perceiving models and analyze the collected videos uniformly, efficiently, and especially intelligently to accomplish complicated tasks is challenging. To address the challenge, we build VIoTGPT, the framework based on LLMs to correctly interact with humans, query knowledge videos, and invoke vision models to analyze multimedia data collaboratively. To support VIoTGPT and related future works, we meticulously crafted the VIoT-Tool dataset, including the training dataset and the benchmark involving 11 representative vision models across three categories based on semi-automatic annotations. To guide LLM to act as the intelligent agent towards intelligent VIoT, we resort to the ReAct instruction tuning method based on VIoT-Tool to learn the tool capability. Quantitative and qualitative experiments and analyses demonstrate the effectiveness of VIoTGPT. We believe VIoTGPT contributes to improving human-centered experiences in VIoT applications. 

### VIoTGPT 
Download the pre-trained LLama-2-7b and Vicuna-7b, then download the LoRA weights from the following links.
1. [LLama-lora](https://drive.google.com/drive/folders/10kY7uuAH4XqVKTALK3jjy4VnUYzTaVZJ?usp=sharing).
2. [Vicuna-lora](https://drive.google.com/drive/folders/10eF7fMXktVJZ30kdyVjuPUluAnJsw5o6?usp=sharing).

### VToT-Tool dataset
1. [training](https://drive.google.com/file/d/10ZTkusnE5OjzUgi7JsD6JeY-nkRluSx9/view?usp=sharing). 
2. [testing](https://drive.google.com/file/d/1kRWQYpzX4XS5Nz-NAFhCy5N-V8Xa1mUa/view?usp=sharing), copy it to "./VIoT_tool"

### Environment
```
torch==2.0.1
transformers==4.31.0
deepspeed==0.10.0
langchain==0.0.101
gradio==3.23.0
```
### Train and Test
1. Train
```
cd train
train_vicuna.sh
```
2. Test
```
test_vicuna.sh 
```

## Citation
```
@inproceedings{zhong2025VIoTGPT,
  title={VIoTGPT: Learning to Schedule Vision Tools in LLMs towards Intelligent Video Internet of Things},
  author={Zhong, Yaoyao and Qi, Mengshi and Wang, Rui and Qiu, Yuhan and Zhang, Yang and Ma, Huadong},
  booktitle={AAAI},
  year={2025}
}
```
