# Tabout

Tabout is a python package that allows you to focus on other things while your script is running, by playing an alert and/or sending a Slack message when it's ready/

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install tabout.

```bash
pip install tabout
```

## Usage

```python
from tabout import alertme

alertme() # plays a sound alert
alertme(sound=False, token='SAMPLE-TOKEN', channel='SAMPLE-CHANNEL-ID') # sends a Slack message
alertme(token='SAMPLE-TOKEN', channel='SAMPLE-CHANNEL-ID', script = 'foobar.py') # plays a sound and sends a Slack message with notice of script used
```
### To find your Slack token and channel ID:
**Slack token:** Go to [Slack's legacy token page](https://api.slack.com/custom-integrations/legacy-tokens), and find the option to create a token to your Slack channel of choice.
![Alt text](/relative/path/to/img.jpg?raw=true "Optional Title"


**Channel ID:** 


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
