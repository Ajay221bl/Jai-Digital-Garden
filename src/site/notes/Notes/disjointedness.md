---
{"dg-publish":true,"permalink":"/notes/disjointedness/","tags":["probability"]}
---


# disjointedness
disjointedness refers to the situation where two sets are disjoint of each other meaning they ___don't share anything common___

to check whether two sets are disjoint use the `.isdisjoint()` method. it will give the [[Notes/Boolean operators\| boolean]] value False if they  have anything in common.
```python
a = {'a', 'b', 1, 2, 3}
b = { 1, 2, 3 }

a.isdisjoint(b)
```
