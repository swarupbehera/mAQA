# mAQA
This repository contains data and codes for our Interspeech 2023 Paper: [Towards Multi-Lingual Audio Question Answering](https://www.isca-speech.org/archive/pdfs/interspeech_2023/behera23_interspeech.pdf).

## Data: mClothoAQA
- The primary challenge for multi-lingual AQA is obtaining high-quality labeled data. To tackle this issue, we developed the mClothoAQA dataset, a multi-lingual AQA dataset.
- We accomplished this by translating questions and answers from the ClothoAQA dataset into seven additional languages. The languages included are French (fr), Hindi (hi), German (de), Spanish (es), Italian (it), Dutch (nl), and Portuguese (pt).
- The mClothoAQA dataset contains a total of 1991 audio files. Each language variant consists of 35838 question-answer pairs.

###  Downloading the Clotho-AQA dataset
- Download the clotho-AQA dataset from https://zenodo.org/record/6473207.
- Extract the zip file and place the audio files in `dataset/audio_files/` directory.

### Multi-lingual mClothoAQA QA Files
- Copy the csv files for 8 languages from `mClothoAQA' directory to `metadata/` directory.

##  Feature Extraction
- Utilize the openL3 open source Python library for calculating deep audio embeddings. Install openL3 via `pip install openl3`.
- Execute the `extract_features.py` script.
- Upon completion, locate the stored deep audio embeddings at `dataset/features`.
