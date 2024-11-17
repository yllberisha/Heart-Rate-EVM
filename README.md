# Heart Rate EVM

Heart Rate EVM (Eulerian Video Magnification) is a real-time heart rate monitor that uses Eulerian Video Magnification techniques to amplify subtle color changes in facial skin. These changes correlate with blood flow, enabling heart rate detection using a standard webcam.

## Features
- **Real-time BPM Calculation**: Detect and display beats per minute (BPM) directly on the screen.
- **Color Magnification**: Amplifies subtle color variations to highlight blood flow patterns.
- **Face Detection**: Focuses on the detected face region for accurate results.
- **Live Visualization**: Displays processed video with overlaid BPM and FPS.

## Performance
- **Customization**: If the FPS in your machine is too high, causing noticeable shifts in BPM calculations, you can modify the code to calculate an average BPM over a 1-second interval or adjust other parameters for improved stability.

## How It Works
1. Captures live video from a webcam.
2. Detects a face and isolates the region of interest.
3. Processes the video using Gaussian pyramids and Fourier transforms.
4. Filters frequencies within the desired range for heart rate detection.
5. Calculates BPM and updates the display.

![HR_EM](https://github.com/user-attachments/assets/45f159f6-2dd2-448a-8768-f66da6fd4ffc)

## Requirements
- Python 3.9
- OpenCV
- NumPy
- cvzone
- [Additional dependencies in `requirements.txt`](#)

## Installation and Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/heart-rate-evm.git
   cd heart-rate-evm

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   
3. Run the application:
   ```bash
   python main.py
   ```

4. Use a webcam and ensure proper lighting for optimal results. Press Q to exit.

## References
This project is based on the Eulerian Video Magnification (EVM) technique developed by MIT. https://people.csail.mit.edu/mrub/evm/

Disclaimer: This application is not a medical device and should not be used for clinical purposes.
