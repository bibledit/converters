# Converters

Converters from the USFM format to other formats.

## Installation

The converters can run on a local workstation and on a server.

Clone or download the converters from the following location:
https://github.com/bibledit/converters.
Unpack the software into a known folder.

The converters need a Java Runtime Environment to run.
Install the ```java``` binary.

## Loading Bible text

The input for the converters will be Bible text in the USFM format.
Download all separate USFM files from your Bible editor and store them into a known folder.
Or download a zip file with all the USFM files, and unpack the zip file into a known folder.

## Quick Bible

Converting Bible data to Quick Bible consists of multiple steps.
1. Convert the USFM data to a ```.yet``` file.
2. Convert the ```.yet``` file to a ```.yes``` file.
3. Load the ```.yes``` file into the Quick Bible app.

To convert the USFM data to a .yet file, issue the following command:
```
java -jar path/to/converters/BibleMultiConverter/BibleMultiConverter.jar USFM path/to/usfm/folder QuickBible path/to/bible.yet
```

Optionally you may edit the ```bible.yet``` file and update the names of the books or make other updates.

To convert the .yet file to a .yes file, issue the following command:
```
java -jar path/to/converters/QuickBible/YetToYes2.jar --ignore-skipped-verses path/to/bible.yet path/to/bible.yes
```

Then finally load the .yet file into the Quick Bible app and enjoy the result.
