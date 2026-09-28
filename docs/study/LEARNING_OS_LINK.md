# LLM-Learning-OS Integration

This repository is the **framework-first execution/lab repository** for the cross-repository LLM training Track.

## Control plane

Canonical orchestration lives in:

- [LLM-Learning-OS PR #4](https://github.com/Xander-Xai/LLM-Learning-OS/pull/4)
- [Dual-Repository LLM Training Track](https://github.com/Xander-Xai/LLM-Learning-OS/blob/feat/link-minimind-mini-qwen/docs/tracks/deep-engineering/llm-training/README.md)
- [Dual-Repository PT/SFT/DPO Project](https://github.com/Xander-Xai/LLM-Learning-OS/blob/feat/link-minimind-mini-qwen/docs/projects/llm-training-dual-repo/README.md)

## This repository owns

Use mini_qwen to study how modern training frameworks package the core mechanisms:

- Qwen-style configuration and randomly initialized causal LM creation;
- Transformers Trainer pretraining flow;
- TRL SFT and completion-only masking;
- TRL DPO;
- Accelerate launch and process orchestration;
- DeepSpeed / ZeRO configuration;
- FlashAttention integration assumptions.

## This repository does not own

Do not turn `docs/study/` into a second Canonical Knowledge base.

- durable concept definitions belong in `LLM-Learning-OS`;
- framework/version-specific traces stay here;
- experiments and debug evidence stay here;
- only validated conclusions are distilled back into the OS;
- missing LoRA/QLoRA/RM/PPO/GRPO/FSDP implementation is treated as an explicit gap, not silently inferred.

## Pairing rule

For shared stages, inspect `Xander-Xai/minimind` first when you need to see **the mechanism directly**, then use mini_qwen to answer **what Transformers / TRL / Accelerate / DeepSpeed automate, hide or standardize**.

The local M00-M17 roadmap remains the execution checklist; LLM-Learning-OS defines the cross-repository outcome, assessment and Stop Rule.
