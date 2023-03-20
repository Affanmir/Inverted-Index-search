# inverted-index-search
inverted-index-search is python library for searching up keywords or sub words in a corpus of data using inverted index lookup

## Installation

Use the package manager pip to install.

```bash
pip install inverted-index-search
```

## Usage

```python
from  inverted_index_search import search_doc



phrases = ["something in the way for us", "bussing in "]
doc = 'something in in in'
print(search_doc(doc, phrases, n_gram_level='char', doc_ngrams=[1],phrase_ngrams=[1], verbose=False))
>> {'something in the way for us': {'s': {'count': 2, 'occured': [(0, 1)]}, 'o': {'count': 2, 'occured': [(1, 2)]}, 'm': {'count': 1, 'occured': [(2, 3)]}, 'e': {'count': 2, 'occured': [(3, 4)]}, 't': {'count': 2, 'occured': [(4, 5)]}, 'h': {'count': 2, 'occured': [(5, 6)]}, 'i': {'count': 8, 'occured': [(6, 7), (10, 11), (13, 14), (16, 17)]}, 'n': {'count': 8, 'occured': [(7, 8), (11, 12), (14, 15), (17, 18)]}, 'g': {'count': 1, 'occured': [(8, 9)]}}, 'bussing in ': {'s': {'count': 2, 'occured': [(0, 1)]}, 'i': {'count': 8, 'occured': [(6, 7), (10, 11), (13, 14), (16, 17)]}, 'n': {'count': 8, 'occured': [(7, 8), (11, 12), (14, 15), (17, 18)]}, 'g': {'count': 1, 'occured': [(8, 9)]}}}




```

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Github

[Affan](https://github.com/Affanmir)
