# AgriBotanica

# TinyML Plant Agents

Edge classifier for plant states + agentic triage/RAG on host.

## Architecture
- TinyML on MCU (TFLite Micro int8): image -> label + confidence
- Host agents: triage (route by confidence), RAG (3-step actionable advice), actions/logs

## Quick start
- `training/train.py` → baseline model
- `training/quantize.py` → int8 TFLite
- `firmware/` → TFLM inference on board
- `host/cli.py` → run triage + RAG locally

## Milestones
See GitHub issues labeled `epic`.
