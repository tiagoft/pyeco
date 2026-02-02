# Python for Economics Course

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tiagoft/pyeco/HEAD)

A course on Python and programming for PhD candidates in economics.

My contact:

Tiago F. Tavares - Office 722 - https://tiagoft.github.io


## Agenda

| Lesson | Content | 
| --- | --- |
| 0 | Python basics: variables, functions, lists, loops |
| 1 | Manipulating data with Pandas |
| 2 | Downloading data: APIs and scrappers |
| 3 | Dealing with datasets: CSVs, JSONs, SQLs | 
| 4 | Making beautiful figures with data | 
| 5 | Machine Learning basics: supervised learning and methodology |
| 6 | Modern Machine Learning: post-2022 |
| 7 | Final Test | 

##

How to use this material:

We have jupyter notebooks meant for in-class discussions. You can use them in your own machine (check the installation instructions below) or use them in an online cloud environment (click here: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tiagoft/pyeco/HEAD)).

After class, you will find a corresponding list of exercises in the `exercises/` directory in this repository. They were actually adapted to a post-AI era, and, since you are reading this, I will go head to explain the rationale.

## How to do homework exercises

After AI, it is true that any and every possible exercise I can give in class is solvable by AI. In fact, chances are that at work, in your thesis, and so on, you will probably use AI as an assistant in various levels: maybe a small correction, maybe a whole function, and maybe you will ask ChatGPT (or one of its colleagues) for code that solves a problem you have carefully described. This, however, does not change the fact that you should understand what the code is doing, especially because you want to avoid misrepresentation of your methods and results.

Until 2022, we could somewhat safely evaluate and practice coding by looking at code creation exercises. This is because, under Bloom's Taxonomy for Learning Goals, code creation is very high. Consequently, creating code (or even adapting code from examples and other sources) was a task that depended on understanding the problem, the solutions, being able to test code and to identify bugs. Nowadays, this is not true.

Although our evaluation process is highly affected by AI, the skills you will need to understand your code, your colleague's, or your AI assistant's code are the same. Hence, the exercises are explicitly distributed into Bloom's taxonomic levels.

Also, they are not *verification* exercises. Rather, they are *investigation* exercises. They are intended not to have immediate, obvious answers. You might have to research, you might have to test ideas, you might have to discuss with colleagues. Some of them might have more than one correct answer.

Just remember they are for you. They are not graded - I (instructor here!) will be happy to discuss exercises with you at any time, but if you ask me if an answer is correct, I will probably reply with: "show me why it should be correct", "let's make a counter example that shows it is not correct", or something like that. In a way, this means that the path is more important than the answer.

Good luck!

## Installing Python for Economics Course in your computer:

To install using `uv`, first ensure you have `uv` installed. Then, run the following commands:

    git clone https://github.com/tiagoft/pyeco.git
    cd pyeco
    uv sync
    source .venv/bin/activate 

To install `uv`, browse to [https://docs.astral.sh/uv/getting-started/installation/](https://docs.astral.sh/uv/getting-started/installation/) and follow the instructions for your operating system!
