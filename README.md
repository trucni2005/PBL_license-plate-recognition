<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>License Plate Recognition System</title>
</head>

<body>

    <h1>License Plate Recognition System</h1>

    <h2>Overview 🚗</h2>
    <p>
        This is a license plate recognition system built using YOLOv5. It is designed to detect and read license plates in images or videos. The system utilizes a pre-trained YOLOv5 model (<code>best.pt</code>) to perform object detection, followed by image processing steps to crop characters and perform binary comparisons for character recognition.
    </p>

    <h2>Prerequisites 🛠️</h2>
    <ul>
        <li>Python 3.10.0</li>
        <li>torch 1.13.1+cpu</li>
        <li>opencv-python</li>
        <li>numpy</li>
        <li>pandas</li>
    </ul>

    <h2>Installation ⚙️</h2>
    <p>
        To install the required packages, run the following command:
    </p>
    <pre><code>pip install torch opencv-python numpy pandas</code></pre>

    <h2>Usage 📸</h2>
    <ol>
        <li>Clone the repository:
            <pre><code>git clone https://github.com/trucni2005/PBL_license-plate-recognition.git
cd pulse</code></pre>
        </li>
        <li>Load the YOLOv5 model:
            <pre><code>import torch

model = torch.hub.load('ultralytics/yolov5', 'custom', path='weights/best.pt')</code></pre>
        </li>
        <li>Use Pulse to read license plates from images or video streams:
            <pre><code># Example: Read license plate from an image
image_path = 'path/to/image.jpg'
result = readPlate(cv2.imread(image_path), model)

# Example: Evaluate and test the system on a dataset
test_result_csv = 'test_set/predicted_testset_output.csv'
evaluate(test_result_csv, 'test_set/true_output.csv')</code></pre>
        </li>
    </ol>

    <h2>Features 🌟</h2>
    <ul>
        <li>License plate detection using YOLOv5.</li>
        <li>Character recognition for reading license plates.</li>
        <li>Support for both single-line and two-line license plates.</li>
    </ul>

    <h2>Kết Quả Kiểm Thử Mới 📊</h2>
<p>Trong quá trình kiểm thử trên {{489}} ảnh, chúng ta có được các kết quả sau:</p>

<ul>
    <li>Tỉ lệ không thể nhận diện biển số: {{0.00}}%</li>
    <li>Tỉ lệ đọc sai biển số: {{5.32}}%</li>
    <li>Tỉ lệ đọc thiếu chữ số: {{1.84}}%</li>
    <li>Tỉ lệ biển số đọc đúng: {{92.84}}%</li>
</ul>

</body>

</html>
