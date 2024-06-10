# PROJECT-COMPUTER-SCIENCE-PROJECT

Requirements

Processor

	•	Minimum: AMD x86 or any Intel - 64 bit processor
	•	Recommended: Any Intel or AMD processor with at least 8 logical cores (logical CPUs) and hyperthreading capability. Preferably Intel i5 8th gen equivalent or above.

Disk

	•	Minimum: 3 GB of HDD for Anaconda distribution and at least 50 GB to store training and testing data chunk-wise.
	•	Recommended: 300 GB free space to store entire data. Having an SSD is an advantage.

RAM

	•	Minimum: 8 GB DDR4 RAM
	•	Recommended: 8 - 16 GB DDR4 RAM or 8 GB DDR5 RAM

Graphics Processing Unit (GPU)

	•	GPU acceleration or having a GPU makes computation very fast.
	•	GPU support is an added advantage.
	•	4 GB of graphics card is more than enough.

Software Requirements

	•	Python: Version 3.6 or higher

Installation Steps

	1.	Install Anaconda: Download and install Anaconda from here.
	2.	Create a Conda Environment:

conda create -n deepfake_detection python=3.8
conda activate deepfake_detection


	3.	Install Required Libraries:

pip install tensorflow keras opencv-python scikit-learn matplotlib nltk seaborn


	4.	Download NLTK Data:

import nltk
nltk.download('punkt')



Project Structure

	•	train: Directory containing training videos.
	•	metadata.json: Metadata file with labels for the videos.
	•	deepfake_detection.py: Main script to load data, build models, train, and evaluate the model.

Running the Project

	1.	Clone the Repository:

git clone <repository_url>
cd <repository_directory>


	2.	Prepare Data:
	•	Ensure your training videos are in the train directory.
	•	Ensure the metadata.json file is correctly placed in the root directory.
	3.	Run the Script:

python deepfake_detection.py

Additional Notes

	•	Ensure you have the correct paths for video_dir and metadata_file.
	•	Adjust the hyperparameters (e.g., num_frames, epochs, batch_size) as needed for your specific use case and computational resources.

By following these steps, you should be able to run the code, train your model on the provided video data, and visualize the results using a confusion matrix and accuracy/loss plots.
