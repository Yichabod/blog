---
title: "What repositories do ML practitioners use most?"
date: 2021-09-19
draft: true
---

# What repositories do ML practitioners use most?: A review of surveys



As part of my quest to find the most important machine learning repositories, I wanted to find the repos that are used most frequently.

This post is my attempt to gauge the most popular libraries using direct surveys of people who do some type of work with machine learning. I start with the public survey data I could find before going into the private survey I did. Ultimately, I find that this approach can’t stand on its own, but that it is useful as a rapid initial look.


### Public Survey Results

It was pretty hard to find data about which machine learning repositories practitioners
use the most. A naive search turned up Buzzfeed-esque listicles with titles like
'Top 10 Machine Learning Projects on Github' from websites like analyticsvidhya.com
and analyticsindiamag.com[1]. I was hoping for a survey aggregating responses from
multiple people. The closest thing I could find was the [2020 Kaggle Developer Survey](https://www.kaggle.com/kaggle-survey-2020).

![From *Kaggle State of Machine Learning and Data Science 2020*](/kaggle_repo_use.png)

Note that the totals sum to more than 100% because the survey is multi-choice.

Kaggle is a company that charges companies to host data science competitions that solve a data science problem of theirs (Netflix famously had a $1M collaborative filtering algorithm [challenge](https://www.kaggle.com/netflix-inc/netflix-prize-data) in 2019)[3]. It is accordingly centered on ML engineers and data scientists, whom I care less about than researchers.

Scikit-learn, Keras, XGBoost, and LightGBM are are libraries that are designed for relatively standard classification and regression tasks. The popularity of these libraries on Kaggle suggest a heavy focus on model engineering and development, rather than novel research.

In looking through the rest of the survey I was surprised to learn that most Kaggle users come from India (~23%) and that the modal user had less than 2 years of experience in machine learning.


### Private Survey Results

I wanted another source of survey data, so I did a quick survey of eight ML practitioners[2]. Here is a chart of their responses.

![A survey of eight machine learning practitioners](/ML_repo_use.png)

What are these packages?

*PyTorch* and *TensorFlow* are used mainly for model specification.

*NumPy* is used for manipulating tensors and arrays easily and efficiently.

*Scikit-Learn* has many functions, but often it is used for pre-specified models that can be run with a single line.

*Matplotlib, TensorBoard,* and *Weights and Biases* are used for visualizations. *Matplotlib* mainly for training data and model outputs. *TensorBoard* and *Weights and Biases* are more for experiment logging and visualizing network weights.

*Jupyter notebook* is a simple development environment mainly used for quickly playing around with visualizations.

*Hydra* is best for specifying complex model configurations (e.g. multiple jobs with different arguments).

*Huggingface* is for easily manipulating language models.


Only responses that had more than one user were included in the bar graph. Other repositories mentioned were *pytorch_lightning, elasticsearch, s3, opencv, pyro, nltk, horovod, gym, e3nn, einops, grafana, biopython*.


### Discussion

So what did I learn?

First, the lack of consensus between the Kaggle survey and my private survey suggests that I need to keep searching. The long tail of libraries mentioned only once is also strong evidence for this.

Also, I was surprised by the lack of public data about ML repository use. To me, this suggests that a little more digging might be useful after all.

Next, I plan to analyze the Github data pulled from collections of repositories like the Linux Foundation’s AI landscape, and of course awesome-ml.

Have I missed anything? Do let me know at maxslangenkamp[at]me.com

*Credits to Tuomas Oikarinen for his comments on this post.*

---
[1] The phenomenon of clickbait-y programming blogs from India is fascinating. What
were the cultural factors that caused such a proliferation of Indian blogs?

[2] The question I used was "Can you describe the 5-10 libraries you most regularly
use for doing ML research and how they fit into your workflow?"

[3] In practice, however, it seems like companies more or less use Kaggle as a recruiting platform; the solutions crafted by participants often don't translate well to actual use cases.
