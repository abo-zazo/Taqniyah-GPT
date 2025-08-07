# Taqniyah-GPT
Welcome to "Taqniyah GPT" Your smart assistant to answer your questions in your language! Start chatting below 👇
from zipfile import ZipFile
import shutil
import os

# Re-define paths after code state reset
zip_path = "/mnt/data/TaqniaGPT_web_wrapper.zip"
extract_path = "/mnt/data/TaqniaGPT_web_wrapper"

# Unzip the uploaded WebView wrapper project to a working directory
with ZipFile(zip_path, 'r') as zip_ref:
    zip_ref.extractall(extract_path)

# Output the list of files/folders extracted for verification
extracted_files = list(sorted((extract_path + "/" + f) for f in os.listdir(extract_path)))
extracted_files[:10]  # Show first 10 items for confirmation
