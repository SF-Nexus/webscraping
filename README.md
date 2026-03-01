# webscraping-SF

Scripts and notebooks for collecting science fiction texts and metadata from various online sources.

## Contents

### gutenberg/

Scrape and download texts from [Project Gutenberg](https://www.gutenberg.org/) bookshelves. Includes a notebook for browsing bookshelves, downloading full texts, and basic cleaning.

### internetarchive/

Download science fiction collections from the [Internet Archive](https://archive.org/) using their Python API. Covers the Project Gutenberg SF collection, Pulp Magazine Archive, and other SF holdings.

### StarTrek/

- **Star_Trek_API.ipynb** -- Query the [STAPI](http://stapi.co/) (Star Trek API) for character and episode data. Uses R via rpy2.
- **Wikidata Star Trek.ipynb** -- Query [Wikidata](https://www.wikidata.org/) via SPARQL for Star Trek series, cast, species, and films. Uses Python/SPARQLWrapper.

### nytimes_books/

Query the [NYT Books API](https://developer.nytimes.com/docs/books-product/1/overview) for bestseller list data. Requires an API key (stored in a local `config.py`, not tracked).

## Requirements

- Python 3.7+
- See `requirements_ia.txt` for Internet Archive dependencies
- Notebooks use standard libraries: `requests`, `pandas`, `SPARQLWrapper`, `beautifulsoup4`
- The Star Trek API notebook requires R and `rpy2`
