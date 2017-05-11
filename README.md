# simper
- read json file to mp3 file

Example: http://neuralpro.be/blog/2017/2/the-love-schema/

## Requires 
- gTTS

## Usage
```bash
usage: simper [-h] [--language LANGUAGE] filenames [filenames ...]

ever-so-useful script to audibly navigate a JSON object

positional arguments:
  filenames            json files to parse

optional arguments:
  -h, --help           show this help message and exit
  --language LANGUAGE  two-character ISO 639-1 language code. Defaults to "en"

```

## Installation
You should probably use a nice virtualenv, since it's not worth the trouble of putting in your path or whatever. Install gTTS ```pip install -r requirements.txt````, and you should be good to go.
