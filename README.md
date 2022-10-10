# StableDiffusionTelegramChatbot
Just a simple Chatbot for Telegram that can generate Images using a prompt from the User and sends back the generated Image.

## Implemented Commands
A quick overview over the implemented commands

|Command|Description|
|:----------------|--------------------------------------------------------------------------------------------------------------------------------|
|/start           |Does nothing special just writes a welcoming message to the user.                                                               |
|/generate <Text> |Generates an image according to what was entered behind the command. For example "/generate Van Gogh playing american football".|
|/help            |Shows a small informational text about how */generate* works.                                                                   |
|/stop            |Should stop the bot but is not working properly, so if you have any suggestions to fix it, hit me up.                           |

## Setup
For the Bot we need two Tokens which are simple to get but you need a github account for one of them.

### Telegram Bot Token
First of all you need to create a Telegram Bot which is very simple. You just need to message "/newbot" to @BotFather on Telegram and follow the steps --> Giving it a Name and a Username. After that you will get the Token which you need to copy into the main.py File.

After this is done we need to do one last step which is to set the 

### Stable Diffusion API Token (Detailed Tutorial: https://replicate.com/blog/run-stable-diffusion-with-an-api)
You need to Sign In to Replicate using your GitHub Account with the following Link: https://replicate.com/signin?next=/blog/run-stable-diffusion-with-an-api. After that you can find your API Token on your Replicate Account: https://replicate.com/account. Now you need to set the Token as environment variable, which is different for Windows and Linux.
- On Windows you can open a command prompt (enter cmd in windows seearch bar) and then enter *SET REPLICATE_API_TOKEN=<token>* where <token> is your Token from Replicate
- On Linux you open the Terminal (CTRL+ALT+T) and then enter *export REPLICATE_API_TOKEN=<token>* where <token> is your Token from Replicate.
  
After this is done, you are almost good to go you just need to run the requirements.txt and then execute the main.py.
  
Have fun and enjoy :)
