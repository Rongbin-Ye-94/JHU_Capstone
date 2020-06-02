Capstone Product Presentation
========================================================
author: Rongbin Ye
date: 5/28/2020
width: 1200
height: 1000
transition: fade


Summary Of Project
========================================================
Pro the request of Swiftkey and JHU data sciencist concetration, an input application is requested to be developed. Utilzing the three dataset of common English languages used in tweets, blogs and news, a predictive model need to be embedded in the app.

- Build a model of predicting next word users might use
- Build an web application of model

![plot of chunk unnamed-chunk-1](sources.png)

N-Gram with Kenser-Ney Smoothing
========================================================
Considering explainability and perplexity,a major model based on N-grams is chosen to be the model for application development (jurafsky & Martin, 2019).

The N-gram model with kenser-ney smoothing is used. The basic idea is a lazy loading model which uses a given chuck to form a probability of the given word and certain combination of word. Furthermore, with kenser-ney smoothing, the higher ngram has a higher priority to stimulate a language context. 

Reference: https://web.stanford.edu/~jurafsky/slp3/3.pdf
   
Data Product
========================================================
This data product contains three major components: main dashboard with prediction and a straightforward GUI for interaction. 

Base on this prototype product, as more data being trained through the model, the capacity of prediction will be reinforced for this model. This is a screenshot of the product developed.

![plot of chunk unnamed-chunk-2](Demo.png)


Improvement of Model
========================================================
Indeed, there are some spaces for improvement for this product. Despite N-gram model provides a great predictictability, this model has three major flaws: 

![plot of chunk unnamed-chunk-3](flaws.png)

- Lack understanding of Context
- Insensitive Sentimental understanding
- Slow Processing Speed due to file size

To tackle these flaws, the process has been optimized by data cleaning process. Yet, if a LSTM RNN could be applied, I expect a better prediction result with these consideration, but have less intepretability. 

Thank You
========================================================
