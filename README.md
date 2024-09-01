# Grammar Development Final Project: English Relative Clauses

_Group members: Ema Nesic, Romaisaa Ahmed, Yeganeh Mohammad Salehi_

## Introduction

Given the assignment prompt of accounting for a linguistic phenomenon in XLE, our group looked to do so in English, seeing that all three members had different native languages: we reasoned English grammatical constructions would serve well as an impartial common denominator. In English, then, we chose to look at relative clauses, a cross-linguistic phenomenon that, in addition to not having been previously discussed in the course, is syntactically relatively straightforward and may be implemented within our existing grammar.


### Relative Clauses
A relative clause is a subordinate clause that modifies its preceding noun phrase (de Vries, 2018). Within this embedded clause, the relative marker (i.e., the head of the embedded phrase), is indicated by English relative pronouns (i.e., who, when, that, etc.); these elements, while informative, are optional in English relative clauses, a finding that is not consistent across languages (i.e., French, where the absence of the relative marker renders the construction ungrammatical). This is illustrated in the English sentence "The trail that I hiked is steep”, where the pronoun **where** modifies _the trail; conversely, “The trail I hiked is steep” is an equally permissible construction[1], and indeed, an example of linguistic variation (Newbrook, 2003). 

Further, there exists variation in the choice of marker - although technically grammatical to use ‘who’ with animate, and ‘that’ with inanimate subjects, native English speakers confound the two - as a result, this is reflected in the grammar, where either variant results in a correct parse; thus an animacy restraint was omitted).

## Part I - Motivation

Having looked at the relevant c-structure for relative clauses, then, we deduced that this subordinate clause relating additional information as to its preceding clause must be embedded within the noun phrase (NP).

![alt text](http://i.pinimg.com/474x/3c/02/d3/3c02d3c06ba7cab08cd9c7de3e9762e3.jpg)

Thus, the rules governing NPs must be modified to accommodate this embedded clause, as an utterance may be grammatical in either reading (i.e., "the man slept" vs. "the man who ate slept"): here, the clause is composed of the head marker (denoted as R) as well as a simplified sentence structure, denoted as ES (i.e., embedded sentence).
There are several common relative clause pronouns in English - that, who, which, whose, whom, etc. Some of these pronouns are restricted to certain types of entities (i.e., whom for accusative case, who for animate, and which or that for inanimate entities), and so these features may be encoded as supplementary semantic information.

Finally, there exist two types of relative clauses: defining and non-defining clauses. In the first variant, the information relayed in the relative clause is necessary to deduce who is being spoken of (i.e., "John, who lives next door, is a good neighbhor). This is in contrast to the second variant, whose relative clause does not add contentful information as to the entity specified (i.e., "John, whom I met, was promoted by his employee").

## Part II - Implementation

Our first goal therefore was to represent the most basic of relative clause examples, “the otter that ate slept”: here, the subject of the embedded relative clause is ‘the otter’, while the pronoun is, accordingly, set to ‘that’, on account of its subject being inanimate (i.e., non-human)[2]. 
In our grammar file, while the matrix sentence, noun phrase and verb phrase are indicated by S, NP, and VP, respectively, the embedded relative clause sentence, noun phrase and verb phrase are instead replaced by ES, ENP, and EVP (i.e., where nouns and verbs in the lexicon have both entries); this ensures that any idiosyncracies of embedded clauses (i.e., omitted subjects) do not affect 

 Next, we looked to represent the passive construction, exhibited in the sentence “the car that I bought was stolen”, any additional grammatical categories (i.e., adjectives, adverbs, and prepositions), as well as capture the distinction between defining and non-defining relative clauses.

## Part III - Remaining Challenges and Future Refinement

In some instances, these embedded relative clauses may be accompanied by the relevant punctuation (i.e., "the man who ate, slept"); because the relative positions of the words are illustrated in the syntactic tree (i.e., whether a verb occurs in the matrix or embedded clause), we reasoned that punctuation may be omitted; this, however, may be implemented in a future project.


Depending on the whether the embedded clause was active or passive, the relative clause element was variable in its being obligatory:
“the trail [that] I hiked was steep” vs. “the trail I hiked was steep” - both grammatical
“the bone that was thrown shattered” vs. *”the bone was thrown shattered” - variable grammaticality

Thus, further improvement of the rules may include taking grammatical voice into consideration, encoding it as a feature of the relative clause marker, R.

## Contributions

| Team Member  | Contributions                                             |
|--------------|-----------------------------------------------------------|
| Ema Nesic  | Github implementation, supplementary theory, grammar implementation |
| Romaisaa Ahmed | Github implementation, grammar implementation, testsuites |
| Yeganeh Mohammad Salehi | testsuites, grammar implementation |

## References
[1] Additionally, the relative clause itself is optional - one can also merely say “The trail is steep” (grammatical, albeit encoded with less information).

[2] In our grammar file, while the matrix sentence, noun phrase and verb phrase are indicated by S, NP, and VP, respectively, the embedded relative clause sentence, noun phrase and verb phrase are instead replaced by ES, ENP, and EVP (i.e., where nouns and verbs in the lexicon have both entries); this ensures that any idiosyncracies of embedded clauses (i.e., omitted subjects) do not affect 

[3] de Vries, M. (2018). Relative Clauses in Syntax. In Oxford Research Encyclopedia of Linguistics https://doi.org/10.1093/acrefore/9780199384655.013.56

[4] Fong, S & Ginsburg, J. (2023). On the computational modeling of English relative clauses. *Open Linguistics*. 9. 10.1515/opli-2022-0246. 

[5] Newbrook, J. (2003).




