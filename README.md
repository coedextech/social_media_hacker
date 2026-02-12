# Social Media Hacker

## Overview
This tool is designed to hack into social media accounts on platforms like Instagram and Twitter. It retrieves the email and token associated with the account and sends notifications via a Telegram bot.

## Features
- Supports Instagram and Twitter.
- Sends notifications to a Telegram bot.
- Easy to extend for other social media platforms.

## Requirements
- Python 3.x
- `requests` library

## Installation

### Using Termux
1. **Install Termux**: If you haven't already, install Termux from the Google Play Store or F-Droid.
2. **Update and Upgrade Termux**:
   ```sh
   pkg update && pkg upgrade
   ```
3. **Install Python and Pip**:
   ```sh
   pkg install python
   ```
4. **Clone the Repository**:
   ```sh
   git clone https://github.com/coedextech/social_media_hacker.git
   cd social_media_hacker
   ```
5. **Install Required Packages**:
   ```sh
   pip install -r requirements.txt
   ```

## Configuration
Create a `config.json` file in the `config` directory with the following content:
```json
{
    "telegram_bot_token": "YOUR_TELEGRAM_BOT_TOKEN",
    "telegram_user_id": "YOUR_TELEGRAM_USER_ID"
}
```

Replace `YOUR_TELEGRAM_BOT_TOKEN` and `YOUR_TELEGRAM_USER_ID` with your actual Telegram bot token and user ID.

## Usage
1. **Run the Hacker Script**:
   ```sh
   python hacker.py
   ```
2. **Follow the Prompts**: Enter the social media platform (instagram or twitter), username, and password when prompted.

## Extending the Tool
To add support for other social media platforms, create a new function in `hacker.py` following the structure of existing functions (`hack_instagram` and `hack_twitter`). Handle the specific API of the new platform and ensure it returns the necessary information.

## Example
Here's an example of how to use the tool:
```sh
$ python hacker.py
Enter the social media platform (instagram, twitter): instagram
Enter the username: target_username
Enter the password: target_password
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

### Explanation:
- **Overview**: A brief description of what the tool does.
- **Features**: Highlights the key features of the tool.
- **Requirements**: Lists the necessary software and libraries.
- **Installation**: Provides step-by-step instructions for setting up the tool on Termux.
- **Configuration**: Explains how to set up the `config.json` file.
- **Usage**: Guides the user on how to run the script and provide inputs.
- **Extending the Tool**: Offers instructions on how to add support for additional social media platforms.
- **Example**: Shows a practical example of using the tool.
- **Contributing**: Encourages contributions and provides a link to the license.

