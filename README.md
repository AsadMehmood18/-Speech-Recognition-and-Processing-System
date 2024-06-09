# Voice-Controlled Speech Recognition and Processing System 🎙🔊

This project involves the implementation of a speech recognition and audio processing system using MATLAB. The system can record audio, apply various audio effects, transcribe speech using the wav2vec2 model, and even open applications using voice commands.

## Table of Contents
- [Introduction](#introduction)
- [Requirements](#requirements)
- [Setup](#setup)
- [Usage](#usage)
- [Features](#features)
- [Project Image](#project-image)
- [Acknowledgments](#acknowledgments)

## Introduction
This project demonstrates a MATLAB app for recording audio, applying audio effects such as pitch modulation and echo, transcribing the recorded speech, and executing voice commands to open applications. The app provides a user-friendly interface to visualize and manipulate audio signals. The transcription functionality is powered by the wav2vec2 model, a state-of-the-art speech recognition model developed by Facebook AI.

## Requirements
- MATLAB R2023a or later
- Audio Toolbox
- Signal Processing Toolbox

## Setup
1. **Download and Unzip wav2vec2 Model:**
    ```matlab
    downloadFile = matlab.internal.examples.downloadSupportFile("audio","wav2vec2/wav2vec2-base-960.zip");
    % Change the working directory to the directory of this code
    wav2vecLocation = fullfile(path of file directory, "wav2vec");
    unzip(downloadFile, wav2vecLocation)
    addpath(wav2vecLocation)
    ```

2. **Initialize the App:**
    The main MATLAB script initializes the app, creates UI elements, and sets up the callbacks for various controls.

## Usage
1. **Launch the App:**
    Run the main script to launch the app. The app interface includes panels for initial and transformed voice, buttons for recording and processing audio, and controls for adjusting line width and color of the plots.

2. **Record Audio:**
    Click the "Record" button to start recording audio. The recording duration can be adjusted using the duration spinner.

3. **Apply Audio Effects:**
    Use the "High Pitch," "Low Pitch," and "Echo" buttons to apply the corresponding audio effects to the recorded audio.

4. **Open Applications:**
    Use voice commands to open applications such as Word, Excel, Paint, and more. Simply say the name of the application to open it.

5. **Replay Audio:**
    Replay the recorded or processed audio using the "Replay" buttons in the respective panels.

## Features
- **Recording:** Record audio using the built-in microphone.
- **Pitch Modulation:** Increase or decrease the pitch of the recorded audio.
- **Echo Effect:** Apply an echo effect to the recorded audio.
- **Visualization:** Visualize the recorded and processed audio signals.
- **Transcription:** Transcribe the recorded audio using the wav2vec2 model, a cutting-edge speech recognition model.
- **Application Opening:** Open applications using voice commands.

## Project Image
![Project Image](path/to/your/project/image.png)
> Replace `path/to/your/project/image.png` with the actual path to your project image.

## Acknowledgments
This project was developed by Asad Mehmood and Mahroona Mariam. Special thanks to the MATLAB community and the developers of the wav2vec2 model for providing the necessary resources and support.

