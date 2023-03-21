# HuRTE
This is the home repository for the Hungarian version of the Recognizing Textual Entailment datasets. This dataset is also part of the Hungarian Language Understanding Evaluation Benchmark Kit [HuLU](hulu.nytud.hu). The corpus was created by translating and re-annotating the instances of the RTE datasets that are part of the GLUE benchmark. 

## Data

The files are in the 'data' folder. The dataset contains 4 504 instances. These contain a (sometimes multi-sentence) premise and a one-sentence hypothesis, and the task is to decide whether the former entails the latter or not. The task is binary classification.

The train, validation and test sets contain 2 131, 242 and 2 131 instances, respectively. The test set is distributed without the labels; to evaluate your model please contact us (ligeti-nagy.noemi@nytud.hu) or visit [HuLU's website](hulu.nytud.hu) for an automatic evaluation. The metric of the evaluation is MCC.

## Data format

The data files are in json format. The keys are the following:

`id`: unique id of the instances;

`premise`: the premise;

'hypothesis': the hypothesis;

`label`: "1", if the premise entails the hypothesis, "0" otherwise.


## License and usage

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/).

## Citation

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
  publisher = {Szegedi Tudományegyetem, Informatikai Intézet}
}
```
and 

Bar-Haim, R., Dagan, I., Dolan, B., Ferro, L., Giampiccolo, D., Magnini, B., Szpektor, I.: The Second PASCAL Recognising Textual Entailment Challenge. In: Proceedings of the Second PASCAL Challenges Workshop on Recognizing Textual Entailment, Venice, Italy. pp. 1–9 (2006).

```bibtex
@InProceedings{rte2,
author="Roy Bar-Haim and Ido Dagan and Bill Dolan and Lisa Ferro and Danilo Giampiccolo and Bernardo Magnini and Idan Szpektor",
title="{The Second PASCAL Recognising Textual Entailment Challenge}",
booktitle="Proceedings of the Second PASCAL Challenges Workshop on Recognizing Textual Entailment, Venice, Italy",
year="2006",
pages="1--9"
}
```

and 

Giampiccolo, D., Magnini, B., Dagan, I., Dolan, B.: The Third PASCAL Recognizing Textual Entailment Challenge. In: Proceedings of the ACL-PASCAL Workshop on Textual Entailment and Paraphrasing. p. 1–9. RTE ’07 (2007).

```bibtex
@inproceedings{rte3,
author = {Giampiccolo, Danilo and Magnini, Bernardo and Dagan, Ido and Dolan, Bill},
title = {{The Third PASCAL Recognizing Textual Entailment Challenge}},
year = {2007},
abstract = {This paper presents the Third PASCAL Recognising Textual Entailment Challenge (RTE-3), providing an overview of the dataset creating methodology and the submitted systems. In creating this year's dataset, a number of longer texts were introduced to make the challenge more oriented to realistic scenarios. Additionally, a pool of resources was offered so that the participants could share common tools. A pilot task was also set up, aimed at differentiating unknown entailments from identified contradictions and providing justifications for overall system decisions. 26 participants submitted 44 runs, using different approaches and generally presenting new entailment models and achieving higher scores than in the previous challenges.},
booktitle = {Proceedings of the ACL-PASCAL Workshop on Textual Entailment and Paraphrasing},
pages = {1–9},
location = {Prague, Czech Republic},
series = {RTE '07}
}
```

and 

Bentivogli, L., Dagan, I., Dang, H.T., Giampiccolo, D., Magnini, B.: The Fifth PASCAL Recognizing Textual Entailment Challenge. In: Proceedings of the TAC Workshop (2009).

```bibtex
@inproceedings{rte5,
author = {Luisa Bentivogli and Ido Dagan and Hoa Trang Dang and Danilo Giampiccolo and Bernardo Magnini},
title = {{The Fifth PASCAL Recognizing Textual Entailment Challenge}},
year = {2009},
booktitle = {Proceedings of the TAC Workshop},
location = {Gaithersburg, MD, USA}
}
```
