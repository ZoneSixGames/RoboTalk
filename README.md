# RoboTalk by ZoneSix.io

The RoboTalk Podcast Creator is an application that helps you conduct research on a given topic, generate podcast scripts based on the researched topic, and create an audio podcast from the generated script.

## Requirements

This application requires API keys from Google Search Engine (https://console.cloud.google.com/) for current articles to research, https://openai.com for news summarization and script creation, and https://elevenlabs.io for speech generation.

## Installation

To run the application, follow these steps:

1. Clone the repository:

   ```shell
   git clone https://github.com/ZoneSixGames/RoboTalk.git
   ```

2. Navigate to the project directory:

   ```shell
   cd RobotTalk
   ```

3. Install the required dependencies:

   ```shell
   pip install -r requirements.txt
   ```

4. Set up environment variables:

   Create a `.env` file in the project directory and add the following environment variables:

   ```shell
   OPENAI_API_KEY=<your_openai_api_key>
   ELEVENLABS_API_KEY=<your_elevenlabs_api_key>
   ELEVENLABS_VOICE_1_ID=<your_elevenlabs_voice_1_id>
   GOOGLE_API_KEY=<your_google_api_key>
   CUSTOM_SEARCH_ENGINE_ID=<your_google_search_engine_id>
   ```

   Replace `<your_openai_api_key>`, `<your_elevenlabs_api_key>`, and other placeholders with your actual API keys.

5. Run the application:

   ```shell
   streamlit run robotalk.py
   ```

   This will start the application, and you can access it in your web browser at the link provided in your console.

## Usage

Once the application is running, you will see a web interface with the following options:

- **Podcast topic**: Enter the topic for your podcast.
- **Host Name**: Enter the name of the podcast host.
- **Enter the personality for the Host**: Describe the personality of the podcast host.
- **Research**: Click this button to research and summarize top news stories related to the podcast topic.
- **Generate Script**: Click this button to generate a podcast script based on the topic, research, and host's personality.
- **Create Podcast**: Click this button to create an audio podcast from the generated script.

The application will guide you through each step, and you can view the generated script and research summaries in the corresponding sections.

## Dependencies

The application uses the following Python dependencies:

decouple==3.3
streamlit==0.88.0
requests==2.26.0
beautifulsoup4==4.10.0
langchain==0.1.1
elevenlabs==1.0.1
urllib3==1.26.7
feedparser==6.0.8
pydub==0.25.1
nltk==3.6.5

These dependencies will be installed automatically when you follow the installation instructions.

## Support

For any issues or questions, please reach out at contact@zonesix.io

