# 010 - EU Country Quiz

Write a small quiz program that checks whether we know all of the countries in the European Union. Ask questions both directions:

  * What is the name of country number N?
  * Which country is numbered N?

for various (Country,N) combinations.

Add basic error handling so that the quiz is not sensitive to capitalization. 

Although we recommend retyping code rather than copying it, in this case you can skip 
(re)typing the related data and start by copying the followind dictionary. (You may need
to do some maniuplation of this to support the exercise.)

```python
eu_quiz = {'Austria': 1, 'Belgium': 2, 'Bulgaria': 3, 'Croatia': 4, 
           'Czechia': 5, 'Denmark': 6, 'Estonia': 7, 'Finland': 8,
           'France': 9, 'Germany': 10, 'Greece': 11, 'Hungary': 12,
           'Ireland': 13, 'Italy': 14, 'Latvia': 15, 'Lithuania': 16,
           'Luxembourg': 17, 'Malta': 18, 'Netherlands': 19, 'Poland': 20,
           'Portugal': 21, 'Romania': 22, 'Slovakia': 23, 'Slovenia': 24,
           'Spain': 25, 'Sweden': 26}
```

![EU Country Map](../assets/eu-europe-with-numeric-labels.png)