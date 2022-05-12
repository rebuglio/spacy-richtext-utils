# spacy-richtext-utils
___

## Usage

```
import spacy
from spacy_richtext_utils import html_utils

nlp = spacy.load("en_core_web_sm")
html_utils(nlp)
doc = nlp("Leonardo Da Vinci painted the <i>monna lisa</i>.")

print('Entities:  ', [ent.text for ent in doc.ents])
print('Spans iter:', [span.text for span in doc._.spans])

>>> Entities:   ['Leonardo Da Vinci', 'monna lisa']
>>> Spans iter: ['Leonardo Da Vinci', 'painted', 'the', 'monna lisa', '.']
```

