# The Literal Chinese Dictionary Data Repository

Welcome! The data that makes up the dictionary is split into two main folders:

* `./json`: main textual information and metadata for each dictionary entry

* `./icons`: the vector images which are included in entries

Please fork and raise a pull request against the data with new entries or fixes.

Contributing standard guidelines are below:

## Json (Entry)

These are the available fields (so far!):

1. `titleEn` **English Title** *(string)*: the most common English name of the object, place, or phrase.

2. `titleEnAlt` **Alternative English Titles** *(string array)*: names in the origin language is especially encouraged if it is a Roman language.

3. `titleZh` **Chinese Title** *(string)*: the most common Chinese name. Traditional Chinese characters should be used.

4. `titleZhAlt` **Alternative Chinese Titles** *(string array)*: these could be different colloquial names or regional translations.

5. `explanation` **The Literal Chinese Meaning** *(string)*: Chinese characters often have multiple meanings, discretion should be used to make sure the main entry here is meaningful or humourous.

6. `icons` **Icon File Names** *(string array)*: exact matching icon file names to be used for the entry.

7. `pinyin` **Mandarin Pinyin** *(string)*: the PRC Ministry of Education scheme is used as the standard.

8. `jyutping` **Cantonese Pinyin** *(string)*: the Linguistic Society of Hong Kong scheme is used as the standard.

9. `tailo` **Minnan/ Hokkien Pinyin** *(string)*:
the Taiwanese Ministry of Education scheme is used as the standard.

10. `credit` **Credit Small Print** *(string)*: always leading with "CC BY-NC-SA 4.0", which is the IP license used by this repository. Then include the licenses of the icons used.

11. `backgroundHex` **Background Colour Hex Code** *(string)*: always leading with "#" and set an alpha (transparency) level between 10 - 40.

12. `tags` **Category Tags** *(string array)*: common tags include: `countries`, `cities`, `activity`, `food`, `animal`. You must include one of these tags: `E2C` (English-to-Chinese translation), `C2E` (Chinese-to-English translation), or `meaning` (Developed from meaning in Chinese).

See [the template file here](template.json).

Please raise an issue if you have any suggestions.

## Icons

These must be vector graphics in `.svg` format.
The maximum resolution should be 512x512.

**Naming Convention**: 

* {shortest_english_title}.svg , or

* {shortest_english_title}_{depiction_of_icon}.svg

The icon style must be mostly flat, bordered in black and filled in technicolour. The artistic style of the author [Freepik](https://www.flaticon.com/authors/freepik) is regarded as a good standard.