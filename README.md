# Summary

The UD Polish treebank is based on “Składnica zależnościowa” (the Polish dependency treebank)
version 0.5.


# Introduction

The data was first converted to the Prague dependency style as a part of HamleDT;
then it was automatically converted to Universal Dependencies (HamleDT 3.0, 2015). The first
release of Universal Dependencies that includes this treebank is UD v1.2 in November 2015. It is
essentially the HamleDT conversion but the data is not identical to HamleDT 3.0 because the
conversion procedure has been further improved.

## References:

* http://zil.ipipan.waw.pl/Sk%C5%82adnica ... Składnica zależnościowa
* http://ufal.mff.cuni.cz/hamledt ... HamleDT
* http://ufal.mff.cuni.cz/treex ... Treex is the software used for conversion
* http://ufal.mff.cuni.cz/interset ... Interset was used to convert POS tags and features

@inproceedings{pl,
  author    = {Wr{\'o}blewska, Alina and Przepi{\'o}rkowski, Adam},
  title     = {Projection-based Annotation of a {Polish} Dependency Treebank},
  booktitle = {Proceedings of the Ninth International Conference on Language Resources and Evaluation, LREC},
  pages     = {2306--2312},
  address   = {Reykjavík, Iceland},
  year      = {2014}
}


# Changelog

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


=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v1.2
License: GNU GPL 3.0
Includes text: yes
Genre: fiction nonfiction news
Lemmas: converted from manual
UPOS: converted from manual
XPOS: manual native
Features: converted from manual
Relations: converted from manual
Contributors: Zeman, Daniel; Mašek, Jan; Rosa, Rudolf
Contributing: elsewhere
Contact: zeman@ufal.mff.cuni.cz
===============================================================================
