# Deep Persian NER
<p align="center">
<img src="https://amintaheri23.github.io/img/portfolio/ner.png">
</p>
Persian Named Entity Classification from Arman Rayan Sharif corpus with deep learning

## About
In this project, your task is to build and train a model to recognize Named Entities from a sentence. This model should give a tag to each word from a sentence. A classical application is Named Entity Recognition (NER). main file is [here](https://github.com/AminTaheri23/Deep-Persian-NER/blob/master/Amin_Taheri_DeepNLp_Final_Project.ipynb)

for replicating results you will need to download PersianNER dataset from [this section](https://github.com/AminTaheri23/Deep-Persian-NER#armanpersonercorpus) (link below in ArmanPersoNERCorpus and you need to change path in ipynb file) and you also need a fastext pretrained model. my fastext model is [here](https://drive.google.com/file/d/1-2xzg-26qqp59PUql_KMWQ7gLli11x_h/view?usp=sharing). you can add it to your drive and use the correct path to address it. (it is recommended that to use this ipynb file in _Google Colab_)

## Named Entity Recognition (NER)
Named Entity Recognition is a process where an algorithm takes a string of text (sentence or paragraph) as input and identifies relevant nouns (people, places, organizations, and...) that are mentioned in that string. Here is an example:

```
John  went to New   York  to interview with Microsoft 
B-PER O    O  B-LOC I-LOC O  O         O    B-ORG
```

## ArmanPersoNERCorpus
https://github.com/HaniehP/PersianNER

This dataset includes 250,015 tokens and 7,682 Persian sentences in total. Each file contains one token, along with its manually annotated named-entity tag, per line. Each sentence is separated with a newline. The NER tags are in IOB format.

**The IOB format (short for inside, outside, beginning) is a common tagging format for tagging tokens in a chunking task in computational linguistics (ex. named entity recognition)**

An example with IOB format:

```
John B-PER
lives O
in O
New B-LOC
York I-LOC
. O
 
This O
is O
another O
sentence
```

## Dataset Structure
In ArmanPersoNERCorpus, NEs are categorized into six classes:

1. person `B-pers`,`I-pers`
2. organization `B-org`,`I-org`(such as banks, ministries, embassies, teams, nationalities, networks and publishers)
3. location `B-loc`,`I-loc`(such as cities, villages, rivers, seas, gulfs, deserts and mountains)
4. facility `B-fac`,`I-fac`(such as schools, universities, research centers, airports, railways, bridges, roads, harbors, stations, hospitals, parks, zoos and cinemas)
5. product `B-pro`, `I-pro` (such as books, newspapers, TV shows, movies, airplanes, ships, cars, theories, laws, agreements and religions)
6. event `B-event`,`I-event`(such as wars, earthquakes, national holidays, festivals and conferences)
7. other `O` are the remaining tokens

## Misc.
This was the final project for [FanAsa Academy's DeepNLP course](http://fanasa.co/academy.php) that held in [Summer of 1398(2019)](https://evand.com/events/%DA%A9%D8%A7%D8%B1%D8%A8%D8%B1%D8%AF%D9%87%D8%A7%DB%8C-%DB%8C%D8%A7%D8%AF%DA%AF%DB%8C%D8%B1%DB%8C-%D8%B9%D9%85%DB%8C%D9%82-%D8%AF%D8%B1-%D9%BE%D8%B1%D8%AF%D8%A7%D8%B2%D8%B4-%D9%85%D8%AA%D9%86-deep-nlp-6960592#event-cover). 

Instructors: Reza Vasefi - Fatemeh Mashhadi
