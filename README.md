<!DOCTYPE html>
<html lang="en">
<body>

  <h1>License Plate Recognition System - README</h1>
  <h2>Overview 🚗</h2>
  <p>
        This is a license plate recognition system built using YOLOv5. It is designed to detect and read license plates in images or videos. The system utilizes a pre-trained YOLOv5 model (best.pt) to perform object detection, followed by image processing steps to crop characters and perform binary comparisons for character recognition.
    </p>
    <h2>Prerequisites 🛠️</h2>
    <ul>
        <li>Python 3.10.0</li>
        <li>torch 1.13.1+cpu</li>
        <li>opencv-python</li>
        <li>numpy</li>
        <li>pandas</li>
    </ul>
    <h2>Features 🌟</h2>
    <ul>
        <li>License plate detection using YOLOv5.</li>
        <li>Character recognition for reading license plates.</li>
        <li>Support for both single-line and two-line license plates.</li>
    </ul>
    <h2>New Test Results 📊</h2>
    <p>During testing on 489 images, the following results were obtained:</p>
    <ul>
        <li>Correctly read license plates: 92.84%</li>
        <li>Unable to detect license plates: 0.00%</li>
        <li>Incorrectly read license plates: 5.32%</li>
        <li>Missing digits in license plates: 1.84%</li>
    </ul>
  
</body>

</html>
