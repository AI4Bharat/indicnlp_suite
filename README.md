# IndicNLPSuite

_(page updation in progress)_

Natural Language Understanding resources for Indian languages

NLP resources for 11 major Indian languages from two major language families. These resources include: (a) large-scale sentence-level monolingual corpora, (b) pre-trained word embeddings, (c) pre-trained language models, and (d) multiple NLU evaluation datasets (IndicGLUE benchmark). 

## IndicCorp

IndicCorp has been developed by discovering and scraping thousands of web sources - primarily news, magazines and books, over a duration of several months.

IndicCorp is one of the largest publicly-available corpora for Indian languages. It has also been used to train our released models which have obtained state-of-the-art performance on many tasks.

### Corpus Format

The corpus is a single large text file containing one sentence per line. The [publicly released version](#downloads) is randomly shuffled, untokenized and deduplicated. 

### Downloads


| Language | \# News Articles* | Sentences     | Tokens        | Link     |
| -------- | ----------------- | ------------- | ------------- | -------- |
| as       | 0.60M             | 1.39M   |  32.6M  | [link](https://objectstore.e2enetworks.net/ai4b-public-nlu-nlg/v1-indiccorp/as.txt) |
| bn       | 3.83M             | 39.9M | 836M  | [link](https://objectstore.e2enetworks.net/ai4b-public-nlu-nlg/v1-indiccorp/bn.txt) |
| en       | 3.49M             | 54.3M | 1.22B | [link](https://objectstore.e2enetworks.net/ai4b-public-nlu-nlg/v1-indiccorp/en.txt) |
| gu       | 2.63M             | 41.1M | 719M  | [link](https://objectstore.e2enetworks.net/ai4b-public-nlu-nlg/v1-indiccorp/gu.txt) |
| hi       | 4.95M             | 63.1M |  1.86B | [link](https://objectstore.e2enetworks.net/ai4b-public-nlu-nlg/v1-indiccorp/hi.txt) |
| kn       | 3.76M             | 53.3M | 713M  | [link](https://objectstore.e2enetworks.net/ai4b-public-nlu-nlg/v1-indiccorp/kn.txt) |
| ml       | 4.75M             | 50.2M |  721M  | [link](https://objectstore.e2enetworks.net/ai4b-public-nlu-nlg/v1-indiccorp/ml.txt) |
| mr       | 2.31M             | 34.0M | 551M  | [link](https://objectstore.e2enetworks.net/ai4b-public-nlu-nlg/v1-indiccorp/mr.txt) |
| or       | 0.69M             | 6.94M   | 107M   | [link](https://objectstore.e2enetworks.net/ai4b-public-nlu-nlg/v1-indiccorp/or.txt) |
| pa       | 2.64M             | 29.2M |  773M  | [link](https://objectstore.e2enetworks.net/ai4b-public-nlu-nlg/v1-indiccorp/pa.txt) |
| ta       | 4.41M             |  31.5M   |  582M  | [link](https://objectstore.e2enetworks.net/ai4b-public-nlu-nlg/v1-indiccorp/ta.txt) |
| te       | 3.98M             | 47.9M   |  674M  | [link](https://objectstore.e2enetworks.net/ai4b-public-nlu-nlg/v1-indiccorp/te.txt) |

## IndicFT

## IndicBERT

## IndicGLUE

To thoroughly evaluate language models on Indian languages, we need a robust NLU benchmark consisting of a wide variety of tasks and covering all the Indian languages. IndicGLUE is a natural language understanding benchmark that we propose. It consists of 6 tasks which we describe in the next section.

In addition, we also compile a list of additional evaluations which comprises of tasks based on publicly-available datasets.

### Downloads


Dataset | Download Link |
------  | -----   |
Soham News Article Classification | [link](https://ai4b-public-nlu-nlg.objectstore.e2enetworks.net/IndicGLUE/soham-articles.tar.gz)
iNLTK Headline Classification | [link](https://ai4b-public-nlu-nlg.objectstore.e2enetworks.net/IndicGLUE/inltk-headlines.tar.gz)
BBC News Article Classification | [link](https://ai4b-public-nlu-nlg.objectstore.e2enetworks.net/IndicGLUE/bbc-articles.tar.gz)
AI4Bharat Wikipedia Section Titles | [link](https://ai4b-public-nlu-nlg.objectstore.e2enetworks.net/IndicGLUE/wiki-section-titles.tar.gz)
AI4Bharat Cloze-style Question Answering | [link](https://ai4b-public-nlu-nlg.objectstore.e2enetworks.net/IndicGLUE/wiki-cloze.tar.gz)
AI4Bharat Winnograd Natural Language Inference | [link](https://ai4b-public-nlu-nlg.objectstore.e2enetworks.net/IndicGLUE/wnli-translated.tar.gz)
AI4Bharat Choice of Plausible Alternatives | [link](https://ai4b-public-nlu-nlg.objectstore.e2enetworks.net/IndicGLUE/copa-translated.tar.gz)
WikiAnnNER  | [link](https://ai4b-public-nlu-nlg.objectstore.e2enetworks.net/IndicGLUE/wikiann-ner.tar.gz)
CVIT-MKB Cross-lingual Sentence Retrieval | [link](https://ai4b-public-nlu-nlg.objectstore.e2enetworks.net/IndicGLUE/cvit-mkb.tar.gz)
IITP Movie Reviews Sentiment | [link](https://ai4b-public-nlu-nlg.objectstore.e2enetworks.net/IndicGLUE/iitp-movie-reviews.tar.gz)
IITP Product Reviews | [link](https://ai4b-public-nlu-nlg.objectstore.e2enetworks.net/IndicGLUE/iitp-product-reviews.tar.gz)
ACTSA Sentiment Classifcation | [link](https://ai4b-public-nlu-nlg.objectstore.e2enetworks.net/IndicGLUE/actsa.tar.gz)
MIDAS Discourse | [link](https://ai4b-public-nlu-nlg.objectstore.e2enetworks.net/IndicGLUE/midas-discourse.tar.gz)
Amrita Paraphrase | [link](https://nlp.amrita.edu/dpil_cen/index.html) _(need to request)_

The code to run evaluations on the above dataset is provided in the [IndicBERT-v1 repo](https://github.com/AI4Bharat/Indic-BERT-v1). To find the source of each dataset, please refer the [citations](#citations).

### Tasks

#### News Category Classification

Predict the genre of a given news article. The dataset contains around 125k news articles across 9 Indian languages. Example:

*Article Snippet*:

```
கர்நாடக சட்டப் பேரவையில் வெற்றி பெற்ற எம்எல்ஏக்கள் இன்று பதவியேற்றுக் கொண்ட நிலையில் , காங்கிரஸ் எம்எல்ஏ ஆனந்த் சிங் க்கள் ஆப்சென்ட் ஆகி அதிர்ச்சியை ஏற்படுத்தியுள்ளார் . உச்சநீதிமன்ற உத்தரவுப்படி இன்று மாலை முதலமைச்சர் எடியூரப்பா இன்று நம்பிக்கை வாக்கெடுப்பு நடத்தி பெரும்பான்மையை நிரூபிக்க உச்சநீதிமன்றம் உத்தரவிட்டது . 
```

*Category*: Politics

*Datasets*

- AI4Bharat
- Soham Articles Genre Classification
- iNLTK Headlines Genre Classifcation
- BBC News Articles

----

#### Headline Prediction

 Predict the correct headline for a news article from a given list of four candidate headlines. The dataset contains around 880k examples across 11 Indian languages. Example:

*News Article:*

     ರಾಷ್ಟ್ರೀಯ\nಪುಣೆ: 23 ವರ್ಷದ ಇನ್ಫೋಸಿಸ್ ಮಹಿಳಾ ಟೆಕ್ಕಿಯೊಬ್ಬರನ್ನು ನಡು ರಸ್ತೆಯಲ್ಲಿಯೇ ಮಾರಾಕಾಸ್ತ್ರಗಳಿಂದ ಬರ್ಬರವಾಗಿ ಹತ್ಯೆ ಮಾಡಿರುವ ಘಟನೆ ಪುಣೆಯಲ್ಲಿ ಶನಿವಾರ ರಾತ್ರಿ ನಡೆದಿದೆ.\nಅಂತರ ದಾಸ್ ಕೊಲೆಯಾದ ಮಹಿಳಾ ಟೆಕ್ಕಿಯಾಗಿದ್ದಾರೆ. ಅಂತರಾ ಅವರು ಪಶ್ಚಿಮ ಬಂಗಾಳದ ಮೂಲದವರಾಗಿದ್ದಾರೆ. ಕಳೆದ ರಾತ್ರಿ 8.00 ಗಂಟೆ ಸುಮಾರಿಗೆ ಕೆಲಸ ಮುಗಿಸಿ ಮನೆಗೆ ತೆರಳುತ್ತಿದ್ದ ಸಂದರ್ಭದಲ್ಲಿ ಅಂತರಾ ಅವರ ಮೇಲೆ ದಾಳಿ ಮಾಡಿರುವ ದುಷ್ಕರ್ಮಿಗಳು ಮಾರಾಕಾಸ್ತ್ರಗಳಿಂದ ಹಲ್ಲೆ ನಡೆಸಿದ್ದಾರೆಂದು ಪೊಲೀಸರು ಹೇಳಿದ್ದಾರೆ.\nದಾಳಿ ನಡೆಸಿದ ನಂತರ ರಕ್ತದ ಮಡುವಿನಲ್ಲಿ ಬಿದ್ದು ಒದ್ದಾಡುತ್ತಿದ್ದ ಅಂತರಾ ಅವರನ್ನು ಸ್ಥಳೀಯರು ಆಸ್ಪತ್ರೆಗೆ ದಾಳಸಿದ್ದಾರೆ. ಆದರೆ, ಆಸ್ಪತ್ರೆಗೆ ದಾಖಲಿಸುವಷ್ಟರಲ್ಲಿ ಅಂತರಾ ಅವರು ಸಾವನ್ನಪ್ಪಿದ್ದಾರೆಂದು ಅವರು ಹೇಳಿದ್ದಾರೆ.\nಪ್ರಕರಣ ದಾಖಲಿಸಿಕೊಂಡಿರುವ ಪೊಲೀಸರು ತನಿಖೆ ಆರಂಭಿಸಿದ್ದಾರೆ",

* *Candidate 1*: ಇನ್ಫೋಸಿಸ್ ಮಹಿಳಾ ಟೆಕ್ಕಿಯ ಬರ್ಬರ ಹತ್ಯೆ    *[correct answer]*
* *Candidate 2:* ಮಾನಸಿಕ ಅಸ್ವಸ್ಥೆ ಮೇಲೆ  ಮಕ್ಕಳ ಕಳ್ಳಿ ಎಂದು ಭೀಕರ ಹಲ್ಲೆ
* *Candidate 3:* ಕಸಬ ಬೆಂಗ್ರೆಯಲ್ಲಿ ಮುಸುಕುಧಾರಿಗಳ ತಂಡದಿಂದ ಮೂವರು ಯುವಕರ ಮೇಲೆ ಹಲ್ಲೆ : ಓರ್ವ ಗಂಭೀರ
* *Candidate 4:* ಕಣಿವೆ ರಾಜ್ಯದಲ್ಲಿ mobile ಬಂದ್, ಪ್ರಿಂಟಿಂಗ್ ಪ್ರೆಸ್ ಮೇಲೆ ದಾಳಿ

*Datasets*

- AI4Bharat

----


#### Wikipedia Section Title Prediction

Predict the correct title for a Wikipedia section from a given list of four candidate titles. The dataset has 400k examples across 11 Indian languages.

*Section Text*:

```
2005માં, જેકમેન નિર્માણ કંપની, સીડ પ્રોડકશન્સ ઊભી કરવા તેના લાંબાસમયના મદદનીશ જહોન પાલેર્મો સાથે જોડાયા, જેમનો પ્રથમ પ્રોજેકટ 2007માં વિવા લાફલિન હતો. જેકમેનની અભિનેત્રી પત્ની ડેબોરા-લી ફર્નેસ પણ કંપનીમાં જોડાઈ, અને પાલેર્મોએ પોતાના, ફર્નેસ અને જેકમેન માટે “ યુનિટી ” અર્થવાળા લખાણની આ ત્રણ વીંટીઓ બનાવી.[૨૭] ત્રણેયના સહયોગ અંગે જેકમેને જણાવ્યું કે “ મારી જિંદગીમાં જેમની સાથે મેં કામ કર્યું તે ભાગીદારો અંગે ડેબ અને જહોન પાલેર્મો અંગે હું ખૂબ નસીબદાર છું. ખરેખર તેથી કામ થયું. અમારી પાસે જુદું જુદું સાર્મથ્ય હતું. હું તે પસંદ કરતો હતો. I love it. તે ખૂબ ઉત્તેજક છે. ”[૨૮]ફોકસ આધારિત સીડ લેબલ, આમન્ડા સ્કિવેઈટઝર, કેથરિન ટેમ્બલિન, એલન મંડેલબમ અને જોય મરિનો તેમજ સાથે સિડની આધારિત નિર્માણ કચેરીનું સંચાલન કરનાર અલાના ફ્રીનો સમાવેશ થતાં કદમાં વિસ્તૃત બની. આ કંપીનોનો ઉદ્દેશ જેકમેનના વતનના દેશની સ્થાનિક પ્રતિભાને કામે લેવા મધ્યમ બજેટવાળી ફિલ્મો બનાવવાનો છે. 
```

* *Candidate 1:* એકસ-મેન
* *Candidate 2:* કારકીર્દિ
* *Candidate 3:* નિર્માણ કંપન [*correct answer*]
* *Candidate 4:* ઓસ્ટ્રેલિય

*Datasets*

- AI4Bharat

----


#### Cloze-style Question Answering

Given a text with an entity randomly masked, the task is to predict that masked entity from a list of 4 candidate entities. The dataset contains around 239k examples across 11 languages. Example:

*Text*

```
ਹੋਮੀ ਭਾਬਾ ਦਾ ਜਨਮ 1949 ਈ ਨੂਂ ਮੁੰਬਈ ਵਿੱਚ ਪਾਰਸੀ ਪਰਿਵਾਰ ਵਿੱਚ ਹੋਇਆ । ਸੇਂਟ ਮੇਰੀ ਤੋਂ ਮੁਢਲੀ ਸਿਖਿਆ ਪ੍ਰਾਪਤ ਕਰਕੇ ਉਹ ਬੰਬੇ ਯੂਨੀਵਰਸਿਟੀ ਗ੍ਰੈਜੁਏਸ਼ਨ ਲਈ ਚਲਾ ਗਿਆ । ਇਸ ਤੋਂ ਬਾਅਦ ਉਹ ਉਚੇਰੀ ਸਿਖਿਆ ਲਈ <MASK> ਚਲਾ ਗਿਆ । ਉਸਨੇ ਓਥੇ ਆਕਸਫੋਰਡ ਯੂਨੀਵਰਸਿਟੀ ਤੋਂ ਐਮ.ਏ ਅਤੇ ਐਮ ਫਿਲ ਦੀਆਂ ਡਿਗਰੀਆਂ ਪ੍ਰਾਪਤ ਕੀਤੀਆਂ । ਤਕਰੀਬਨ ਦਸ ਸਾਲ ਤਕ ਉਸਨੇ ਸੁਸੈਕਸ ਯੂਨੀਵਰਸਿਟੀ ਦੇ ਅੰਗਰੇਜ਼ੀ ਵਿਭਾਗ ਵਿੱਚ ਬਤੌਰ ਲੈਕਚਰਾਰ ਕਾਰਜ ਨਿਭਾਇਆ । ਇਸਤੋਂ ਇਲਾਵਾ ਹੋਮੀ ਭਾਬਾ ਪੈਨਸੁਲਵੇਨਿਆ , ਸ਼ਿਕਾਗੋ ਅਤੇ ਅਮਰੀਕਾ ਦੀ ਹਾਰਵਰਡ ਯੂਨੀਵਰਸਿਟੀ ਵਿੱਚ ਵੀ ਪ੍ਰੋਫ਼ੇਸਰ ਦੇ ਆਹੁਦੇ ਤੇ ਰਿਹਾ ।
```

* *Candidate 1*: ਬਰਤਾਨੀਆ *[correct answer]*
* *Candidate 2*: ਭਾਰਤ
* *Candidate 3*: ਸ਼ਿਕਾਗੋ
* *Candidate 4*: ਪਾਕਿਸਤਾਨ

*Datasets*

- AI4Bharat

----


#### Named Entity Recognition

Recognize entities and their coarse types in a sequence of words. The dataset contains around 787k examples across 11 Indian languages.

*Example*:


|     |     |     |     |     |     |     |     |     |     |
|-------------|-------------|-------------|-------------|-------------|-------------|-------------|-------------|-------------|-------------|
| **Token** | चाणक्य | पुरी   | को   | यहाँ  | देखने  | हेतु   | यहाँ  | क्लिक | करें   |
| **Type** | B-LOC | I-LOC | O    | O    | O    | O    | O    | O    | O    |

*Datasets*

- WikiAnnNER

----



#### Cross-lingual Sentence Retrieval

Given a sentence in language $L_1$ the task is to retrieve its translation from a set of candidate sentences in language $L_2$. The dataset contains around 39k parallel sentence pairs across 8 Indian languages. Example:

*Input Sentence*

```
In the health sector the nation has now moved ahead from the conventional approach.
```

*Retrieve the following translation from a set of 4886 sentences:*

```
ആരോഗ്യമേഖലയില് ഇന്ന് രാജ്യം പരമ്പരാഗത രീതികളില് നിന്ന് മുന്നേറിക്കഴിഞ്ഞു.
```

*Datasets*

- CVIT-Mann ki baat test set 

----


#### Natural Language Inference

*Datasets*

- AI4Bharat Winnograd Natural Language Inference (WNLI)
- AI4Bharat Choice of Plausible Alternatives (COPA)

These are translations of the WNLI and COPA datasets into some Indian languages.

----

#### Sentiment Analysis

*Datasets*

- IITP Movie Reviews Sentiment 
- IITP Product Reviews
- ACTSA Sentiment Classifcation

----

#### Discourse Analysis

*Datasets*

- MIDAS Discourse

----

#### Paraphrase Detection

*Datasets*

* Amrita Exact Paraphrase Detection
* Amrita Rough Paraphrase Detection

----

### Citing

If you are using IndicGLUE, please cite the following article: 

```
@inproceedings{kakwani2020indicnlpsuite,
    title={{IndicNLPSuite: Monolingual Corpora, Evaluation Benchmarks and Pre-trained Multilingual Language Models for Indian Languages}},
    author={Divyanshu Kakwani and Anoop Kunchukuttan and Satish Golla and Gokul N.C. and Avik Bhattacharyya and Mitesh M. Khapra and Pratyush Kumar},
    year={2020},
    booktitle={Findings of EMNLP},
}
``` 

If you are using IndicGLUE and additional evaluation datasets in your work, then we request you to use the following detailed citation text so that the original authors of the datasets also get credit for their work. As more authors contribute to this benchmark we will add their references also to the below text.


<div style=" font-size: .85em; line-height: 1.45; text-align:left; padding: 1rem;">
We use the IndicGLUE dataset <code>\cite{kakwani2020indicnlpsuite}</code> which is an evaluation benchmark containing datasets for NLU tasks in Indian languages. Some of these datasets were built from Wikipidea and IndicCorp <code>\cite{kakwani2020indicnlpsuite}</code>. In addition, it also contains other publicly available datasets for cross-lingual similarity <code>\cite{siripragrada-etal-2020-multilingual}</code>, named entity recognition <code>\cite{pan-etal-2017-cross}</code>, paraphrase detection <code>\cite{Kumar2016DPILFIRE2016OO}</code>, discourse analysis <code>\cite{Dhanwal2020AnAD}</code>, sentiment analysis <code>\cite{cicling/Akhtar16}</code>, <code>\cite{DBLP:conf/coling/Akhtar0EB16}</code>, <code>\cite{mukku-mamidi-2017-actsa}</code> and genre classification <code>\footnote{https://github.com/goru001/inltk}</code> <code>\footnote{https://www.kaggle.com/csoham/classification-bengali-news-articles-indicnlp}</code> <code>\footnote{https://github.com/NirantK/hindi2vec/releases/tag/bbc-hindi-v0.1}</code>. It also contains translations of the original WNLI <code>\cite{Levesque2011TheWS}</code> and COPA <code>\cite{Gordon2011SemEval2012T7}</code> datasets in 3 Indian languages.
</div>

The bibtex entries for the above sources is available [here](https://indicnlp.ai4bharat.org/papers/indic-glue.bib).

----


