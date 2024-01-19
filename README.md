# Edgar Allen Poe's language use in his gothic short stories<br>

**1. Corpus**<br>
The corpus contains four short stories written by the American author Edgar Allen Poe (1809-1849): *The Assignation*, *The Black Cat*, *The Masque of the Red Death*, and *The Tell-Tale Heart*. These short stories constitute parts of Poe's gothic fiction.<br>

**2. Target audience and intended use of the corpus**<br>
The corpus can be used by anyone interested in Edgar Allan Poe’s gothic literature, especially from the perspective of language use regarding this genre.<br>

**3. Text selection criteria**<br>
I aimed to select texts that can be downloaded as plain text files and that are openly accessible. I intended to gather short stories of the same genre, so that features of one specific style can be investigated and revealed through a series of texts. Another aspect I took into consideration is the limit of the number of word tokens (preferably not more than 10,000) stated in the instructions of the assignment. <br>

**4. Data collection process**<br>
I accessed the short stories through the [Gutenberg project](https://www.gutenberg.org/), and downloaded them as plain text files with UTF-8 encoding. <br>
Source: https://www.gutenberg.org/ebooks/2148<br>

**5. Cleaning and pre-processing steps**<br>
I removed the titles of the short stories from the beginning of the texts and removed the extra spaces from the text files.<br>

**6. Tools and annotations**<br>
I used pandas to create dataframes and spaCy to process, tokenize, lemmatize, and annotate the short stories.<br>
I added part-of-speech category tags and named entity tags as annotations. <br>

**7. File format description**<br>
The files in the data directory are the four short stories as plain text files (poe_the assignation.txt, poe_the black cat.txt, poe_the masque of the red death.txt, poe_the tell-tale heart.txt). <br>

The repository also includes the following files: <br>
- `metadata.csv` the metadata about the short stories in a CSV file <br>
- `processing_text_corpus.ipynb` the processing of the text corpus <br>
- `poe_short_stories_enriched_with_spaCy_tags.csv` the short stories enriched with metadata and spaCy annotations in a CSV file <br>

**8. Description of columns in the CSV file containing annotations**<br>

| Columns | Description |
| ------------- | ------------- |
| Filename | the name of the file |
| Author | the name of the author of the short story |
| Title | the title of the short story |
| Language | the language of the short story |
| Genre | the genre of the short story |
| First published | the year in which the short story was first published |
| Text | the original short story without its title, exactly as it appears in the plain text file |
| Tokens | the tokenized version of the short story |
| Token_counts | the number of word tokens of the short story |
| Lemmas | the lemmatized version of the short story |
| POS | part-of-speech category tags of the short story |
| Adjectives | words tagged as adjectives in the short story |
| Named_Entities | named entity tags of the short story |
| NE_Words | phrases tagged as named entities |
| NE_PERSON | phrases tagged as 'PERSON' named entity |
| NE_TIME | phrases tagged as 'TIME' named entity |
| NE_DATE | phrases tagged as 'DATE' named entity |

**9. Quality checks** <br>
I checked whether there is a different number of occurrences of a verb as a token and as a lemma (see Jupyter Notebook).

**10. Analysis** <br>
The Jupyter Notebook contains a brief analysis of the occurrence of verbs, nouns, and adjectives in each short story, the most frequently appearing adjectives in the corpus, the distribution of 'PERSON', 'TIME' and 'DATE' named entities across the short stories, and the most common named entities tagged as 'TIME' in the corpus.

![a photo of Edgar Allan Poe](https://media.poetryfoundation.org/uploads/media/default/0001/21/bd5c888c4689e6cd3583bbe7575a1a2cad3487f6.jpeg?w=1274&h=&fit=max&key=3&sig=8d502e04711b2041ace345b267647ca4bfe0881cdc1ec890ddc9c8b0f81331c3&1274)
