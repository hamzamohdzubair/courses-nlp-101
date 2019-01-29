---
title: NLTK
description: ""
---

## Splitting Sentence - 1

```yaml
type: NormalExercise
key: 108cd7d469
xp: 100
```

Let's start with dividing a document into sentences. Normally the first thing we do when we want to analyse a document is to break it down into sentences.

`@instructions`


`@hint`
text.split('something goes in here')

`@pre_exercise_code`
```{python}
import nltk
nltk.download('punkt')
```

`@sample_code`
```{python}
text = "Hello everyone. Hope you enjoy learning NLP. All the best."
# Try to extract the three sentences.
# Try the split method
sentences = # YOUR CODE HERE
```

`@solution`
```{python}
sentences = text.split('.')
```

`@sct`
```{python}

```

---

## Sentences - 3

```yaml
type: NormalExercise
key: 8c951e37ce
xp: 100
```



`@instructions`


`@hint`


`@pre_exercise_code`
```{python}
import nltk
nltk.download('punkt')
```

`@sample_code`
```{python}
text =  "Have you heard of Prof. Noam Chomsky? Father of Modern Linguistics, and author of over 100 books in linguistics, philosophy, war, etc. as well as a key figure in Psychology."
from nltk.tokenize import sent_tokenize
sentences = sent_tokenize(text)
```

`@solution`
```{python}

```

`@sct`
```{python}

```

---

## Splitting Sentences - 2

```yaml
type: NormalExercise
key: 4877d6777c
xp: 100
```

Let's try the same technique again on a different text. And you will see the challenge

`@instructions`


`@hint`


`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
text =  "Have you heard of Prof. Noam Chomsky? Father of Modern Linguistics, and author of over 100 books in linguistics, philosophy, war, etc. as well as a key figure in Psychology."
# Be careful this time. There are only two sentences.
sentences = # YOUR CODE HERE
```

`@solution`
```{python}

```

`@sct`
```{python}

```

---

## Splitting Sentence

```yaml
type: TabExercise
key: cade31ed0d
xp: 100
```

Let's start with dividing a document into sentences. Normally the first thing we do when we want to analyse a document is to break it down into sentences.

`@pre_exercise_code`
```{python}
import nltk
nltk.download('punkt')
```

***

```yaml
type: NormalExercise
key: caece64b2f
xp: 50
```

`@instructions`
Let's start with the simplest method from python. Every string in python has a split method.

`@hint`
text.split('something goes in here')

`@sample_code`
```{python}
text = "Hello everyone. Hope you enjoy learning NLP. All the best."

# HINT: Try the split method like this => text.split()

sentences = # YOUR CODE HERE

print(sentences)

# Your output should contain a list of three sentences. ignore the empty space
```

`@solution`
```{python}
text = "Hello everyone. Hope you enjoy learning NLP. All the best."
sentences = text.split('.')
```

`@sct`
```{python}
Ex().check_object('sentences').has_equal_value()
```

***

```yaml
type: NormalExercise
key: 5a1e276faa
xp: 50
```

`@instructions`
Try using the split method this time. You will realize that it's really difficult using the split method, because of the **prof.**, **etc.** **?**.

For this we will introduce the sentence tokenizer in nltk.

`@hint`


`@sample_code`
```{python}
text =  "Have you heard of Prof. Noam Chomsky? Father of Modern Linguistics, and author of over 100 books in linguistics, philosophy, war, etc., as well as a key figure in Psychology."

sentences = # YOUR CODE HERE
print(sentences)
# Your output should contain only the two sentences.

from nltk.tokenize import sent_tokenize
sentences = sent_tokenize(text)
```

`@solution`
```{python}
text =  "Have you heard of Prof. Noam Chomsky? Father of Modern Linguistics, and author of over 100 books in linguistics, philosophy, war, etc., as well as a key figure in Psychology."
from nltk.tokenize import sent_tokenize
sentences = sent_tokenize(text)
```

`@sct`
```{python}

```
