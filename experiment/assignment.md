**Q1**. Add-one smoothing works horribly in practice because of giving too much probability mass to unseen n-grams. Prove using an example.

**Q2**. In Add-&#948; smoothing, we add a small value '&#948;' to the counts instead of one. Apply Add-&#948; smoothing to the below bigram count table where &#948;=0.02.

|   |(eos)|John|Read|Fountainhead|Mary|a|Different|Book|She|By|Dickens|
|---|---|---|---|---|---|---|---|---|---|---|---|
|(eos)|0   |300 |0   |0   |300	|0   |0   |0   |300   |0   |0   |
|John |0   |0   |300 |0   |0   |0   |0   |0   |0   |0   |0   |
|Read |0   |0   |0   |300 |0   |600 |0   |0   |0   |0   |0   |
|Fountainhead|300 |0   |0   |0   |0   |0   |0   |0   |0   |0   |0   |
|Mary |0   |0   |300|0   |0   |0   |0   |0   |0   |0   |0   |
|a | 0  |0   |0   |0   |0   |0   |300 |300 |0   |0   |0   |
|Different|0   |0   |0   |0   |0   |0   |0   |300 |0   |0   |0   |
|Book |300 |0   |0   |0   |0   |0   |0   |0   |0   |300 |0   |
|She|0   |0   |0   |300 |0   |0   |0   |0   |0   |0   |0   |0   |
|By |0   |0   |0   |0   |0   |0   |0   |0   |0   |0   |0   |300 |
|Dickens|300 |0   |0   |0   |0   |0   |0   |0   |0   |0   |0   |

N = 5100 V = 11


Q3. Given S = Dickens read a book, find P(S)</br>
**(a)** Using unsmoothed probability</br>
**(b)** Applying Add-One smoothing.</br>
**(c)** Applying Add-&#948; smoothing</br>