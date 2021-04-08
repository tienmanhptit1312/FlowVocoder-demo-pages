
# Abstract
Recently, non-autoregressive neural vocoders have provided remarkable performance in generating high-fidelity speech andhave been able to produce synthetic speech in real-time. However, non-autoregressive neural vocoders such as WaveGloware far behind  autoregressive neural vocoders like WaveFlowin terms of modeling audio signals due to their limitation in ex-pressiveness. In addition, though NanoFlow is a state of theart autoregressive neural vocoder that has immensely small parameters, its performance is marginally lower than WaveFlow. Therefore, in this paper, we propose a new type of autore-gressive neural vocoder called FlowVocoder, which has a smallmemory footprint and is able to generate high-fidelity audio inreal-time. Our proposed model improves the expressiveness offlow blocks by operating a mixture of Cumulative DistributionFunction (CDF) for bipartite transformation. Hence, the pro-posed model is capable of modeling waveform signals as wellas WaveFlow, while its memory footprint is much smaller thanWaveFlow. As shown in experiments, FlowVocoder achieves competitive results with baseline methods in terms of both subjective and objective evaluation, also, it is more suitable for real-time text-to-speech applications.


# Synthetic audio conditioned on mel spectrogram

| FlowVocoder | WaveFlow | NanoFlow | WaveGlow | Ground-truth |
|-------------|----------|----------|----------|--------------|
| <audio src="./Neural-Vocoder/FlowVocoder/LJ001-0001.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveFlow/LJ001-0001.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/NanoFlow/LJ001-0001.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveGlow/LJ001-0001.wav_synthesis.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0001.wav" controls preload size=3></audio> |      

| <audio src="./Neural-Vocoder/FlowVocoder/LJ001-0002.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveFlow/LJ001-0002.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/NanoFlow/LJ001-0002.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveGlow/LJ001-0002.wav_synthesis.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0002.wav" controls preload size=3></audio> |  

| <audio src="./Neural-Vocoder/FlowVocoder/LJ001-0003.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveFlow/LJ001-0003.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/NanoFlow/LJ001-0003.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveGlow/LJ001-0003.wav_synthesis.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0003.wav" controls preload size=3></audio> |  

| <audio src="./Neural-Vocoder/FlowVocoder/LJ001-0004.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveFlow/LJ001-0004.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/NanoFlow/LJ001-0004.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveGlow/LJ001-0004.wav_synthesis.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0004.wav" controls preload size=3></audio> |  

| <audio src="./Neural-Vocoder/FlowVocoder/LJ001-0005.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveFlow/LJ001-0005.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/NanoFlow/LJ001-0005.wav" controls preload size=3></audio> | <audio src="./Neural-Vocoder/WaveGlow/LJ001-0005.wav_synthesis.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0005.wav" controls preload size=3></audio> |  


# Text to speech with Tacotron2

| FlowVocoder | WaveFlow | NanoFlow | WaveGlow | Ground-truth |
|-------------|----------|----------|----------|--------------|
| <audio src="./TTS/FlowVocoder/LJ001-0006.wav" controls preload size=3></audio> | <audio src="./TTS/WaveFlow/LJ001-0006.wav" controls preload size=3></audio> | <audio src="./TTS/NanoFlow/LJ001-0006.wav" controls preload size=3></audio> | <audio src="./TTS/WaveGlow/LJ006-0006.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0006.wav" controls preload size=3></audio> |      

| <audio src="./TTS/FlowVocoder/LJ001-0007.wav" controls preload size=3></audio> | <audio src="./TTS/WaveFlow/LJ001-0007.wav" controls preload size=3></audio> | <audio src="./TTS/NanoFlow/LJ001-0007.wav" controls preload size=3></audio> | <audio src="./TTS/WaveGlow/LJ001-0007.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0007.wav" controls preload size=3></audio> |  

| <audio src="./TTS/FlowVocoder/LJ001-0008.wav" controls preload size=3></audio> | <audio src="./TTS/WaveFlow/LJ001-0008.wav" controls preload size=3></audio> | <audio src="./TTS/NanoFlow/LJ001-0008.wav" controls preload size=3></audio> | <audio src="./TTS/WaveGlow/LJ001-0008.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0008.wav" controls preload size=3></audio> |  

| <audio src="./TTS/FlowVocoder/LJ001-0009.wav" controls preload size=3></audio> | <audio src="./TTS/WaveFlow/LJ001-0009.wav" controls preload size=3></audio> | <audio src="./TTS/NanoFlow/LJ001-0009.wav" controls preload size=3></audio> | <audio src="./TTS/WaveGlow/LJ001-0009.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0009.wav" controls preload size=3></audio> |  

| <audio src="./TTS/FlowVocoder/LJ001-0010.wav" controls preload size=3></audio> | <audio src="./TTS/WaveFlow/LJ001-0010.wav" controls preload size=3></audio> | <audio src="./TTS/NanoFlow/LJ001-0010.wav" controls preload size=3></audio> | <audio src="./TTS/WaveGlow/LJ001-0010.wav" controls preload size=3></audio> | <audio src="./Ground-truth/LJ001-0010.wav" controls preload size=3></audio> |  



