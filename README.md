# Transfer Learning and Few-Shot Learning for Deepfake Detection based on AST and ConvNeXt
This project explores deepfake speech detection using two state-of-the-art models: ConvNeXt and the Audio Spectrogram Transformer (AST). We conducted a comprehensive study across multiple fine-tuning strategies; full, partial, linear probing, few-shot, and adapter-based tuning, using the ASVspoof 2019 Logical Access dataset.
We also evaluated model performance under low-resource conditions, tackled class imbalance, and experimented with ensemble methods to boost detection accuracy.

### Achivements

* **Best single-model result**: AST with partial tuning and weighted loss achieved an **Equal Error Rate (EER) of 0.0620**
* **Adapter-based tuning**: Competitive EER of **0.0722** while training <1% of parameters
* **Few-shot tuning**: ConvNeXt-Tiny performed better than AST when trained on only 20 samples
* **Best overall**: Ensemble of AST models reached **EER of 0.0543**

### Methods

* Input: log-Mel spectrograms
* Models: ConvNeXt-Tiny and AST (ViT-based)
* Dataset: [ASVspoof2019 LA](https://www.asvspoof.org/index2019.html)
* Frameworks: PyTorch, HuggingFace `transformers`, `timm`, `librosa`

### Full Report

[Read the full report]()

### Disclaimer

> **Note:** This project was completed as part of the *Computational Linguistics: Phonetics Team Lab* course at the **University of Stuttgart**, in collaboration with **Alba Prados Moya** and **Nan Ye**. It is shared here for educational and portfolio purposes only. Please do not reuse the work for coursework or academic submissions.


