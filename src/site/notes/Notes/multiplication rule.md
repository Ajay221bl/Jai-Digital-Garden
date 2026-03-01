---
{"dg-publish":true,"permalink":"/notes/multiplication-rule/","tags":["probability","combinatorics"]}
---

# multiplication rule
> note: the multiplication rule applies when the outcomes of two events are not [[Notes/mutually exclusive sets or events\|mutually exclusive]] (meaning they can occur simultaneously).


if there are i choices to be made, with $n_{1}$ possibilities for the first choice, $n_{2}$ possibilities for the second choice, and so forth, then the aggregate number of potential outcomes equals the product of the individual choices, denoted as:
$$
n_{1}\times n_{2}\times n_{3}\dots n_{i}
$$

for example when choosing a number for a license plate with the following pattern: $ABC123$ we have a total of $17,576,000$ options to choose from. HOW?

since we have to make a total of 6 choices, for characters on the plate which are 6 in total:

| char     | possibilities |
| -------- | ------------- |
| alphabet | 26            |
| alphabet | 26            |
| alphabet | 26            |
| digit    | 10            |
| digit    | 10            |
| digit    | 10            |
hence total number of choices are :
$$
{26}\times{26}\times{26}\times{10}\times{10}\times{10} = 17,578,000
$$
