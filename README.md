# Text Mining and Sentiment Analysis @ ADD_in 2023

This repository contains a number of examples on Text Processig and Sentiment Analyis, to be explored in the context of the Summer School: [Advanced Analysis for Integrated Urban Development Strategies (ADD_In)](https://istar.iscte-iul.pt/summerschool2023/)

### Contents and how to proceed

* [SA-strategies](sa-strategies.ipynb) - Describes a number of strategies for performing Sentiment Analysis


<p id="files-in-google-colab"></p>

### Using your files in Google Colab

Supose that you have the file data.zip.
You should perform the following steps in order to use that data in a persistent way in google colab.
1. Uncompress the file, thus creating a folder named "data", containing files.
2. Create the folder ADD_In in your Google Drive, and upload the "data" folder into this folder. You will get the following directory structure: ADD_In/data
3. In order to use the data in google colab, you should now perform the following sequence:

        from google.colab import drive
        drive.mount('/content/drive')
        # You will have to authorize this operation using your internet browser.

        # The following command allows you to go to the "data" directory
        %cd /content/drive/MyDrive/ADD_In/data

        # The following example lists the files
        import glob
        files=glob.glob("*")
        print(files)