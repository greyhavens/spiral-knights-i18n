# spiral-knights-translations
Internationalization bundles for Spiral Knights

## How it works
We will occasionally publish new English translations here.

We will accept pull requests for other languages, including new ones.

Then these translations will make their way into the game.

## License, of sorts

The files in this repository are intended only to help improve Spiral Knights.
Contributions are granted to Grey Havens for use in the game.

### Fine details

If a translation doesn't need to change it can be omitted from a bundle and the English
version will be used.

The properties files need to be well-formatted and readable by Java. Characters above 127
should be escaped by using `\u00e7` convention.

Run `python3 tools/check_bundles.py` before sending a pull request. It reports keys that
aren't in the English bundle, unescaped characters, and placeholders, HTML tags or `|`
separators that don't match the English.

#### Ancient history

We used to have a google spreadsheet. We could push a button and it would export the current
english translations and also import anything from any of the corresponding columns for
each language. Perhaps it would be nice to re-create something like that, built on top of this.

Having a front-end for nicely typing-in a label or message and having it automatically output
a well-formatted .properties file would be great!
