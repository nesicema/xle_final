# Grammar Development Final Project: English Relative Clauses

_Group members: Ema Nesic, Romaisaa Ahmed, Yeganeh Mohammad Salehi_

## Introduction

Given the assignment prompt of accounting for a linguistic phenomenon in XLE, our group looked to do so in English, seeing that all three members had different native languages: we reasoned English grammatical constructions would serve well as an impartial common denominator. In English, then, we chose to look at relative clauses, a cross-linguistic phenomenon that, in addition to not having been previously discussed in the course, is syntactically relatively straightforward and may be implemented within our existing grammar.


### Relative Clauses
A relative clause is a subordinate clause that modifies its preceding noun phrase (de Vries, 2018). Within this embedded clause, the relative marker (i.e., the head of the embedded phrase), is indicated by English relative pronouns (i.e., who, when, that, etc.); these elements, while informative, are optional in English relative clauses, a finding that is not consistent across languages (i.e., French, where the absence of the relative marker renders the construction ungrammatical). This is illustrated in the English sentence "The trail that I hiked is steep”, where the pronoun **where** modifies _the trail; conversely, “The trail I hiked is steep” is an equally permissible construction*, and indeed, an example of linguistic variation (Newbrook, 2003). 

Further, there exists variation in the choice of marker - although technically grammatical to use ‘who’ with animate, and ‘that’ with inanimate subjects, native English speakers confound the two - this is reflected in the grammar, where either variant results in a correct parse; thus an animacy restraint was omitted).

## Part I - Motivation

Having looked at the relevant c-structure for relative clauses, we deduced that this embedded clause must occur within the noun phrase (NP); thus, the NP had to be modified to accomodate this optional information, as an utterance may be grammatical in either reading (i.e., "the man slept" vs. "the man who ate slept").
Additionally, relative clauses are composed of a marker clause as well as a recursive sentence structure - these are denoted as C and S, respectively.


![alt text](http://i.pinimg.com/474x/3c/02/d3/3c02d3c06ba7cab08cd9c7de3e9762e3.jpg)


...

## Part II - Implementation


Our first goal therefore was to represent the most basic of relative clause examples, "the man who ate slept": here, the subject of the embedded relative clause is __the man__.

Next, we looked to capture the passive construction, exhibited in the sentence "the bone that was thrown shattered".
...

## Part III - Remaining Challenges and Future Refinement

In some instances, these embedded relative clauses may be accompanied by the relevant punctuation (i.e., "the man who ate, slept"); because the relative positions of the words are illustrated in the syntactic tree (i.e., whether a verb occurs in the matrix or embedded clause), we reasoned that punctuation may be omitted; this, however, may be implemented in a future project.

...


## Contributions

| Team Member  | Contributions                                             |
|--------------|-----------------------------------------------------------|
| Ema Nesic  | Github implementation, supplementary theory, ... |
| Romaisaa Ahmed | ... |
| Yeganeh Mohammad Salehi | ... |

## References

[1] Fong, Sandiway & Ginsburg, Jason. (2023). On the computational modeling of English relative clauses. Open Linguistics. 9. 10.1515/opli-2022-0246. 

[2]

[3]


