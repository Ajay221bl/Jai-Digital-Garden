---
{"dg-publish":true,"permalink":"/notes/conditional-probability/","tags":["probability"]}
---

# conditional probability
the likelihood of something happening given that something else has already happened.
Rather than quantifying [[Notes/probability\|probabilities]] in isolation, we assess them within a context where additional information (conditions) shapes our expectations.

- The [[Notes/conditional probability\|conditional probability]] affects the size of the [[Notes/sample space\|sample space]].
- conditional probability applies only on the [[Notes/dependent events\|dependent events]]

examples of [[Notes/conditional probability\|conditional probability]]:
what is the [[Notes/probability\|Notes/probability]] of you carrying an umbrella today?
well it depends on another event which is if it ___rains___ today or not.
if it rains then there are high chances of you taking your umbrella out.
THIS IS WHAT CONDITIONAL PROBABILITY IS....................


formula:
$$ P(A|B) = \frac{P(A~and~B)}{P(B)}$$
where:
- $P(A|B)$ denotes the [[Notes/conditional probability\|conditional probability]] of event $A$ occurring with the knowledge that [[Notes/event\|event]] $B$ has already occurred.
- $P(\text{ A and B})$ is the [[Notes/probability\|Notes/probability]] of both events $A$ and $B$ occurring.
- $P(B)$ is the probability of event $B$ occurring.
#### example 
suppose you are typing on whatsapp. You have typed "How are" and the whatsapp gives these three choices to choose from: "you", "things" and "the".

How does the whatsapp able to predict this??? this is where [[Notes/conditional probability\|conditional probability]] comes into play.
$${P(\text{next word = "you" | first word="How", second word="are"})}$$
the [[Notes/algorithm\|algorithm]] goes through all the sentences that have `How` and `are` as first and second word respectively and then finds which word has the __highest probability__ to appear as third word given that first and second words are "How" and "are"


[[Notes/conditional probability two dice example\|conditional probability two dice example]]
