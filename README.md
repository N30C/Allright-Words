# Keyword extraction from scraped job descriptions using NLP and neural networks
Jupyter notebook that performs a keyword extraction from scraped job descriptions using NLP and neural networks.

This code is intended for **educational use only**. It can go against terms of service of the platforms scraped.
## Infos
This Jupyter Notebook contains a sequenced set of modular Python code blocks.
In the third cell is possible to specify the job position and the location:   
```
position = 'Software Developer'
location = 'Silicon Valley'
  ```
It uses beautiful soup and selenium to scrape LinkedIn and Indeed jobs descriptions list and save it as a .csv file.
The csv file is then processed using NLP (Natural Language Processing) algorithms to remove stop words (both default and custom), to do stemming and lemmatization to reduce inflectional forms and sometimes derivationally related forms of a word to a common base form.
Then the most common keywords are computed and visualized in different forms: 
1. Word cloud
2. Single word bar plot
3. Bi-gram bar plot 
4. Tri-gram bar plot

Moreover three different list of keywords are retrieved using:
1. TF-IDF (term frequency–inverse document frequency)
2. Summa - TextRank
3. YAKE - Yet Another Keyword Extractor

## How to use it
1. From the command line, clone this repo. Or download it manually.
  ```
  git clone https://github.com/Niko30C/Allright-Words.git
  ```
2. Copy the stop words custom file int he working directory, modify it or do your own, putting a word per line
  * custom-stopwords.txt
3. Then, you can import it on [Google Colab](https://colab.research.google.com/) or run it in your machine.
4. Modify job position and location in the third cell.
5. Run it! If some cells retrieve errors, wait few seconds and rerun the cell.
6. Don't run it too often in a small amount of time or the websites will blacklist list you for hours or even days.  

