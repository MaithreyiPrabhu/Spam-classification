# Spam-classification

## Algorithm used

```
1. Data with or without text Pre Processing

2. Calculate probability of a word being a spam and not spam using the training data given (Calculated log probabilities)

3. Given test data, calculate, P(S=spam|w1,...wn) and P(S= notspam|w1,...wn) using the probabilities calculated using step 2

4. If P(S=spam|w1,...wn) > P(S=notspam|w1,...wn) then assign the class as "Spam" else "Notspam". If the probabilities are equal then assign a random class

```

## Sample Outputs

Without Text Cleaning

```
./spam.py 'data/train' 'data/test' output.txt

Accuracy : 98.6%

```

With Text Cleaning

```
./spam.py 'data/train' 'data/test' output.txt

Accuracy : 95.9%

```
Accuracy was better when we tried running without pre processing of text. Also tried removing sparse words with very low count, but accuracy was better when we included all the words.
