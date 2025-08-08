Pipeline that transforms **human voice** into **instrumental sound** using deep learning models, all implemented in a single jupyter notebook.

## Pipeline Overview

1. **Converts waveform into a time-frequency representation**
   - Tools: librosa, numpy
   - Input: Raw human voice audio, target instrument sounds
   - Output: Mel spectrogram  

3. **Voice-to-Instrument Domain Transformation**  
   - Model: MaskCycleGAN-VC
   - Input: Mel spectrogram of voice  
   - Output: Transformed Mel spectrogram resembling target instrument domain

4. **Waveform Reconstruction**  
   - Model: HiFi-GAN  
   - Input: Instrument-like Mel spectrogram  
   - Output: Audio waveform 
