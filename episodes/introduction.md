---
title: "Building an HPC for Training"
teaching: 10
exercises: 2
---

:::::::::::::::::::::::::::::::::::::: questions 

- Why would you want to build an HPC for training?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Explain the the reasons (advantages) for building an HPC for training.


::::::::::::::::::::::::::::::::::::::::::::::::

## Introduction

When running a workshop to teach learners how to use an HPC, an instructor is
immediately presented with a few problems:

1. Very few users ever get to see an HPC in real life and it is left to 
imaginations and sci-fi movies to visualise what an HPC is. To many this is
quite a scary concept. 
1. Training on a "real" HPC can cause learners to be anxious that they might 
"break" something.
1. Access to an HPC needs to be arranged. This is not always a trivial task as
the use of HPC resources can be quite restricted in terms of who are allowed
to use a specific HPC. 
1. Workshop attendees often do not read their emails 
requesting them to create accounts before they turn up for the workshop which
results in instructors having to create accounts on the day. Apart from quite
often delaying the start of the workshop, it is also not always possible for 
instructors to create the user accounts on the day.
1. HPC resources are always in demand and running a workshop on a "real" HPC
takes resources away from "real" processes running at the time.
1. HPCs typically have to be connected to via the Internet. Any issues with 
accessing the Internet will affect the workshop.
1. If an HPC is heavily used or if someone runs a job on the login node, 
learners might not be able to log in or there are significant delays in getting
jobs into queues which again affects the timing of the workshop.

All these mentioned issues (and probably more) can be addressed by having a
dedicated HPC for training. But usually "real" HPCs are very expensive. 

:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::: instructor

Inline instructor notes can help inform instructors of timing challenges
associated with the lessons. They appear in the "Instructor View"

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: challenge 

## Challenge 1: Can you do it?

What is the output of this command?

```r
paste("This", "new", "lesson", "looks", "good")
```

:::::::::::::::::::::::: solution 

## Output
 
```output
[1] "This new lesson looks good"
```

:::::::::::::::::::::::::::::::::


## Challenge 2: how do you nest solutions within challenge blocks?

:::::::::::::::::::::::: solution 

You can add a line with at least three colons and a `solution` tag.

:::::::::::::::::::::::::::::::::
::::::::::::::::::::::::::::::::::::::::::::::::

## Figures

You can use standard markdown for static figures with the following syntax:

`![optional caption that appears below the figure](figure url){alt='alt text for
accessibility purposes'}`

![You belong in The Carpentries!](https://raw.githubusercontent.com/carpentries/logo/master/Badge_Carpentries.svg){alt='Blue Carpentries hex person logo with no text.'}

::::::::::::::::::::::::::::::::::::: callout

Callout sections can highlight information.

They are sometimes used to emphasise particularly important points
but are also used in some lessons to present "asides": 
content that is not central to the narrative of the lesson,
e.g. by providing the answer to a commonly-asked question.

::::::::::::::::::::::::::::::::::::::::::::::::


## Math

One of our episodes contains $\LaTeX$ equations when describing how to create
dynamic reports with {knitr}, so we now use mathjax to describe this:

`$\alpha = \dfrac{1}{(1 - \beta)^2}$` becomes: $\alpha = \dfrac{1}{(1 - \beta)^2}$

Cool, right?

::::::::::::::::::::::::::::::::::::: keypoints 

- Use `.md` files for episodes when you want static content
- Use `.Rmd` files for episodes when you need to generate output
- Run `sandpaper::check_lesson()` to identify any issues with your lesson
- Run `sandpaper::build_lesson()` to preview your lesson locally

::::::::::::::::::::::::::::::::::::::::::::::::

[r-markdown]: https://rmarkdown.rstudio.com/
