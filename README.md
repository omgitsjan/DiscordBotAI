
# Discord Bot powered by OpenAI _(ChatGPT, DALL-E and more)_

This is a simple Discord bot that uses the OpenAI ChatGPT API to generate responses to messages in a Discord chat, also having some additional features. The bot is written in C# and uses the [DSharpPlus](https://github.com/DSharpPlus/DSharpPlus) library to interact with the Discord API and the [RestSharp](https://github.com/restsharp/RestSharp) library to make HTTP requests to the OpenAI API and for Example to the Watch2Gether API.

## Installation

To fully use this bot, you will need the following:

- A Discord bot token
- An OpenAI API key
- An Watch2Gether API key
- An OpenWeatherMap API key

Once you have these, you can clone this repository and build the project using the `dotnet` command, like this:

Copy code

`git clone https://github.com/omgitsjan/DiscordBotAI
cd DiscordBot
dotnet restore
dotnet build`

Next, you need to specify the environment variables for the Discord bot token and ChatGPT API key when starting the bot. For example:

Dont forget to change the variables in appsettings.json.

Replace `DiscordToken`, `ChatGptApiKey`, `W2GApiKey` and `OpenWeatherMapApiKey` with your actual tokens and API keys, respectively.

## Usage

To use the bot, send a message in the form of `/chatgpt <prompt>` or `/dall-e <prompt>` where `<prompt>` is the text you want the bot to generate a response for. For example:

*ChatGPT:*

`/chatgpt What is the meaning of life?`

*DALL-E:*

`/dall-e Pixel art where monkeys trying to rob a bank`

The bot will respond with a generated image/text response based on the prompt you provided.


**Additional**

*Watch2Gether:*

`/watch2gether (optional)<video-url>`

The bot will response with a link to a Watch2Gether Room with an optional Video as preload.

*OpenWeatherMap:*

`/weather <city>`

The bot will respond with the current Weather to a specific city.

*Ping:*

`/ping`

Retruns the Latency Pong...

## License

This project is licensed under the MIT License. See [LICENSE](https://github.com/omgitsjan/DiscordBot/blob/main/LICENSE) for details.
