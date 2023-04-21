# Audio to Text Summary Generator

This Python script uses OpenAI's GPT-3 language model to generate a summary of the audio content in a YouTube video. It also splits the summary into multiple "too long; didn't read" (tl;dr) chunks using the same language model.

## Dependencies

- Python 3.6 or higher
- `whisper` library
- `pytube` library
- `torch` library
- `torchaudio` library
- `openai` library

You can install these dependencies by running:

```
pip install whisper pytube torch torchaudio openai
```

## Usage

1. Set your OpenAI API key in the `openai.api_key` variable.
2. Set the `youtube_video_url` variable to the URL of the YouTube video you want to summarize.
3. Run the script using the command:

   ```
   python audio_to_text_summary_generator.py
   ```

4. The script will download the audio content of the video, generate a summary of the audio content using OpenAI's GPT-3 language model, and save the summary to a text file called `output.txt`.
5. The script will then split the summary into multiple tl;dr chunks using the same language model, and combine them into a full summary called `full_summary`.
6. You can modify the parameters of the OpenAI API request (e.g. temperature, max_tokens, etc.) in the `openai.Completion.create()` function to change the behavior of the language model.

## License

This script is released under the MIT License. See LICENSE for more details.

## Credits

This script was created by [YOUR NAME HERE] using the Whisper library by [WhisperAI](https://github.com/whisper-ai) and the OpenAI API.
