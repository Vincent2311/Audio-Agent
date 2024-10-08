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

We introduce Audio-Agent, a multimodal framework for audio generation, editing and composition based on text or video inputs. Conventional approaches for text-to-audio (TTA) tasks often make single-pass inferences from text descriptions. While straightforward, this design struggles to produce high-quality audio when given complex text conditions. In our method, we utilize a pre-trained TTA diffusion network as the audio generation agent to work in tandem with GPT-4, which decomposes the text condition into atomic, specific instructions, and calls the agent for audio generation. Consequently, Audio-Agent generates high-quality audio that is closely aligned with the provided text or video while also supporting variable-length generation. For video-to-audio (VTA) tasks, most existing methods require training a timestamp detector to synchronize video events with generated audio, a process that can be tedious and time-consuming. We propose a simpler approach by fine-tuning a pre-trained Large Language Model (LLM), e.g., Gemma2-2B-it, to obtain both semantic and temporal conditions to bridge video and audio modality. Thus our framework provides a comprehensive solution for both TTA and VTA tasks without substantial computational overhead in training.

## Samples
See index.html. The index.html file can be opened by Googol Chrome and render a static website.

All the files in assets/TTA are labeled from 1 to 17 with the same order. The captions for TTA can be found in assets/TTA/caption.csv. 

We additional provide long audio examples with assets/TTA/caption_20s.csv

All the files in assets/VTA are labeled from 1 to 6 with the same order. The inference audio result has been combined with the video input(muted) for clearer evaluation


We will release codes and details upon the acceptance of the paper 