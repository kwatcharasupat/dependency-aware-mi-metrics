**Metrics from this work is now part of [Latte](https://github.com/karnwatcharasupat/latte)! Please take a look there for a tested and cross-framework implementation.**

----

# Evaluation of Latent Space Disentanglement in the Presence of Interdependent Attributes
Supplementary materials for ISMIR 2021 LBD submission:

> K. N. Watcharasupat and A. Lerch, "Evaluation of Latent Space Disentanglement in the Presence of Interdependent Attributes," submitted to the Late-Breaking Demo Session of the 22nd International Society for Music Information Retrieval Conference (ISMIR), Online, 2021. [[arXiv]](https://arxiv.org/abs/2110.05587)

## Data
- NSynth: https://magenta.tensorflow.org/datasets/nsynth
- AudioCommons Timbral Models: https://github.com/AudioCommons/timbral_models

## Model
<img width=50% src=model.png/>

## Training and hyperparameters
- `Adam(lr=1e-4, weight_decay=1e-6)`
- `ReduceLROnPlateau(factor=0.75, patience=3)`
- `stft(n_fft=1024,
	hop_length=128,
	window=hann_window
	center=True,
	pad_mode="constant",
	normalized=True)
`

## Results
<img src=results.png>

## How to Cite
```
@article{watcharasupat2021metrics,
	title        = {Evaluation of Latent Space Disentanglement in the Presence of Interdependent Attributes},
	author       = {Karn N. Watcharasupat and Alexander Lerch},
	year         = 2021,
	month        = 11,
	booktitle    = {submitted to the Extended Abstracts for the Late-Breaking Demo Session of the 22nd International Society for Music Information Retrieval Conference},
	location     = {Online},
	publisher    = {ISMIR}
}
```
