# Arte Discreta

*A predictive model of Michelin recognition*

> "Tell me what you eat, and I will tell you what you are."
> — Jean Anthelme Brillat-Savarin, *The Physiology of Taste*, 1825

For a hundred years the Michelin Guide has awarded stars without 
explaining itself. No published criteria, no named inspectors, no 
reasoning offered. This project tests the inverse: that what diners 
write — long before any inspector arrives, long before any verdict 
exists — already carries the star within it.

Working only from independent Yelp reviews, written by people who never 
knew the outcome in advance, a classifier learns to separate the 
restaurants Michelin recognized from those it passed over. The reviews 
are scored against a hand-built taxonomy of luxury — service, culinary 
precision, ambience, ingredients, experience — testing whether the model 
reasons in the vocabulary of fine hospitality, or whether ordinary 
language dominates instead.

It does not discover that luxury has a vocabulary. With only two 
Michelin-starred restaurants surviving into the working set of 8,816, 
the taxonomy's five aspects rank dead last among 305 features — a 
finding the notebook treats as data, not failure. What the project 
demonstrates instead is a pipeline built correctly under conditions that 
punish carelessness: stratified evaluation for extreme imbalance, two 
complementary metrics rather than one flattering one, and a model 
interrogated for *why* it decided, not just trusted because the score 
looked good.

This is the first of two movements. A later, deeper version — built on 
larger corpora and pretrained language representations rather than a 
hand-typed taxonomy — picks up exactly where this one's limits were 
exposed.

## Contents

The full analysis lives in `arte-discreta.ipynb`:

1. Introduction
2. Background
3. The Mathematics of Judgment
4. The Data
5. A Taxonomy of Luxury
6. Feature Engineering
7. Modelling
8. Interpretation
9. Results and Discussion
10. Conclusions
11. References

## Data

Built on the [Yelp Open Dataset](https://www.yelp.com/dataset). Raw and 
intermediate data files are tracked via DVC and are not committed to 
this repository; only the notebook, figures, and code are public.

## Requirements
```
pandas
numpy
scikit-learn
matplotlib
seaborn
rapidfuzz
scipy
```

## Author

Avgustina Daskalova · Machine Learning with Python · SoftUni · 2026
