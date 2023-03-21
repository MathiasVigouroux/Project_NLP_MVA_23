# HuWNLI
Anaphora resolution datasets for Hungarian formulated as an inference task

This is the repository for the Hungarian datasets of anaphora resolution, designed as a sentence pair classification task of natural language inference.
As a first version, the repo contains the translation of the Winograd schemata formatted as an inference task. A Winograd schema is a pair of sentences that differ in only one or two words and that contain an ambiguity that is resolved in opposite ways in the two sentences and requires the use of world knowledge and reasoning for its resolution (Levesque et al. 2012). This dataset is also part of the Hungarian Language Understanding Evaluation Benchmark Kit [HuLU](hulu.nytud.hu). 

The [HuWS corpus](github.com/nytud/HuWSC) was created by translating and manually curating the original English Winograd schemata. The NLI format published here was created by replacing the ambiguous pronoun with each possible referent in the schemata (the method is described in GLUE's paper, Wang et al. 2019). We extended the set of sentence pairs derived from the schemata by the translation of the sentence pairs that - together with the Winograd schema sentences - build up the WNLI dataset of GLUE. 

## Dataset Structure

### Data Instances

For each instance, there is an orig_id, an id, two sentences and a label.

An example:

```
{"orig_id": "4",
 "id": "4",
 "sentence1": "A férfi nem tudta felemelni a fiát, mert olyan nehéz volt.",
 "sentence2": "A fia nehéz volt.",
 "Label": "1"
}
```

### Data Fields
- orig_id: the original id of this sentence pair (more precisely, its English counterpart's) in GLUE's WNLI dataset;

- id: unique id of the instances;

- sentence1: the premise;

- sentence2: the hypothesis;  

- Label: "1" if sentence2 is entailed by sentence1, and "0" otherwise.

The data is distributed in three splits: training set (562), development set (59) and test set (134). The splits follow GLUE's WNLI's splits, but contain less instances as many sentence pairs had to be thrown away for being untranslatable to Hungarian. 
The test set's sentence pairs are translated from GLUE's WNLI's test set. This set was distributed without labels. 3 annotators annotated the Hungarian sentence pairs. The test set of HuWNLI is also distributed without labels.
To evaluate your model, please [contact us](mailto:ligeti-nagy.noemi@nytud.hu), or check [HuLU's website](hulu.nytud.hu) for an automatic evaluation (this feature is under construction at the moment). 
### Licensing Information

HuWNLI is released under the CC-BY-SA-4.0 License.


### Citation Information

If you use this resource or any part of its documentation, please refer to:

Vadász, N., & Ligeti-Nagy, N. (2022). Winograd schemata and other datasets for anaphora resolution in Hungarian, Acta Linguistica Academica, 69(4), in press.
```
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

Levesque, Hector, Davis, Ernest, Morgenstern, Leora (2012) The winograd schema challenge. In: Thirteenth International Conference on the Principles of Knowledge Representation and Reasoning.

```
@inproceedings{levesque2012winograd,
  title={The Winograd Schema Challenge},
  author={Levesque, Hector and Davis, Ernest and Morgenstern, Leora},
  booktitle={Thirteenth International Conference on the Principles of Knowledge Representation and Reasoning},
  year={2012},
  organization={Citeseer}
}
```
