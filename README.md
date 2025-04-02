# Lip Sync Video Generation with Sync.so API

This project demonstrates how to generate a lip-synced video using the Sync.so API. The script takes an input video and an audio file and syncs the lip movements in the video to match the provided audio.

## Features
- Uses **Sync.so API** for AI-powered lip sync.
- Supports **MP4** output format.
- Polls the API to check the job status.

## Prerequisites
- Python 3.x
- `requests` library (`pip install requests`)
- Sync.so API key (Get yours from [Sync.so](https://sync.so/))

## Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/Tamilselvam-coder/lipsync-ai-using-api.git
   cd lipsync-ai-using-api
   ```
2. Install required dependencies:
   ```sh
   pip install requests
   ```

## Configuration
Update the `api_key` in the script with your Sync.so API key.

```python
api_key = "YOUR_API_KEY_HERE"
```

## Usage
Run the script:
```sh
python main.py
```

## Example Input
- **Video URL:** [Sample Video](https://synchlabs-public.s3.us-west-2.amazonaws.com/david_demo_shortvid-03a10044-7741-4cfc-816a-5bccd392d1ee.mp4)
- **Audio URL:** [Sample Audio](https://synchlabs-public.s3.us-west-2.amazonaws.com/david_demo_shortaud-27623a4f-edab-4c6a-8383-871b18961a4a.wav)

## Example Output
Once the job completes, the generated video URL will be printed in the terminal.
Example output:
```
Job completed!
Generated video URL: (https://api.sync.so/v2/generations/03175510-cac1-4c47-ac71-cdbc0053db20/result?token=a1ecc777-6d88-44ff-82b6-694c0f7afcc0)
```

## API Workflow
1. **Submit a Job**: Sends a request to Sync.so API with video and audio URLs.
2. **Poll the Job**: Continuously checks job status until completion.
3. **Retrieve Output**: Prints the generated video link upon successful completion.

## License
This project is licensed under the MIT License.

## Author
[tamilselvam](https://github.com/Tamilselvam-coder)

---
Feel free to modify and enhance this script according to your needs!


