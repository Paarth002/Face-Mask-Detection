# Face-Mask-Detection

This model checks if a person is wearing face-mask or not.  <br>
It detects faces using OpenCV. <br/>
Classification is done using Deep-Learning Model.<br/>
The model contains Tensorflow-Keras and CNN Layers.<br/>

The dataset used to train the model contains 12,000 images. <br/>
Link to the dataset: https://www.kaggle.com/ashishjangra27/face-mask-12k-images-dataset <br/>

Check the presentation "IITISOC - Bhore Parth Shirish.pptx" for more details. <br/>

This TensorFlow face mask detection model has been deployed using a Podman Docker image and Flask API. To run the Podman image on your Windows local machine, follow the steps below:

1. Install Podman on your local machine. Download and install the [MSI file](https://github.com/containers/podman/releases/download/v4.4.0/podman-v4.4.0.msi) from the 'Assets' section of the latest version of Podman. 
2. After you have installed Podman, create a new virtual machine that runs the Podman container engine by entering this command in your Windows PowerShell: `podman machine init`.
3. Start the virtual machine by running this command: `podman machine start`.
4. Pull the Podman image from GitHub Packages by running the following command: `podman pull ghcr.io/atharva-mohite/fmd:1`. The size of this image is 1.79 GB.
5. Run the Podman container using the following command: `podman run -p 8080:5000 ghcr.io/atharva-mohite/fmd:1`.
6. You should be able to access the API by visiting http://localhost:8080 in your web browser.
7. You can remove the image using the command: `podman rmi ghcr.io/atharva-mohite/fmd:1` or `podman rmi --force ghcr.io/atharva-mohite/fmd:1`.

<p align="center">
  Examples
  <img src="face.jpeg" width="100%" title="1">
</p><br/>
