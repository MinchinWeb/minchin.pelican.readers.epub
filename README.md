# minchin.pelican.readers.epub

Pelican ePub reader

## Background

I've been looking at a way to keep study notes on various books. See [study companion](https://github.com/MinchinWeb/study-companion). The (possible) solution here is to create a "reader" or plugin for [Pelican](https://docs.getpelican.com/en/latest/index.html) that would render the source material (provided as an ePub file) with the annotations provided in "sidecar" file(s). (There is already an annotation format defined as part of the ePub standard.

## Anticipated Development Process

1. Create Pelican reader for ePub format.
    1. re-write internal links
    2. apply internal CSS?
    3. add *next* and *previous* page metadata
2. Determine possitions within the file (aka "annotation addresses")
    1. add these locations inline in the output HTML to confirm and for placing new annotations 
3. Read sidecar annotations
    1. is there a standardized file format already specified?
    2. apply highlighting
    3. add text notes as "footnotes", possiblity as inline HTML
    4. update site CSS to display annotations as a "side note"

## See Also

- [How to create a new reader](https://docs.getpelican.com/en/latest/plugins.html) -- basics of how to create a new reader from the Pelican documentation
- [Pelican MboxReader](https://github.com/TC01/pelican-mboxreader) -- plugin that reads archived email and outputs each email as a seperate page. Of interest because this ePub reader will also have one input file but many output files.







