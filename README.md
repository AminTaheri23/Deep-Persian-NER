# Deep Persian NER
Persian Named Entity Classification from Arman Rayan Sharif corpus with deep learning

## About
In this project, your task is to build and train a model to recognize Named Entities from a sentence. This model should give a tag to each word from a sentence. A classical application is Named Entity Recognition (NER)

## Named Entity Recognition (NER)
Named Entity Recognition is a process where an algorithm takes a string of text (sentence or paragraph) as input and identifies relevant nouns (people, places, organizations, and...) that are mentioned in that string. Here is an example:

```
John  went to New   York  to interview with Microsoft 
B-PER O    O  B-LOC I-LOC O  O         O    B-ORG
```

## ArmanPersoNERCorpus
https://github.com/HaniehP/PersianNER
This dataset includes 250,015 tokens and 7,682 Persian sentences in total. Each file contains one token, along with its manually annotated named-entity tag, per line. Each sentence is separated with a newline. The NER tags are in IOB format.

The IOB format (short for inside, outside, beginning) is a common tagging format for tagging tokens in a chunking task in computational linguistics (ex. named entity recognition)

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
1. person
2. organization (such as banks, ministries, embassies, teams, nationalities, networks and publishers)
3. location (such as cities, villages, rivers, seas, gulfs, deserts and mountains)
4. facility (such as schools, universities, research centers, airports, railways, bridges, roads, harbors, stations, hospitals, parks, zoos and cinemas)
5. product (such as books, newspapers, TV shows, movies, airplanes, ships, cars, theories, laws, agreements and religions)
6. event (such as wars, earthquakes, national holidays, festivals and conferences)
7. other are the remaining tokens

## Misc.
This was the final project for [FanAsa Academy's DeepNLP course](http://fanasa.co/academy.php) that held in [Summer of 1398(2019)](https://evand.com/events/%DA%A9%D8%A7%D8%B1%D8%A8%D8%B1%D8%AF%D9%87%D8%A7%DB%8C-%DB%8C%D8%A7%D8%AF%DA%AF%DB%8C%D8%B1%DB%8C-%D8%B9%D9%85%DB%8C%D9%82-%D8%AF%D8%B1-%D9%BE%D8%B1%D8%AF%D8%A7%D8%B2%D8%B4-%D9%85%D8%AA%D9%86-deep-nlp-6960592#event-cover). 

Instructors: Reza Vasefi - Fatemeh Mashhadi
