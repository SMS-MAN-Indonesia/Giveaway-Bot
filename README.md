# Giveaway Bot

Giveaway Bot is a Telegram bot designed to manage and run giveaways in a specified channel. This bot supports multiple languages and can be configured to use different language files.

## Installation

### Prerequisites

- Python 3.x
- pip (Python package installer)
- A Telegram bot token from [BotFather](https://core.telegram.org/bots#botfather)

### Step-by-Step Guide

1. **Clone the Repository**

   ```sh
   git clone https://github.com/SMS-MAN-Indonesia/Giveaway-Bot.git
   cd Giveaway-Bot
   ```

2. **Create a Virtual Environment**

   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install Dependencies**

   ```sh
   pip install -r requirements.txt
   ```

4. **Configure the Bot**

   Create a `config.py` file in the root directory with the following content:

   ```python
   TOKEN = 'your_bot_token_here'  # Replace 'your_bot_token_here' with your actual bot token from BotFather
   db_url = 'sqlite:///giveaway_bot.db'  # SQLite database URL

   ```

5. **Prepare Language Files**

   Ensure that you have the language files (`ID.json`, `ENG.json`, `RU.json`) in the root directory of the project. These files contain the bot's responses in different languages.

## Usage

1. **Run the Bot**

   ```sh
   python main.py
   ```

   This will start the bot using the configurations specified in `config.py`.

2. **Interacting with the Bot**

   - Invite the bot to your Telegram channel.
   - Use the bot commands to create and manage giveaways.

### Functions

- **language_check(user_id)**: Determines the user's language preference and loads the appropriate language file.
- **create_inlineKeyboard(key, row=0)**: Creates an inline keyboard for the bot interface.

## Example Configuration

Here is an example of what your `config.py` might look like:

```python
TOKEN = '123456789:ABCDefghIJKlmnoPQRSTUvwxYZ'  # Example token from BotFather
db_url = 'sqlite:///giveaway_bot.db'
```

## Contributing

Feel free to fork this project, create a new branch, and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
