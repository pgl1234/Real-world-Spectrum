# Real-world Spectrum Dataset 
## Title
Robust Spectrum Prediction With Deep 3D Pyramid Vision Transformer Learning

## Dataset 
This paper uses three spectrum datasets collected in the real world, including frequency-modulated (FM) spectrum dataset, long-term evolution (LTE) spectrum dataset, and cross-validation spectrum dataset, to prove the effectiveness of the proposed methods.  
The datasets are collected at the Jungjun Road Campus of Nanjing University of Aeronautics and Astronautics (NUAA) in Nanjing, China. You can obtain all datasets from [Google Drive](https://drive.google.com/drive/folders/1w2kTaRKVRmsO5jUAovZc78W_eTQ63TDm?usp=sharing). Specific details about these three datasets are as follows:

.<div align=center><img src="Spectrum-sensor-map/sensor-map.png" width="300" height="360" /></div>
<p align="center">  
 Figure 1. Spectrum sensor map.
</p>

### A. FM Spectrum Dataset
The FM dataset is collected by a spectrum collection sensor located at [118.7905 (east longitude), 31.9378 (northern latitude), 12.10 (altitude)] on the Jiangjun Road campus of the NUAA in Nanjing, China (see Figure 1 node 1). The data was collected over a bandwidth of 90-110 MHz, with data types being I and Q path signals. The collection time was from 17:20 on Sep. 23rd, 2022, to 20:20 on Sep. 23rd, 2022, with a sampling interval of 1s. 

We convert the FM I/Q data collected every second to a spectrogram via the STFT. The configurations are: the sampling frequency is 125 MHz, the descending sampling coefficient is 4, the STFT number is 32508, the center frequency of the FM is 99 MHz, and the length-window is 256. These spectrograms constitute the FM dataset. We split the spectrogram series into the training set (7200 samples with 17:20-19:20), validation set (1800 samples with 19:20-19:50), and test set (1800 samples with 19:50-20:20) with a 4:1:1 ratio in chronological order.

This dataset is used to demonstrate the superiority of the proposed methods over the baseline methods.

### B. LTE Spectrum Dataset
The LTE dataset was collected by a spectrum collection node located at [118.7905 (east longitude), 31.9378 (northern latitude), 12.10 (altitude)] on the Jiangjun Road campus of the NUAA in Nanjing, China (see Figure 1 node 1). The data was collected over a bandwidth of 690-710 MHz, with data types being I and Q path signals. The collection time was from 17:20 on Sep. 23rd, 2022, to 20:20 on Sep. 23rd, 2022, with a sampling interval of 1s. 

We convert the LTE I/Q data collected every second to a spectrogram via the STFT. The configurations are: the sampling frequency is 125 MHz, the descending sampling coefficient is 4, the STFT number is 32508, the center frequency of the LTE is 700 MHz, and the length-window is 256. These spectrograms constitute the LTE dataset. We split the spectrogram series into the training set (7200 samples with 17:20-19:20), validation set (1800 samples with 19:20-19:50), and test set (1800 samples with 19:50-20:20) with a 4:1:1 ratio in chronological order.

This dataset is used to demonstrate the transfer learning performance of the proposed method.

### C. Cross-Validation Spectrum Dataset
The cross-validation dataset (select FM band) is collected by a spectrum collection node located at [118.7907 (east longitude), 31.9386 (northern latitude), 36.80 (altitude)] on the Jiangjun Road campus of the NUAA in Nanjing, China (see Fig. 1 node 1). The data was collected over a bandwidth of 690-710 MHz, with data types being I and Q path signals. The collection time was from 22:14 on Jul. 10, 2024, to 00:04 on Jul. 11, 2024, with a sampling interval of 1s. 

We convert the FM I/Q data collected every second to a spectrogram via the STFT. The configurations are: the sampling frequency is 125 MHz, the descending sampling coefficient is 4, the STFT number is 32508, the center frequency of the FM is 99 MHz, and the length-window is 256. These spectrograms constitute the LTE dataset. We split the spectrogram series into the training set (7200 samples with 17:20-19:20), validation set (1800 samples with 19:20-19:50), and test set (1800 samples with 19:50-20:20) with a 4:1:1 ratio in chronological order.

This dataset is used to cross-validate the superiority of the proposed methods over the baseline methods.

## Dataset
If you find this repo useful, please cite our paper.
