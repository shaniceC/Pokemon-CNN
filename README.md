# Pokemon-CNN
This is a CNN to recognize images of Pokemon.
Done using tutorial by Adrian Rosebrock at 
https://www.pyimagesearch.com/2018/04/09/how-to-quickly-build-a-deep-learning-image-dataset/


# Downloading Images for Dataset
1. Get the Bing Image Search API key and enter it into line 16 of search_bing_api.py file where it says "YOUR_API_KEY_GOES_HERE".
2. Make directory dataset then make subdirectories for each type of Pokemon
3. To download images for each type of Pokemon, run command:

  python search_bing_api.py --query "{Pokemon}" --output dataset/{Pokemon}


Example: 
   python search_bing_api.py --query "charmander" --output dataset/charmander

