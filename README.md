# DrawMyNumber

In this Keras machine learning tutorial you’ll learn:

- how to train a deep-learning convolutional neural network model, 
- convert it to Core ML, 
- and integrate it into an iOS app. 

You’ll learn some ML terminology, use some new tools, and pick up a bit of Python along the way.

The sample project uses ML’s Hello-World example — a model that classifies hand-written digits, trained on the MNIST dataset.

![screenshot](https://koenig-media.raywenderlich.com/uploads/2017/12/drawing.png)

#### Setting Up & Run Docker

- Download, install, and start Docker Community Edition for Mac
- In Terminal, enter the following commands, one at a time
 
```
cd <where you clone DrawMyNumber project>/others/docker-keras
docker build -t keras-mnist .
docker run --rm -it -p 8888:8888 -v $(pwd)/notebook:/workspace/notebook keras-mnist
```

- At the very end of the command output is a URL containing a token. It looks like this, but with a different token value:

```
http://0.0.0.0:8888/?token=7b189c8e200f49dcc33845d39101e8a0ab257db5f3b539a7
```

- Paste this URL into a browser to login to the Docker container’s notebook server.
- Open the notebook folder, then open keras_mnist.ipynb. Tap the Not Trusted button to change it to Trusted: this allows you to save changes you make to the notebook, as well as the model files, in the notebook folder.

---

Source:

- [Beginning Machine Learning with Keras & Core ML](https://www.raywenderlich.com/181760/beginning-machine-learning-keras-core-ml)
