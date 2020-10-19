This is the demo page for [Semi-supervised Many-to-many Music Timbre Transfer](https://github.com/sumfish/music-style-transfer)

## Abstract
Inspired by the success in voice conversion, the concept of music timbre transfer is considered in the task of transforming the style of a music clip while preserving the semantic content. However, the many-to-many timbre transfer between different instruments remains an under-explored area. 

In this work, we investigate many-to-many transfer based on an autoencoder framework, which comprises two pretrained encoders and one decoder trained in an unsupervised manner. To learn more representative features for encoders, we produced a parallel dataset, called the MI-Para, synthesized from MIDI files and digital audio workstations (DAW). 

Evaluation results showed the effectiveness of the proposed framework. To scale up the application scenario, we also demonstrated that our model can achieve style transfer by training in a semi-supervised manner with a smaller parallel dataset.

-------
## Dataset
[The parallel dataset]()

The MIDI files of 21 pop and cartoon songs (total 2700 seconds) are collected from [Bitmidi](https://bitmidi.com/). Then the parallel dataset is synthesized from these MIDI files and digital audio workstation (DAW). Each song in the dataset is played by four kinds of instruments, including piano, acoustic guitar, electric guitar, and bass.

-------
## Demo
There are four kinds of instruments in the MI-Para dataset, so we conducted twelve transfer tasks between different kinds of instruments in our experiment.

### Piano to Acoustic Guitar

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/piano_10.mp3" controls preload></audio> | <audio src="Res_demopage/target/ag.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/p2ag_10_2.mp3" controls preload></audio> | <audio src="Res_demopage/semi/p2ag_10_2.wav" controls preload></audio> |

### Piano to Electric Guitar

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/piano_04.mp3" controls preload></audio> | <audio src="Res_demopage/target/eg.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/p2eg_04_2.mp3" controls preload></audio> | <audio src="Res_demopage/semi/p2eg_04_2.wav" controls preload></audio> |

### Piano to Bass

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/piano_09.mp3" controls preload></audio> | <audio src="Res_demopage/target/bass.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/p2bass_09_2.mp3" controls preload></audio> | <audio src="Res_demopage/semi/p2bass_09_2.wav" controls preload></audio> |

### Acoustic Guitar to Piano

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/ag_10.mp3" controls preload></audio> | <audio src="Res_demopage/target/ag.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/ag2p_10_2.mp3" controls preload></audio> | <audio src="Res_demopage/semi/ag2p_10_2.wav" controls preload></audio> |

### Acoustic Guitar to Electric Guitar

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/ag_10.mp3" controls preload></audio> | <audio src="Res_demopage/target/eg.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/ag2eg_10_2.mp3" controls preload></audio> | <audio src="Res_demopage/semi/ag2eg_10_2.wav" controls preload></audio> |

### Acoustic Guitar to Bass

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/ag_09.mp3" controls preload></audio> | <audio src="Res_demopage/target/bass.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/ag2bass_09_2.mp3" controls preload></audio> | <audio src="Res_demopage/semi/ag2bass_09_2.wav" controls preload></audio> |

### Electric Guitar to Piano

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/eg_04.mp3" controls preload></audio> | <audio src="Res_demopage/target/piano.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/eg2p_04_2.mp3" controls preload></audio> | <audio src="Res_demopage/semi/eg2p_04_2.wav" controls preload></audio> |

### Electric Guitar to Acoustic Guitar

### Electric Guitar to Bass

### Bass to Piano

### Bass to Acoustic Guitar

### Bass to Electric Guitar
