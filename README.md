# SpeechEE

## SpeechEE: A Novel Benchmark for Speech Event Extraction

## ACMMM 2024 Submission


## Requirements

General

- Python (verified on 3.9)
- CUDA (verified on 11.8)

Python Packages

- see requirements.txt

```bash
conda create -n speechee python=3.9
conda activate speechee
pip install -r requirements.txt
```


## Data Structure
```
data
├── PHEE_subtype
│   ├── audio
│   │   ├── train
│   │   │   ├── train-0.wav
│   │   │   ├── ...
│   │   ├── dev
│   │   │   ├── dev-0.wav
│   │   │   ├── ...
│   │   ├── test
│   │   │   ├── test-0.wav
│   │   │   ├── ...
│   ├── event.schema
│   ├── train.json
│   ├── val.json
│   ├── test.json
├── ...
```


## Running SpeechEE

The command for training is as follows:

```bash
nohup bash run.bash -d 0 -f tree -m t5-large --label_smoothing 0 -l 5e-5 --lr_scheduler linear --warmup_steps 2000 -b 16 -i PHEE_subtype
```

- `-d` refers to the GPU device id.
- `-m t5-large` refers to using T5-large as the textual decoder.
- `-i` refers to the dataset.
