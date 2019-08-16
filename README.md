# Tabout

Tabout is a module that allows you to focus on other things while your script is running by playing an alert and/or sending a Slack message when your script is ready. Just enter the code into your script whenever you would like to be informed of completion, an error, a checkpoint, etc.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install tabout.

```bash
pip install tabout
```

## Usage

```python
from tabout import alertme

alertme() # plays a sound alert
alertme(sound=False, token='SAMPLE-TOKEN', channel='SAMPLE-CHANNEL-ID') # sends a Slack message to the channel chosen
alertme(token='SAMPLE-TOKEN', channel='SAMPLE-CHANNEL-ID', script = 'foobar.py') # plays a sound and sends a Slack message with notice of script used
```
### Finding your Slack token and channel ID:
**Slack token:** Go to [Slack's legacy token page](https://api.slack.com/custom-integrations/legacy-tokens), and find the option to create a token to your Slack channel of choice.

![Slack token screenshot](/tutorial/tabout_slack_token.png?raw=true)

**Channel ID:** To find the channel ID, first decide which channel or direct message you would like to send the alert to. Unless you want to let other know the status of your script, I would recommend choosing your own direct messages or Slackbot's. After joining that channel, the channel ID can be found in the url.

![Slack channel ID screenshot](/tutorial/tabout_slack_channel_url.png?raw=true)


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
