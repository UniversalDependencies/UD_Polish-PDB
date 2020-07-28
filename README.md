# Summary

The Polish PDB-UD treebank is based on the Polish Dependency Bank 2.0 (PDB 2.0), created at the Institute of Computer Science, Polish Academy of Sciences in Warsaw. The PDB-UD treebank is an extended and corrected version of the Polish SZ-UD treebank (the release 1.2 to 2.3).


# Introduction

The PDB-UD treebank consists of 22,152 sentences (350K tokens). It contains all 8K sentences of the Polish UD-SZ treebank and further 14K unique sentences. The additional sentences enclose linguistic phenomena that did not occur or were not annotated (e.g. relative clauses, reported speech) in the UD-SZ trees. The PDB-UD treebank contains enhanced graphs, i.e. trees with the enhanced edges encoding the shared dependents and the shared governors of coordinated conjuncts (9141 PDB-UD trees contain enhanced edges).

The morphological, syntactic and semantic annotation of the PDB-UD treebank is created through a conversion of PDB 2.0 data. The conversion procedure has been designed and implemented by Alina Wróblewska partly based on the conversion of the UD-SZ trees.

# Data Split

The PDB-UD treebank contains sentences from Polish National Corpus, CDSCorpus, parallel corpora (e.g. Europarl, OPUS, and Pelcra Prallel Corpus) and other sources (e.g. literature). The PDB-UD treebank is divided into three parts:

* training: 17,722 trees (281,736 tokens),
* test: 2215 trees (33,617 tokens),
* development: 2215 trees (34,683).

The procedure of assigning dependency trees to particular data sets is generally random while maintaining the proportion of data from individual sources. There is one constraint on the dividing procedure: if a sentence occurs in the test, dev or train subset of the Polish LFG-UD treebank, this sentence is assigned to the test, dev or train set of the Polish PDB-UD treebank, respectively.

# License/Copyright

Universal Polish Dependency Bank © 2019 by Alina Wróblewska, Institute of Computer Science, Polish Academy of Sciences.

The Polish PDB-UD treebank is licensed under [CC BY-NC-SA 4.0](http://creativecommons.org/licenses/by-nc-sa/4.0/).


## History Note

The earlier release of the Polish UD treebank, i.e. the UD-SZ treebank, was first converted to the Prague dependency style as a part of HamleDT;
then it was automatically converted to Universal Dependencies (HamleDT 3.0, 2015). The first
release of Universal Dependencies that includes this treebank is UD v1.2 in November 2015. It is
essentially the HamleDT conversion but the data is not identical to HamleDT 3.0 because the
conversion procedure has been further improved.

## References

If you use the Polish PDB-UD treebank, you are encouraged to cite this paper:

<pre>
@inproceedings{pl,
  author    = {Wr{\'o}blewska, Alina},
  title     = {Extended and Enhanced Polish Dependency Bank in Universal Dependencies Format},
  booktitle = {Proceedings of the Second Workshop on Universal Dependencies (UDW 2018)},
  editor    = {de Marneffe, Marie-Catherine and Lynn, Teresa and Schuster, Sebastian},
  pages     = {173--182},
  publisher = {Association for Computational Linguistics},
  year      = {2018}
}
</pre>

* http://git.nlp.ipipan.waw.pl/alina/PDBUD
* http://zil.ipipan.waw.pl/PDB
* http://ufal.mff.cuni.cz/hamledt ... HamleDT
* http://ufal.mff.cuni.cz/treex ... Treex is the software used for conversion
* http://ufal.mff.cuni.cz/interset ... Interset was used to convert POS tags and features

# Acknowledgments

We would like to thank all of the contributors of the original Polish Dependency Bank 2.0. The development of the PDB-UD treebank was founded by the Polish Ministry of Science and Higher Education as part of the investment in the CLARIN-PL research infrastructure.


# Changelog

* 2019-11-15 v2.5
  * Duplicate sentences are removed.
  * The treebank is divided anew into train, test and dev subsets.
  * The bugs fixed in the original PDB trees resulted in modifications to the UD trees.
  * Fixed nominal dependents of nouns that were attached as obl:arg; correct: nmod:arg.
  * Emphasizing words are annotated as advmod:emph.
* 2019-05-15 v2.4
  * Repository renamed from UD_Polish-SZ to UD_Polish-PDB.
  * Completely new conversion of the data.
  * In addition to the texts from “Składnica zależnościowa” 0.5, new data from PDB was added.
  * License changed from GNU GPL 3.0 to CC BY-NC-SA 4.0.
* 2018-04-15 v2.2
  * Repository renamed from UD_Polish to UD_Polish-SZ.
* 2017-11-15 v2.1
  * Prepositional objects are now “obl:arg” instead of “obj”.
  * Instrumental phrases for demoted agents in passives are now “obl:agent”.
* 2017-03-01 v2.0
  * Converted to UD v2 guidelines.
  * Reconsidered PRON vs. DET.
  * Improved advmod vs. obl distinction.
  * Participles moved from verbs to adjectives.
* 2016-05-15 v1.3
  * Fixed adverbs that were attached as nmod; correct: advmod.
  * Conditional auxiliary "by" changed from PART to AUX (and features added).
  * Demonstrative, interrogative, indefinite, total and negative PRON/DET separated from NOUN/ADJ.
  * Proper nouns (PROPN) separated from NOUN.
  * Past tense / l-participles changed from VerbForm=Fin to VerbForm=Part.
  * Verbal nouns (VerbForm=Ger) retagged and relemmatized from VERB to NOUN.


<pre>
=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v1.2
License: CC BY-NC-SA 4.0
Includes text: yes
Genre: fiction nonfiction news
Lemmas: converted from manual
UPOS: converted from manual
XPOS: manual native
Features: converted from manual
Relations: converted from manual
Contributors: Wróblewska, Alina; Zeman, Daniel; Mašek, Jan; Rosa, Rudolf
Contributing: elsewhere
Contact: alina@ipipan.waw.pl
===============================================================================
</pre>
