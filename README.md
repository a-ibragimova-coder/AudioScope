# AudioScope - Day 15

A real-time audio spectrum analyzer that visualizes microphone input using Fast Fourier Transform (FFT).

## Features

- **Real-time Frequency Spectrum**: Displays the audio frequency spectrum on a logarithmic scale.
- **Frequency Band Analysis**: Breaks down the audio into standard frequency bands (Sub-bass, Bass, Low-mid, Mid, High-mid, Treble, Air) with color-coded bars.
- **Peak Frequency Detection**: Identifies and displays the loudest frequency in the current audio chunk.
- **Auto-scaling**: Dynamically adjusts the plot scales based on the audio levels.

## Requirements

- Python 3.x
- PyAudio
- NumPy
- Matplotlib

## Installation

1. Install the required Python packages:

   ```
   pip install pyaudio numpy matplotlib
   ```

2. **System Dependencies for PyAudio**:
   - **macOS**: `brew install portaudio`
   - **Linux**: `sudo apt-get install portaudio19-dev`
   - **Windows**: `pip install pipwin && pipwin install pyaudio`

## Troubleshooting

- If no microphone is found, ensure your audio device is properly connected and not muted.
- For PyAudio installation issues, refer to the system-specific commands above.
- If the visualization is slow, try reducing the `CHUNK` size or `RATE`.
