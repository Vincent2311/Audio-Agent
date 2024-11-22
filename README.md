<h1 align="center">Audio-Agent: Leveraging LLMs For Audio Generation, Editing and Composition</h1>
<div align="center">
  <span class="author-block">
    Zixuan Wang<sup>1</sup>,</span>
  <span class="author-block">
    Yu-Wing Tai<sup>2</sup>,</span>
  <span class="author-block">
    Chi-Keung Tang<sup>1</sup>,</span>
</div>
<div align="center">
  <span class="author-block"><sup>1</sup>HKUST,</span>
  <span class="author-block"><sup>2</sup>Dartmouth College</span>
</div>

[![arXiv](https://img.shields.io/badge/arXiv-2405.16136-brightgreen.svg?style=flat-square)](https://arxiv.org/abs/2410.03335)  

## Abstract

We introduce Audio-Agent, a multimodal framework for audio generation, editing and composition based on text or video inputs. Conventional approaches for text-to-audio (TTA) tasks often make single-pass inferences from text descriptions. While straightforward, this design struggles to produce high-quality audio when given complex text conditions. In our method, we utilize a pre-trained TTA diffusion network as the audio generation agent to work in tandem with GPT-4, which decomposes the text condition into atomic, specific instructions and calls the agent for audio generation. In doing so, Audio-Agent can generate high-quality audio that is closely aligned with the provided text or video exhibiting complex and multiple events, while supporting variable-length and variable-volume generation. For video-to-audio (VTA) tasks, most existing methods require training a timestamp detector to synchronize video events with the generated audio, a process that can be tedious and time-consuming. Instead, we propose a simpler approach by fine-tuning a pre-trained Large Language Model (LLM), e.g., Gemma2-2B-it, to obtain both semantic and temporal conditions that bridge the video and audio modality. Consequently, our framework contributes a comprehensive solution for both TTA and VTA tasks without substantial computational overhead in training.

We will release codes and details upon the acceptance of the paper. Thanks for understanding 
