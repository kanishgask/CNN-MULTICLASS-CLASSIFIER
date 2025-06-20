# CNN-MULTICLASS-CLASSIFIER
🧠 CNN Multiclass Image Classifier
A Convolutional Neural Network (CNN) implemented in Python using TensorFlow/Keras to classify images into multiple categories. This example uses the CIFAR-10 dataset, but it can be easily adapted to any custom image dataset.

**📂 Project Structure**
graphql
Copy
Edit
cnn-multiclass-classifier/
├── cnn_classifier.py       # Main CNN model training script
├── README.md               # Project documentation
└── requirements.txt        # Python dependencies
**🚀 Features**
Convolutional Neural Network built with TensorFlow/Keras

Multiclass classification with Softmax output

Trained on CIFAR-10 (can be replaced with a custom dataset)

Dropout for regularization

Simple and easy to adapt

**✅ Requirements**
Python 3.7 – 3.11

TensorFlow 2.x

NumPy

**🛠️ Installation**
1. Clone the repository
bash
Copy
Edit
git clone https://github.com/yourusername/cnn-multiclass-classifier.git
cd cnn-multiclass-classifier
2. Create a virtual environment (optional but recommended)
bash
Copy
Edit
python3 -m venv venv
source venv/bin/activate      # Windows: venv\Scripts\activate
3. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
Or manually:

bash
Copy
Edit
pip install tensorflow numpy
🧪 Run the Classifier
bash
Copy
Edit
python cnn_classifier.py
The model will train on the CIFAR-10 dataset for 10 epochs and evaluate accuracy on the test set.

🖼️ Custom Dataset (Optional)
To use your own dataset:

Organize your images like this:

kotlin
Copy
Edit
data/
├── class1/
│   ├── img1.jpg
│   ├── img2.jpg
├── class2/
│   ├── img1.jpg
│   ├── img2.jpg
Replace the dataset loading part in the script with:

python
Copy
Edit
from tensorflow.keras.utils import image_dataset_from_directory

dataset = image_dataset_from_directory(
    "data",
    image_size=(32, 32),
    batch_size=32,
    label_mode='categorical'  # for one-hot encoded labels
)
📈 Example Output:
![image](https://github.com/user-attachments/assets/c20f36ae-c402-42e4-b914-7d3842a6ea9d)

