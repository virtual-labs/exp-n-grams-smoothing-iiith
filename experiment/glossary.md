### Core N-gram and Smoothing Terms

**N-gram**:  
A contiguous sequence of N items (typically words) from a given text or speech sample.

**Bigram**:  
An N-gram where N=2; a sequence of two words.

**Trigram**:  
An N-gram where N=3; a sequence of three words.

**Unigram**:  
An N-gram where N=1; a single word.

**Smoothing**:  
A technique used in language modeling to adjust probability estimates for unseen N-grams, preventing zero probabilities.

**Add-One (Laplace) Smoothing**:  
A simple smoothing method that adds one to each N-gram count before calculating probabilities.

**Zero Probability Problem**:  
The issue that arises when an N-gram does not appear in the training data, resulting in a probability of zero.

**Vocabulary Size (V)**:  
The total number of unique words in the corpus.

**Maximum Likelihood Estimate (MLE)**:  
A method of estimating probabilities based on observed frequencies in the training data, without smoothing.

**Sparse Data**:  
A situation where many possible N-grams are not observed in the training corpus.

### Analysis Terms

**Language Model**:  
A statistical model that assigns probabilities to sequences of words.

**Probability Distribution**:  
A function that describes the likelihood of occurrence of different possible outcomes.

**Corpus**:  
A large and structured set of texts used for statistical analysis and hypothesis testing.

**Token**:  
An individual instance of a sequence in text, such as a word or punctuation mark.

**Type**:  
A unique word in the corpus, regardless of how many times it appears.

**Context**:  
The surrounding words or items that influence the probability of a given word in an N-gram model.

**Backoff**:  
A smoothing technique where lower-order N-gram probabilities are used when higher-order N-gram counts are zero.

**Interpolation**:  
A smoothing technique that combines probabilities from different N-gram models.

**Perplexity**:  
A measurement of how well a probability model predicts a sample; lower perplexity indicates a better model.

**Training Data**:  
The set of text used to build and estimate the parameters of a language model.

**Test Data**:  
The set of text used to evaluate the performance of a language model.

### Practical Terms

**Sentence Probability**:  
The probability assigned to a sequence of words by a language model.

**Out-of-Vocabulary (OOV) Word**:  
A word that does not appear in the training corpus.

**Frequency Count**:  
The number of times a particular N-gram appears in the corpus.

**Conditional Probability**:  
The probability of a word given its preceding context in an N-gram model.

**Normalization**:  
Adjusting probability values so that they sum to one.

---
