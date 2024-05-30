# XR-based-Dyslexia-Friendly-Text-Detector
An XR based dyslexia reader that converts the text into an OpenDyslexic font through text detection using google vision API


## Dyslexia-Friendly Text Detection with Animation

The purpose of this project is to provide a way for dyslexic users to more easily interact with the world around them. This project leverages Unity and the Google Cloud Vision API to detect text from the environment and present it in a dyslexia-friendly font with an animated effect. 

## The Problem

### What is Dyslexia?

Dyslexia is a specific learning difficulty affecting the acquisition of fluent and accurate reading and spelling skills, affecting approximately 10% of the population. People with dyslexia encounter difficulties with spelling, writing, reading aloud, and determining the correct pronunciation of written words, despite not being impaired in other aspects of their learning.

### Problem Statement

People with dyslexia find it hard to interact with and read text in the world around them. This project aims to provide a solution for people with dyslexia to interact with any text around them using a smartphone.

## Our Solution

Our solution intends to present dyslexic users with a more accessible environment by allowing them to use their smartphone to alter the presentation of words and sentences in their environment. Users will be able to read text at a glance using a device that is always on their person. We will achieve this by changing the font of the detected text to a dyslexia-friendly font such as OpenDyslexic and applying animation to the text.

## Scope

The minimum scope for this project includes:

1. Design an app that detects and changes the font of words in the environment.
2. Delivery of a working prototype that achieves the above brief.
3. Final hand-over of the app ready for use, with a high standard of code that is easily extensible.

An extended scope for this project includes:

1. Colour-coding of vowels and syllables to aid pronunciation of new words.
2. The ability to change the background to allow for easier interpretation of the words.
3. Opt-in text-to-speech capabilities for recognized text.

## Prerequisites

You will need:

* Unity version `2020.1` or higher
* A Google Cloud project with the Vision API enabled
* An API key for the Google Cloud Vision API
* A dyslexia-friendly font (e.g., OpenDyslexic)
* An Android or iOS device capable of running the app

### Packages

In the project, we utilized various Unity packages. Ensure you have the necessary dependencies installed to build the project with Unity.

## Setup Instructions

### Google Cloud Vision API

1. Create a project on the [Google Cloud Console](https://console.cloud.google.com/).
2. Enable the Vision API for your project.
3. Create an API key for accessing the Vision API.
4. Note down the API key.

### Unity Project

1. Clone this repository or download the project files.
2. Open the project in Unity.
3. Import a dyslexia-friendly font (e.g., OpenDyslexic) into your Unity project.
4. Add the font to a `Fonts` folder within the `Assets` directory.
5. In the Unity Editor, select the `Main Camera` GameObject.
6. In the Inspector, find the `WebCamTextureToCloudVision` component.
7. Set the following fields in the component:
   - `Api Key`: Your Google Cloud Vision API key.
   - `Dyslexia Font`: The imported dyslexia-friendly font.
   - `Response Text`: The UI Text element for displaying the detected text.
   - `Response Array`: The UI Text element for displaying the text split into lines.
   - `Res Panel`: The UI Panel containing the text elements.
8. Save your scene.

### Running the Project

1. Play the scene in the Unity Editor.
2. The application will start capturing images from the webcam.
3. Detected text will be displayed on the UI with the dyslexia-readable font and animation.
   ![Running Scene](img/running_scene.png)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [Google Cloud Vision API](https://cloud.google.com/vision)
- [OpenDyslexic Font](https://opendyslexic.org/)
