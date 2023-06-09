# CapsON
To generate multiple captions on uploading image

Create a 'static' folder in the same directory as the root folder containing all '.html' and '.py' files. In the static folder, create a 'uploads' folder. This uploads folder is where all the uploaded pictures will get saved.

# Home Page (Before uploading the image to be captioned)
<img width="1440" alt="Screenshot 2023-06-04 at 10 04 07 PM" src="https://github.com/anusha-adhikari/CapsON/assets/74814765/7de374bf-bb75-46ad-b7af-e84b15a23139">

# Home Page (After uploading the image to be captioned)
<img width="1440" alt="Screenshot 2023-06-04 at 10 06 57 PM" src="https://github.com/anusha-adhikari/CapsON/assets/74814765/5e3e464d-056d-4b43-9798-aea6ff105eec">

# Captions generated
<img width="1440" alt="Screenshot 2023-06-04 at 10 04 15 PM" src="https://github.com/anusha-adhikari/CapsON/assets/74814765/d7fdd468-49c1-4726-a6a8-7c1bcf17fba5">

# Files Explained :
1) CapGen.py - To generate a caption from the input image using VisionEncoderDecoderModel (model), ViTImageProcessor (feature_extractor), AutoTokenizer (tokenizer)
2) MultiCap.py - To augment the caption from CapGen.py using PegasusForConditionalGeneration (model), PegasusTokenizer (tokenizer)
3) index.html - HTML code for the index page to enter the image for caption generation.
4) result.html - HTML code for the result page to show the 10 different captions generated for the input image. (10 captions generated by augmenting (MultiCap.py) the caption from CapGen.py 10 times using a for loop (main.py, described below))
5) main.py - Combining the Multiple Caption Generation codes with the HTML codes to create a website using the Flask framework. MultiCap.py is looped 10 times to generate 10 different captions.


# Challenges faced in a tight 2-day timeframe :
1) Being from an ML background, it was especially hard for me to create an user interface as well as the image caption generator, and ML model.
2) Not only learning certain aspects of NLP (Natural Language Processing) along with usage of Hugging Face, but also implementing the same.

# Disclaimer :
Despite the efforts, due to lack in web development background, the website could not be deployed. However, by downloading the codes in the same file (preferably) and performing the following instructions, one could get a local IP address to run the website.
