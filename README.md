# Donald Trump Rallies Speeches

## The Corpus
The dataset comprises a comprehensive collection of full speeches delivered by **Donald Trump**, the 45th President of the United States, during **35 of his political rallies in 2019 and 2020**.  
A political rally is a public event where a political figure addresses a gathering of supporters to share their views, promote their agenda, and connect with the audience.  
In the context of Donald Trump's rally speeches, these events were pivotal moments in his political campaigns and presidency, characterized by passionate addresses, policy discussions, and engagement with the crowd. Analyzing these rally speeches provides insights into Trump's communication style, the issues he prioritized, and the sentiments he aimed to evoke among his supporters.
## Target Audience and the Intended Use of the Corpus
The target audience for the corpus includes political analysts, NLP researchers, journalists, political campaign strategists, public opinion researchers, educators, and students. The intended use spans political discourse analysis, NLP algorithm development, media coverage assessment, campaign strategy formulation, public opinion research, and educational purposes across various disciplines.  
## Text Selection Criteria
- **Inclusion of Rally Speeches**: Only speeches delivered during political rallies were considered, providing a concentrated focus on Trump's communication within the dynamic and charged atmosphere of campaign events.  
- **Time Frame**: The corpus comprises speeches delivered by Donald Trump during the years 2019 and 2020. This temporal restriction allows for a nuanced examination of his rhetoric during a critical period in his political career.
## Data Collection Process
The corpus of speeches used in this analysis was meticulously collected from [Kaggle](https://www.kaggle.com/datasets/christianlillelund/donald-trumps-rallies).  
The speeches, available in full length, are provided in TXT (text) file format. 
## Cleaning and Preprocessing Steps
- Cleaning:
  - The heading spaces in each txt files are removed.
  - The text is changed to lower case.
  - The punctuations in each txt file are removed.
- Preprocessing:
  - Natural Language Processing (NLP) and Python is used for Tokenization (splitting text into words/sentences).  
## Annotations Added and Tools
| Annnotations                 | Tools           |
|------------------------------|-----------------|
| Lemmas                       | spaCy, Python   |
| Part-of-Speech (POS) Tagging | spaCy, Python   |
| Proper Nouns                 | spaCy, Python   |
| Named Entity Recognition     | spaCy, Python   |
| Sentiment Classification     | spaCy, Python   |

## Files in this repository
- `txt` Each speech is stored in a separate TXT file, presenting the complete speech. The filename includes the date and location where the speech was delivered.
- `csv` This file is derived from the TXT files and has been enhanced using spaCy for additional linguistic analysis.
- `ipynb` This file contains the code of cleaning/preprocessing and processing of the TXT files and finally generating a CSV file.
## Columns in the CSV File
| Column           | Description                                              |
|------------------|----------------------------------------------------------|
| Filename         | The file name in the 'archive' folder                    |
| Document         | The original text exactly as it appears in the text file|
| Text             | Preprocessed text of this document                       |
| Tokens           | Splitting text into pieces called tokens                 |
| Lemmas           | Lemma is the form of a word as it appears in the dictionary|
| Parts-of-speech  | Part of speech, is a category of words with similar grammatical properties|
| Proper_Nouns     | The name of a particular person, place, organization, or thing in the files| 
| Named_Entities   | Named entity labels, providing information about the type of each named entity|
| NE_Words         | Real-world entities (location, person, time) mentioned in the text|

## Quality Check
- I reviewed each TXT file to identify and rectify any typos.
- I verified the successful import of the resulting CSV file and ensured its integrity.
