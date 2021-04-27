# AREEB: ARabic Embeddings Evaluation Benchmark

- [Description](#description)
- [Dataset](#dataset)
- [Citation](#citation)

## Description

AREEB is a benchmark to evaluate word embedding models for Arabic language. The benchmarks that have been used thus far in Arabic have mimicked those in English. AREEB benchmark is one that is designed to reflect linguistic patterns in both Contemporary Arabic and Classical Arabic. The analogy items we included in this benchmark are chosen in a transparent manner such that they capture the major features of nouns and verbs; derivational and inflectional morphology; high, middle, and low frequency patterns and lexical items; and morphosemantic, morphosyntactic, and semantic dimensions of the language. 
All categories included in this benchmark are carefully selected to ensure proper representation of the language. The benchmark consists of 45 roots of the trilateral, all-consonantal, and semivowel-inclusive types; two morphosemantic patterns (>fEala  and  AstafEala); three derivations (the verbal noun, active participle, and masculine-feminine contrast); and morphosyntactic transformations (perfect and imperfect verbs conjugated for the pronouns: she, he, and they); and lexical semantics (synonyms, antonyms, and hyponyms of nouns, verbs, and adjectives), as well as capital cities and currencies. All categories include an equal proportion of high, medium, and low frequency items.

The complete benchmark consists of 44 tests, each consisting of several word pairs. Every pair is evaluated in word analogy tests.
The process of testing involves studying the word analogy relationship between each pair of words, in each file, against the remaining pairs in the same file. The objective is to recover the missing word. This process is repeated in each file for each benchmark indicator. This process is similar to what Mikolov et al.(2013) and Elrazzaz (2017} did for evaluating word embeddings. In order to recover the missing word, it is suggested here that the top-5 matches be considered, rather than the top candidate as the case is for English. This is because Arabic derivational and inflectional nature allows the top candidate to appear in a word form that might differ from the targeted form by a one letter clitic or affix. Koper, et al (2015) lend support to our recommendation with their finding that the morphological richness of German makes the prediction of analogies more difficult; thus, the overall performance of embeddings in German are lower than their counterparts in English. 

The benchmark consists of:

| Indicator         | n1 	| n2  |
|------------------	|---- |----	|
| Morphosyntax      | 28 	|  6  |
| Morphosemantics   | 11 	|  5	|
| Semantics       	| 5   |  5	|

where n1 and n2 are the total number of testing files in the complete and minimal datasets, respectively.

## Dataset

- data/
                      
  - Compete testing dataset: is a collection of 44 files to test each of the indicators.
                     
  - Minimal testing dataset: is a satisfactory subset of 18 files to test each of the indicators.
                     
## Citation

Please cite the following paper if you decise to use the dataset:

    TBA
