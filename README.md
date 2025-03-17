# Denoising-Autoencoder-to-remove-noise-in-the-audio

The  code runs on limited Dataset hence the model is overfitting on the dataset. Approximate audio dataset required for the training is 2000 audios and the dataset can also be trained in 500 audio files. 

This repository contains a **Denoising Autoencoder** implemented using Python to remove noise from audio files. It leverages the `librosa` and `noisereduce` libraries to process `.wav` files, reduce background noise, and visualize the results.  

## 📌 Features  

- **Load & process audio files**: Uses `librosa` to read `.wav` files.  
- **Noise reduction**: Applies the `noisereduce` library for audio enhancement.  
- **File renaming**: Replaces spaces in filenames with underscores for consistency.  
- **Waveform & Spectrogram visualization**: Displays before-and-after comparisons.  
- **Audio playback**: Enables listening to the original and denoised audio within the notebook.  

## 🛠️ Installation  

Ensure you have the required dependencies installed:  

```bash
pip install librosa noisereduce soundfile matplotlib numpy
```

If using **Google Colab**, mount Google Drive to access files:  

```python
from google.colab import drive
drive.mount('/content/drive')
```

## 🚀 Usage  

1. **Set the dataset paths** in the notebook (`Denoising_Autoencoder.ipynb`).  
2. **Run the notebook cells** to process `.wav` files in the dataset folder.  
3. **View and compare** the original vs. denoised waveforms & spectrograms.  
4. **Listen to the cleaned audio** to assess improvement.  

## 📊 Visualization  

The notebook includes **waveform and spectrogram plots** for:  

- **Original noisy audio**  
- **Denoised output**  

## 📂 File Structure  

```
📂 Denoising_Autoencoder
 ├── 📜 Denoising_Autoencoder.ipynb  # Jupyter Notebook with the implementation
 ├── 📂 VoiceDataset
 │   ├── 📂 WAV_Files  # Original noisy audio files
 │   ├── 📂 Denoised_WAV  # Processed audio files after noise reduction
```

## 📌 Example Output  

| **Original Audio** | **Denoised Audio** |
|--------------------|--------------------|
| ![Original Waveform](example_waveform.png) | ![Denoised Waveform](denoised_waveform.png) |

## 🏆 Credits  

Developed using:  
- [Librosa](https://librosa.org/) for audio processing  
- [NoiseReduce](https://pypi.org/project/noisereduce/) for noise reduction  
- [Matplotlib](https://matplotlib.org/) for visualization  

---

