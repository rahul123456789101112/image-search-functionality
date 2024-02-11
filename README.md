# Simple Image Search Engine Through Python Script


## Overview
- Simple image-based image search engine using Keras + Flask. You can launch the search engine just by running two python scripts.
- `offline.py`: This script extracts a deep-feature from each database image. Each feature is a 4096D fc6 activation from a VGG16 model with ImageNet pre-trained weights.
- `server.py`: This script runs a web-server. You can send your query image to the server via a Flask web-interface. The server finds similar images to the query by a simple linear scan.


## Usage
```bash
pip install -r requirements.txt

# Put your image files (*.jpg) on static/img

# Then fc6 features are extracted and saved on static/feature
# Note that it takes time for the first time because Keras downloads the VGG weights.
python offline.py

# Now you can do the search via localhost:5000
python server.py
```

# Simple Image Search Engine Through .ipynb File


## Overview
-Simple image-based image search engine using Keras + matplotlib You can Get the similar Images just by Put your Image Path.

## Usage
'''
-Open the Image_Search.ipynb file and  
Shift+Enter

At one time It Asked for Query Image Path Give it The Path and it Will give you the Similar Images
