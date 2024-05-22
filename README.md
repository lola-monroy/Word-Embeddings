# Catalan General Crawling
## Directory structure

<pre>
corpus/
catalan_general_crawling.txt: Catalan corpus in txt format crawled from the web.
</pre>

## Sources
The Catalan General Crawling Corpus is a 435-million-token web corpus of Catalan built from the web. It has been obtained by crawling the 500 most popular .cat and .ad domains during July 2020. It consists of 434.817.705 tokens, 19.451.691 sentences and 1.016.114 documents. Documents are separated by single new lines. It is a subcorpus of the [Catalan Textual Corpus](https://zenodo.org/record/4519349).

## Processing
In order to be able to obtain a high-quality corpus, we applied strict filters to the raw data, by means of a cleaning pipeline built for the purpose. This pipeline supports 100+ languages and stands out for keeping document boundaries, instead of being sentence-based, which allows maintaining long-range dependencies.

Some of the supported input formats accepted:
- WARC (crawling)
- Plain text

Some of the text transformations applied:
- Encoding fixing and UTF-8 normalization
- Markup cleaning
- Sentence splitting
- Recover sentence splitting from badly converted PDFs

Some of the (heuristic) filters applied:
- Cascade of language identifiers
- Deduplication both at sentence and document level
- Percentage of characters not belonging to the alphabet
- Character length per sentence standard deviation of documents

## Contact
Ona de Gibert Bonet (ona.degibert@bsc.es)

Marta Villegas (marta.villegas@bsc.es)

## License
[![License: CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/)

The corpus is released under this licensing scheme:
- We do not own any of the text from which these data has been extracted
- We license the actual packaging of these data under a [Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/)

For more information, please see <https://creativecommons.org/licenses/by/4.0/>

### Notice and take down policy

Notice: Should you consider that our data contains material that is owned by you and should therefore not be reproduced here, please:

    Clearly identify yourself, with detailed contact data such as an address, telephone number or email address at which you can be contacted.
    Clearly identify the copyrighted work claimed to be infringed.
    Clearly identify the material that is claimed to be infringing and information reasonably sufficient to allow us to locate

Copyright (c) 2021 Text Mining Unit at BSC

