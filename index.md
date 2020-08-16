This is the demo page for [Semi-supervised Many-to-many Music Timbre Transfer](https://github.com/sumfish/music-style-transfer)

## Abstract
Inspired by the success in voice conversion, the concept of music timbre transfer is considered as to transform the style of the music clip to a target clip while preserving the semantic content of the music. Even the concept has been commonly used in music transfer, the many-to-many timbre transfer between different instruments still remain under-explored area. In this work, we investigate the possibility of many-to-many music timbre transfer based on an autoencoder framework, which is composed of two pre-trained encoder and one decoder trained in an unsupervised manner. To learn more representative features in the pre-trained content and style encoder, we produce a parallel dataset synthesized from MIDI files and digital audio workstation (DAW). 

We evaluates the content preservation and the success of style transfer in both objective and subjective manners. In addition to the performance measurement, we also demonstrate that on the basis of state-of-the-art Triplet network, the content encoder is able to learn meaningful content representations with the collected parallel dataset, which has no manually labelled annotations of music content.

-------
## Demo
There are four kinds of instruments in our datasets, so we conducted twelve transfer tasks between different kinds of instruments in our experiment.

### Piano to Acoustic Guitar

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/piano_10.mp3" controls preload></audio> | <audio src="Res_demopage/target/ag.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/p2ag_10_2.mp3" controls preload></audio> |

### Piano to Electric Guitar

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/piano_04.mp3" controls preload></audio> | <audio src="Res_demopage/target/eg.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/p2eg_04_2.mp3" controls preload></audio> |

### Piano to Bass

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/piano_09.mp3" controls preload></audio> | <audio src="Res_demopage/target/bass.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/p2bass_09_2.mp3" controls preload></audio> |

### Acoustic Guitar to Piano

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/ag_10.mp3" controls preload></audio> | <audio src="Res_demopage/target/ag.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/ag2p_10_2.mp3" controls preload></audio> |

### Acoustic Guitar to Electric Guitar

Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/ag_10.mp3" controls preload></audio> | <audio src="Res_demopage/target/eg.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/ag2eg_10_2.mp3" controls preload></audio> |

### Acoustic Guitar to Bass
Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/ag_09.mp3" controls preload></audio> | <audio src="Res_demopage/target/bass.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/ag2bass_09_2.mp3" controls preload></audio> |

### Electric Guitar to Piano
Source | Target | 
------------ | ------------- | 
<audio src="Res_demopage/source/eg_04.mp3" controls preload></audio> | <audio src="Res_demopage/target/piano.mp3" controls preload></audio> |

Ours - Baseline | Ours - Semi | 
------------- | ------------- |
<audio src="Res_demopage/base/eg2p_04_2.mp3" controls preload></audio> |

### Electric Guitar to Acoustic Guitar

### Electric Guitar to Bass

### Bass to Piano

### Bass to Acoustic Guitar

### Bass to Electric Guitar
