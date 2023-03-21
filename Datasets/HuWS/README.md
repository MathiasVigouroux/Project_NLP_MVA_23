# HuWS

This is the home repository for the Hungarian set of the Winograd schemas. A Winograd schema is a pair of sentences that differ in only one or two words and that contain an ambiguity that is resolved in opposite ways in the two sentences and requires the use of world knowledge and reasoning for its resolution (Levesque et al. 2012). This dataset is also part of the Hungarian Language Understanding Evaluation Benchmark Kit [HuLU](hulu.nytud.hu). The corpus was created by translating and manually curating the original English Winograd schemata.

## Dataset Structure

### Data Instances

For each instance, there is an id, a sentence, a question and two possible answers, and a correct answer. 

An example:

```

{"ID": "1",
 "Sent": "A városi tanácstagok nem adtak engedélyt a tüntetőknek, mert kerülték az erőszakot.",
 "Question": "Kik kerülték az erőszakot?",
 "Answer1": "a városi tanácstagok",
 "Answer2": "a tüntetők",
 "CorrectAnswer": "a városi tanácstagok"
}

```

### Data Fields
- id: unique id of the instances;
- Sent: the sentence, which is a translation of the original English sentence;
- Question: a manually formed question;  
- Answer1: the first possible reference;
- Answer2: the second possible reference;
- CorrectAnswer: the correct answer :)

## Dataset Creation

The data is a translation of the English Winograd schemas. Each schema was translated by a human translator. Each translation was manually checked and further refined by another annotator. Each schema was manually curated by a linguistic expert. 

## Additional Information

### Licensing Information

HuWSC is released under the CC-BY-SA 4.0 license.

### Citation Information

If you use this resource or any part of its documentation, please refer to:

Ligeti-Nagy, N., Ferenczi, G., Héja, E., Jelencsik-Mátyus, K., Laki, L. J., Vadász, N., Yang, Z. Gy. and Váradi, T. (2022) HuLU: magyar nyelvű benchmark adatbázis kiépítése a neurális nyelvmodellek kiértékelése céljából [HuLU: Hungarian benchmark dataset to evaluate neural language models]. In: Berend, G., Gosztolya, G. and Vincze, V. (eds), XVIII. Magyar Számítógépes Nyelvészeti Konferencia. Szeged, Szegedi Tudományegyetem, Informatikai Intézet. 431–446.

```bibtex
@inproceedings{ligetinagy2022hulu,
  title={HuLU: magyar nyelvű benchmark adatbázis kiépítése a neurális nyelvmodellek kiértékelése céljából},
  author={Ligeti-Nagy, N. and Ferenczi, G. and Héja, E. and Jelencsik-Mátyus, K. and Laki, L. J. and Vadász, N. and Yang, Z. Gy. and Váradi, T.},
  booktitle={XVIII. Magyar Számítógépes Nyelvészeti Konferencia},
  year={2022},
  pages = {431--446},
  editors = {Berend, G. and Gosztolya, G. and Vincze, V.},
  address = {Szeged},
  publisher = {JATEPress}
}
```
and to:

Vadász, N., & Ligeti-Nagy, N. (2022). Winograd schemata and other datasets for anaphora resolution in Hungarian, Acta Linguistica Academica, 69(4), in press.

```bibtex
@article{vadaszligeti2022actawinograd,
      author = "Noémi Vadász and Noémi Ligeti-Nagy",
      title = "Winograd schemata and other datasets for anaphora resolution in Hungarian",
      journal = "Acta Linguistica Academica",
      year = "2022",
      publisher = "Akadémiai Kiadó",
      address = "Budapest, Hungary",
      volume = "69",
      number = "4",
      note = "In press."
}
```
and to:
Levesque, Hector, Davis, Ernest, Morgenstern, Leora (2012) he winograd schema challenge. In: Thirteenth International Conference on the Principles of Knowledge Representation and Reasoning.

```bibtex
@inproceedings{levesque2012winograd,
  title={The winograd schema challenge},
  author={Levesque, Hector and Davis, Ernest and Morgenstern, Leora},
  booktitle={Thirteenth International Conference on the Principles of Knowledge Representation and Reasoning},
  year={2012},
  organization={Citeseer}
}
```
