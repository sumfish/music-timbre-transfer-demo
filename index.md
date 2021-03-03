This is the demo page for [Semi-supervised Many-to-many Music Timbre Transfer](https://github.com/sumfish/music-style-transfer)

## Abstract
This work presents a music timbre transfer model that aims to transfer the style of a music clip while preserving the semantic content. Compared to the existing music timbre transfer models, our model can achieve many-to-many timbre transfer between different instruments. 

The proposed method involves only an autoencoder framework, which comprises two pretrained encoders and one decoder trained in an unsupervised manner. To learn more representative features for the encoders, we produced a parallel dataset, called MI-Para, which is synthesized from MIDI files and digital audio workstations (DAW). 

Both the objective and the subjective evaluation results showed the effectiveness of the proposed framework. To scale up the application scenario, we also demonstrate that our model can achieve style transfer by training in a semi-supervised manner with a smaller parallel dataset.

-------
## MI-Para Dataset

The MIDI files of 21 Western pop songs and cartoon songs (total 2700 seconds) are collected from [Bitmidi](https://bitmidi.com/). Then we utilize MIDI files and digital audio workstation (DAW) to synthesize audio files. By doing this, we ensure that the only change between the two audio files is the timbre. Each song in the dataset was played by four kinds of instruments, including piano, acoustic guitar, electric guitar, and bass.

-------
## Demo
There are four kinds of instruments in the MI-Para dataset, so we conducted twelve transfer tasks between different kinds of instruments in our experiment.

### Piano to Acoustic Guitar

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/24_piano.mp3" controls preload></audio> | <audio src="Res_demopage/target/ag.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/p2ag_24_0.mp3" controls preload></audio> | <audio src="Res_demopage/semi/p2ag_24_1.mp3" controls preload></audio> |

### Piano to Electric Guitar

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/24_piano.mp3" controls preload></audio> | <audio src="Res_demopage/target/eg.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/p2eg_24_0.mp3" controls preload></audio> | <audio src="Res_demopage/semi/p2eg_24_1.mp3" controls preload></audio> |

### Piano to Bass

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/piano_09.mp3" controls preload></audio> | <audio src="Res_demopage/target/bass.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/p2bass_09_2.mp3" controls preload></audio> | <audio src="Res_demopage/semi/p2bass_09_2.mp3" controls preload></audio> |

### Acoustic Guitar to Piano

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/24_ag.mp3" controls preload></audio> | <audio src="Res_demopage/target/piano.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/ag2p_24_0.mp3" controls preload></audio> | <audio src="Res_demopage/semi/ag2p_24_1.mp3" controls preload></audio> |

### Acoustic Guitar to Electric Guitar

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/ag_10.mp3" controls preload></audio> | <audio src="Res_demopage/target/eg.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/ag2eg_10_2.mp3" controls preload></audio> | <audio src="Res_demopage/semi/ag2eg_10_2.mp3" controls preload></audio> |

### Acoustic Guitar to Bass

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/22_2ag.mp3" controls preload></audio> | <audio src="Res_demopage/target/bass_09.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/ag2bass_22_b_0.mp3" controls preload></audio> | <audio src="Res_demopage/semi/ag2bass_22_b_1.mp3" controls preload></audio> |

### Electric Guitar to Piano

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/22_eg.mp3" controls preload></audio> | <audio src="Res_demopage/target/piano.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/eg2p_22_0.mp3" controls preload></audio> | <audio src="Res_demopage/semi/eg2p_22_1.mp3" controls preload></audio> |

### Electric Guitar to Acoustic Guitar

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/22_eg.mp3" controls preload></audio> | <audio src="Res_demopage/target/ag.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/eg2ag_22_0.mp3" controls preload></audio> | <audio src="Res_demopage/semi/eg2ag_22_1.mp3" controls preload></audio> |

### Electric Guitar to Bass

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/22_2_eg.mp3" controls preload></audio> | <audio src="Res_demopage/target/bass.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/eg2bass_22_b_0.mp3" controls preload></audio> | <audio src="Res_demopage/semi/eg2bass_22_b_1.mp3" controls preload></audio> |

### Bass to Piano

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/22_bass.mp3" controls preload></audio> | <audio src="Res_demopage/target/piano.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/b2p_22_0.mp3" controls preload></audio> | <audio src="Res_demopage/semi/b2p_22_1.mp3" controls preload></audio> |

### Bass to Acoustic Guitar

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/22_bass.mp3" controls preload></audio> | <audio src="Res_demopage/target/ag.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/b2ag_22_0.mp3" controls preload></audio> | <audio src="Res_demopage/semi/b2ag_22_1.mp3" controls preload></audio> |

### Bass to Electric Guitar

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/22_bass.mp3" controls preload></audio> | <audio src="Res_demopage/target/piano.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/b2eg_22_0.mp3" controls preload></audio> | <audio src="Res_demopage/semi/b2eg_22_1.mp3" controls preload></audio> |
