<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=24,20,15&height=140&section=header&text=Sai%20Krishna&fontSize=42&fontColor=ffffff&fontAlignY=55&desc=CS%20%40%20VIT%20Chennai%20%C2%B7%20Building%20things%20that%20think&descSize=14&descAlignY=75&descColor=a0a0b0" width="100%"/>
</div>

<br/>

Hey — I'm a second-year CS student who spends most of his time trying to make small models punch above their weight. Lately that means RL post-training, inference-time memory, and figuring out what's actually possible on a laptop GPU.

I like problems where the constraint is the interesting part.

<br/>

---

### What I'm building

**[Qwen3-0.6B Reasoning Pipeline](https://github.com/Skrisps26)**
&nbsp;·&nbsp; *active*

Training a 0.6B model to reason using a 4-stage GRPO pipeline — SFT coldstart, RL on math, mode fusion, then generalization. At inference I attach a Hopfield episodic memory bank (~20MB) that retrieves similar past problems as context. The bet is that a sub-1B model with the right inference-time setup can match 7B+ on reasoning benchmarks.

<br/>

**[PowerBench-Consumer](https://github.com/Skrisps26/powerbench)**
&nbsp;·&nbsp; *complete*

Benchmarked LLM inference and GRPO training on an RTX 2050 (4GB VRAM) — extending DREAM:Lab's Jetson Orin AGX methodology to hardware most people actually own. The interesting finding: INT8 is 3× slower than FP16 on consumer GPUs, the opposite of what happens on the Jetson. Quantization benefits don't travel across hardware architectures.

```
FP16  →  2,407ms  ·  13.29 tok/s  ·  PPL 14.80
INT8  →  10,056ms ·  3.18  tok/s  ·  PPL 19.46
INT4  →  3,965ms  ·  8.07  tok/s  ·  PPL 15.36
```

<br/>

**[Neural Global Illumination Engine](https://github.com/Skrisps26)**
&nbsp;·&nbsp; *complete*

Reframed Global Illumination as a regression task — an MLP learns to predict radiance instead of ray-tracing it. Brought per-frame compute from 26ms down to 11ms with a +4.1dB PSNR improvement. Runs at 60+ FPS with dynamic lighting and moving occluders.

<br/>

**[Deepfake Detector](https://github.com/Skrisps26)**
&nbsp;·&nbsp; *complete*

Multimodal detection pipeline across video and audio. 85%+ accuracy, processes 10K+ frames and audio samples per batch in under 3 seconds.

<br/>

---

### A few things I've picked up

```python
{
  "research":  ["PyTorch", "GRPO", "QLoRA", "TRL", "HuggingFace Transformers"],
  "cv / edge": ["OpenCV", "TFLite", "YOLO", "Taichi CUDA"],
  "backend":   ["FastAPI", "Node.js", "Express", "MongoDB", "PostgreSQL"],
  "cloud":     ["AWS Lambda", "Bedrock", "S3", "DynamoDB", "Step Functions"],
  "languages": ["Python", "C", "C++", "JavaScript", "Go"],
}
```

<br/>

---

### Recognition

Qualcomm Edge AI Hackathon 2025 — Finalist &nbsp;·&nbsp; top teams from 2000+ participants  
DevsHouse '25 — MongoDB Track Winner &nbsp;·&nbsp; 4th overall

<br/>

---

<div align="center">

<img height="155" src="https://github-readme-stats.vercel.app/api?username=Skrisps26&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&rank_icon=github&hide_title=true"/>
&nbsp;&nbsp;
<img height="155" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Skrisps26&layout=compact&theme=tokyonight&hide_border=true&langs_count=5&hide_title=true"/>

</div>

<br/>

<div align="center">
<a href="https://linkedin.com/in/saik26">LinkedIn</a>
&nbsp;·&nbsp;
<a href="mailto:saikris.dev@gmail.com">saikris.dev@gmail.com</a>
</div>

<br/>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=24,20,15&height=80&section=footer" width="100%"/>
</div>
