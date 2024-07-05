# Text_Extraction_From_Image
In this project, we will focus on extracting text from images. Once the text is extracted, we will apply several basic OpenCV functions to enhance the text and improve accuracy. This project aims to save time and effort by eliminating the need to manually type text from images.

# import requests to install tesseract

      import requests 

we have to importing request library for fetching the url for git file and images.

# Downloading tesseract-ocr file

    r = requests.get("https://raw.githubusercontent.com/tesseract-ocr/tessdata/4.00/ind.traineddata", stream = True)

# writing data to file to avoid path issues 
     with open("/usr/share/tesseract-ocr/4.00/tessdata/ind.traineddata", "wb") as file:
           for block in r.iter_content(chunk_size = 1024):
               if block:
                   file.writer(block)

we will now download tesseract which is required for pytesseract library to run and save the file at the path in open() function.



# install libraries required for optical character recongnition 
     ! apt install tessert-ocr libtesseract-dev libmagickwand-dev

# importing IPython to clear output which is not important 

    from IPython.display import HTML, clear_output
    clear_output()

In this step we will install the required libraries for ocr and we will also import IPython function to clear the undesired.


# installing pytesseract and opencv

     ! pip install pytesseract wand opencv-python
     clear_output()

Now we will install pytesseract and opencv libraries 


     # Import libraries 
     from PIL import Image 
     Import pytesseract
     Import cv2
     Import numpy as np
     from pytesseract import Output
     Import re

Importing require libraries


# Reading image from url 

    





    

   
