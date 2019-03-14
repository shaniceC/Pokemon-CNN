# Pokemon-CNN
This is a CNN to recognize images of Pokemon.
Done using tutorials by Adrian Rosebrock at 
https://www.pyimagesearch.com/2018/04/09/how-to-quickly-build-a-deep-learning-image-dataset/

https://www.pyimagesearch.com/2018/04/16/keras-and-convolutional-neural-networks-cnns/

# Downloading Images for Dataset
1. Get the Bing Image Search API key and enter it into line 16 of search_bing_api.py file where it says "YOUR_API_KEY_GOES_HERE".
2. Make directory dataset then make subdirectories for each type of Pokemon
3. To download images for each type of Pokemon, run command:

  python search_bing_api.py --query "{Pokemon}" --output dataset/{Pokemon}


Example: 
   python search_bing_api.py --query "charmander" --output dataset/charmander

# Training the Network
To train the network, run command:

python train.py --dataset {path to dataset} --model pokedex.model --label lb.pickle

# Classify Images
1. Create a new directory in the main folder for the images to be classified
2. Run command,

python classify.py --model pokedex.model --labelbin lb.pickle --image {directory/image_name}