1. Install Node.js
Ensure you have Node.js installed on your system. You can download it here.

To check if it's installed, run:
node -v
npm -v

2. Clone or Create the Project Directory
Create a directory for the project and navigate to it.

mkdir my-discord-hf-bot
cd my-discord-hf-bot

3. Initialize npm Project
Inside your project directory, initialize the Node.js project:

npm init -y
4. Install Required npm Packages
Run the following command to install the necessary packages, including Discord.js for interacting with Discord, Hugging Face inference for AI interactions, and UUID for unique IDs.

npm install discord.js @huggingface/inference uuid
5. Configure Your API Keys
Replace the placeholders with your actual API keys:

DISCORD_TOKEN: Your Discord bot token.
HUGGING_FACE_API_KEY: Your Hugging Face API key.
You can get the tokens from:

Discord Bot Token: Create a bot using the Discord Developer Portal.
Hugging Face API Key: Sign up and get the API key from Hugging Face.
Replace the following placeholders in the code:

const DISCORD_TOKEN = 'YOUR_DISCORD_BOT_TOKEN';
const HUGGING_FACE_API_KEY = 'YOUR_HUGGING_FACE_API_KEY';
6. Create and Configure the Bot on Discord
Go to the Discord Developer Portal, create a new application, and then create a bot for it.
Copy the Bot Token and replace the placeholder in your code.
Under the bot settings, enable the required intents (like Message Content Intent, Guild Messages, Direct Messages).
Add the bot to your Discord server using the OAuth2 URL generator and give it appropriate permissions, e.g., SEND_MESSAGES, READ_MESSAGE_HISTORY, etc.

7. Run the Project
Once you've configured everything, you can start the bot using:

node index.js
Make sure the bot logs in and you see the message indicating it’s online:

Logged in as [BotName]!
