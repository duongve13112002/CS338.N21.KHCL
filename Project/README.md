# Final Project
Developing a convolutional neural network using TensorFlow and Google's Quick, Draw! [dataset](https://github.com/googlecreativelab/quickdraw-dataset) to recognize hand-drawn images. Additionally, create a web application that allows users to draw images.

You can find a webapp demo [here](https://huggingface.co/spaces/duongve/Quick-Draw.Webapp).

## Setup
### Install libraries
Switch to the `Web Application` directory, create a new virtual environment, and install the required packages:

```
python -m venv ./venv
source ./venv/bin/activate
pip install -r requirements.txt
```

### Webapp

#### Native

After installing the required libraries, you can run the webapp using the following command:

```
uvicorn main:app
```
If the previous command doesn't work, please use this command instead.

```
python -m uvicorn main:app
```

The webapp should be available at [http://127.0.0.1:8000](http://127.0.0.1:8000).

#### Docker

Alternatively, you can also run it via Docker:

```
docker build . -t quickdraw-webapp
docker run -p 443:443 quickdraw-webapp
```

The webapp should be available at [http://127.0.0.1:443](http://127.0.0.1:443).
