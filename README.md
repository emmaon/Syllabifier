# syllabifier
Syllabifies words outputting ARPAbet phoneme strings

## Requirements:
- Python 3 
- NLTK (and nltk.corpus.cmudict.dict() - may require downloading)

## Input:

- *\[name\].txt* :  file containing one word per line you wish to syllabify (case insensitive)
> THIS  
> IS  
> AN  
> EXAMPLE  

- *\[dictionary_name\].txt* (optional) : additional pronunciation file for words not included in the CMU Pronouncing Dictionary 
(can be generated using [this tool](http://www.speech.cs.cmu.edu/tools/lextool.html))
> THIS	DH IH S  
> IS	IH Z  
> AN	AE N  
> EXAMPLE	IH G Z AE M P AH L  

## Output:
- *syllables.\[name\].txt* : file containing one syllable per line
> \['DH', 'IH', 'S'\]  
> \['IH', 'Z'\]  
> \['AE', 'N'\]  
> \['IH', 'G'\]  
> \['Z', 'AE', 'M'\]  
> \['P', 'AH', 'L'\]  

- *unknown.\[name\].txt* : file containing any words not contained in the CMU Pronouncing Dictionary or Supplementary Dictionary
