
# Abstract
Recently, autoregressive neural vocoders have provided remarkable performance in generating high-fidelity speech and have been able to produce synthetic speech in real-time. However, autoregressive neural vocoders such as WaveFlow are capable of modeling waveform signals from mel-spectrogram, its parameters are significant to deploy on edge devices. Though NanoFlow, that has a small number of parameters, is a state-of-the art autoregressive neural vocoder, the performance of NanoFlow is marginally lower than WaveFlow. Therefore, we propose a new type of autoregressive neural vocoder called FlowVocoder, which has a small memory footprint and is able to generate high-fidelity audio in real-time. Our proposed model improves the density estimation of flow blocks by utilizing a mixture of Cumulative Distribution Functions (CDF) for bipartite transformation. Hence, the proposed model is capable of modeling waveform signals, while its memory footprint is much smaller than WaveFlow. As shown in experiments, FlowVocoder achieves competitive results with baseline methods in terms of both subjective and objective evaluation, also, it is more suitable for real-time text-to-speech applications.

# Synthetic audio conditioned on mel spectrogram

| FlowVocoder | WaveFlow | NanoFlow | Ground-truth |
|-------------|----------|----------|--------------|
| <audio src="./Neural-Vocoder/FlowVocoder/LJ001-0001.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveFlow/LJ001-0001.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/NanoFlow/LJ001-0001.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0001.wav" controls preload size=3></audio> |      

| <audio src="./Neural-Vocoder/FlowVocoder/LJ001-0002.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveFlow/LJ001-0002.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/NanoFlow/LJ001-0002.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0002.wav" controls preload size=3></audio> |  

| <audio src="./Neural-Vocoder/FlowVocoder/LJ001-0003.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveFlow/LJ001-0003.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/NanoFlow/LJ001-0003.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0003.wav" controls preload size=3></audio> |  

| <audio src="./Neural-Vocoder/FlowVocoder/LJ001-0004.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveFlow/LJ001-0004.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/NanoFlow/LJ001-0004.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0004.wav" controls preload size=3></audio> |  

| <audio src="./Neural-Vocoder/FlowVocoder/LJ001-0005.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveFlow/LJ001-0005.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/NanoFlow/LJ001-0005.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0005.wav" controls preload size=3></audio> |  


# Text to speech with Tacotron2

| FlowVocoder | WaveFlow | NanoFlow | Ground-truth |
|-------------|----------|----------|--------------|
| <audio src="./TTS/FlowVocoder/LJ001-0006.wav" controls preload size=3></audio> | <audio src="./TTS/WaveFlow/LJ001-0006.wav" controls preload size=3></audio> | <audio src="./TTS/NanoFlow/LJ001-0006.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0006.wav" controls preload size=3></audio> |      

| <audio src="./TTS/FlowVocoder/LJ001-0007.wav" controls preload size=3></audio> | <audio src="./TTS/WaveFlow/LJ001-0007.wav" controls preload size=3></audio> | <audio src="./TTS/NanoFlow/LJ001-0007.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0007.wav" controls preload size=3></audio> |  

| <audio src="./TTS/FlowVocoder/LJ001-0008.wav" controls preload size=3></audio> | <audio src="./TTS/WaveFlow/LJ001-0008.wav" controls preload size=3></audio> | <audio src="./TTS/NanoFlow/LJ001-0008.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0008.wav" controls preload size=3></audio> |  

| <audio src="./TTS/FlowVocoder/LJ001-0009.wav" controls preload size=3></audio> | <audio src="./TTS/WaveFlow/LJ001-0009.wav" controls preload size=3></audio> | <audio src="./TTS/NanoFlow/LJ001-0009.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0009.wav" controls preload size=3></audio> |  

| <audio src="./TTS/FlowVocoder/LJ001-0010.wav" controls preload size=3></audio> | <audio src="./TTS/WaveFlow/LJ001-0010.wav" controls preload size=3></audio> | <audio src="./TTS/NanoFlow/LJ001-0010.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0010.wav" controls preload size=3></audio> |  



