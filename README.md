# PlayingCardDetection
Proof of concept: detecting playing cards using OpenCV. Made with love for Procesamiento de Imágenes Digitales.

## Setting up
You will need Python 3 installed (we recommend using the latest version) in your system before running this project.

After downloading and unzipping the project, go into the root folder where requirements.txt is located and type this command in a terminal to install the required dependencies in your Python environment:

```console
pip install -r requirements.txt
```

You are required to open Jupyter notebooks, so most likely you will need an IPython kernel installed. Some things you can do:

- Install some scientific Python distribution like Anaconda, that will allow you to play with Jupyter notebooks and will ship all the required dependencies.

- Use the Jupyter plugin for Visual Studio Code, as it is described in https://code.visualstudio.com/docs/datascience/jupyter-notebooks.

The main file is located at src/main.ipynb. I've tried my best to make the code lean and mean, so I hope it is understandable for everyone. If you don't want to customize the deck and you only want to run the detection on the shipped images, then you only need to run all the blocks except for the last two. Eventually, choose one of the last two blocks depending on which identification technique you want to apply, change the name of the file you want to analyze (by changing the value of query_image_name) and run it. You should be able to see results reasonably fast. It is not required to run all the blocks again if you want to analyze another image.

If you want to customize the deck, you can just replace all the images in the template folder. It is necessary, though, to remove the template image counterpart in the training folder, so it gets trained again. Deleting the entire training folder will make the program to train all cards again.

Some globals can be changed to further customize your deck, the name of the folder that contains the files or the filename patterns.
