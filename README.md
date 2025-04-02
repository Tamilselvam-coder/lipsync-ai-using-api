Lip Sync Video Generation with Sync.so API

This project demonstrates how to generate a lip-synced video using the Sync.so API. The script takes an input video and an audio file and syncs the lip movements in the video to match the provided audio.

Features

Uses Sync.so API for AI-powered lip sync.

Supports MP4 output format.

Polls the API to check the job status.

Prerequisites

Python 3.x

requests library (pip install requests)

Sync.so API key (Get yours from Sync.so)

Installation

Clone this repository:

git clone https://github.com/yourusername/syncso-lipsync.git
cd syncso-lipsync

Install required dependencies:

pip install requests

Configuration

Update the api_key in the script with your Sync.so API key.

api_key = "YOUR_API_KEY_HERE"

Usage

Run the script:

python lipsync.py

Example Input

Video URL: Sample Video

Audio URL: Sample Audio

Example Output

Once the job completes, the generated video URL will be printed in the terminal.
Example output:

Job completed!
Generated video URL: https://api.sync.so/output/generated_video.mp4

API Workflow

Submit a Job: Sends a request to Sync.so API with video and audio URLs.

Poll the Job: Continuously checks job status until completion.

Retrieve Output: Prints the generated video link upon successful completion.

License

This project is licensed under the MIT License.

Author

Your Name

Feel free to modify and enhance this script according to your needs!
