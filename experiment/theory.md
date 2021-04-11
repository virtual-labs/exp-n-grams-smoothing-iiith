The standard N-gram models are trained from some corpus. The finiteness of the training corpus leads to the absence of some perfectly acceptable N-grams. This results in sparse bigram matrices. This method tend to underestimate the probability of strings that do not occur in their training corpus.


There are some techniques that can be used for assigning a non-zero probabilty to these 'zero probability bigrams'. This task of reevaluating some of the zero-probability and low-probabilty N-grams, and assigning them non-zero values, is called smoothing. Some of the techniques are: Add-One Smoothing, Witten-Bell Discounting, Good-Turing Discounting.

### Add-One Smoothing

In Add-One smooting, we add one to all the bigram counts before normalizing them into probabilities. This is called add-one smoothing.

### Application on unigrams

The unsmoothed maximum likelihood estimate of the unigram probability can be computed by dividing the count of the word by the total number of word tokens N.

```
P(w<sub>x</sub>) = c(w<sub>x</sub>)/sum<sub>i</sub>{c(w<sub>i</sub>)}
      = c(w<sub>x</sub>)/N
```

Let there be an adjusted count c*.
c<sub>i</sub><sup>*</sup> = (c < sub="">+1)*N/(N+V)
where where V is the total number of word types in the language.
Now, probabilities can be calculated by normalizing counts by N.
p i* = (c < sub="">+1)/(N+V)

### Application on bigrams

Normal bigram probabilities are computed by normalizing each row of counts by the unigram count:
P(w n|wn-1) = C(wn-1wn)/C(wn-1)

For add-one smoothed bigram counts we need to augment the unigram count by the number of total word types in the vocabulary V:
p *(wn|wn-1) = ( C(wn-1wn)+1 )/( C(wn-1)+V ) 