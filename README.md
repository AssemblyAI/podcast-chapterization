# Podcast Chapterization

## Description

With this application, you can use AssemblyAI's [Auto Chapters](https://www.assemblyai.com/blog/introducing-assemblyai-auto-chapters-summarize-audio-and-video-files/) model to automatically create logical chapters for your favorite podcasts. This "summary over time" will create logical chapters as the topic of conversation changes.

Check out [this YouTube tutorial](https://youtu.be/q-5uAFJGqOk) to learn more about this application and how to run it locally. 

## To Run

* Download project files by running `git clone https://github.com/AssemblyAI/podcast-chapterization.git`
* Navigate to the project folder
* Ensure that [Streamlit](https://pypi.org/project/streamlit/) and other project dependencies are installed
* Add your AssemblyAI and [Listen Notes](https://www.listennotes.com/api/) API keys to the `api_secrets.py` file
* Run the application using the `streamlit run app.py`

## How it works

We start by working with the Listen Notes API to download podcast information. We then use the AssemblyAI API and the [Auto Chapters](https://www.assemblyai.com/docs/audio-intelligence#auto-chapters) feature to transcribe the podcast and generate chapters for us. When then iterate over that data to display information in the browser using Streamlit.
