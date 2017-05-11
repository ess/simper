# simper
Parse JSON file "end-to-end" and output text to an mp3 file of the same name. Not particularly useful, but I was having fun writing bad poetry in JSON format, since sestinas are so, like 12th century, man.

A json file constructed like so:

```json
{
	"happy": [
		"clam",
		"clown",
		{
			"bottle of": [
				"bees",
				"kazoos"
			]
		}
	]
}
```
. . . yields an mp3 file with the following strings:

```
happy clam
happy clown
happy bottle of bees
happy bottle of kazoos
```

Example: http://neuralpro.be/blog/2017/2/the-love-schema/

Only tested on linux, so YMMV on other platforms.

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
You should probably use a nice virtualenv, since it's not worth the trouble of putting in your path or whatever. Install gTTS ```pip install -r requirements.txt```, and you should be good to go.
