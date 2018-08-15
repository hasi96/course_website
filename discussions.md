---
layout: discussions
---


## Discussion Board Etiquette

We are using GitHub Issues for discussion boards so that you can get practice posting questions in a typical data science forum. This format is similar to Stack Overflow, one of the best resources available for questions about R code and R packages.

GitHub speaks Markdown, which allows you to write questions that include reproducible code so that others can easily diagnose the problem and offer you solutions.

<br>
<img src="https://raw.githubusercontent.com/hasi96/course_website/master/assets/img/github-issues.png" 
alt="Issues" width="400" />
<br>
<img src="https://raw.githubusercontent.com/hasi96/course_website/master/assets/img/github-issues-preview.png" 
alt="Issues" width="400" />
<br>

## Simple Rules for Clear Questions

#### Don't Repeat Questions

Check the existing list of questions and topics to make sure your questions has not been asked already. Often times the answer already exists, you just need to read a couple of previous discussions.

#### Include Your Code 

There are a million ways to do something incorrectly, so we cannot guess what you are doing wrong unless you show us. Don't write questions like:

> I am trying to merge my data, but I keep getting the error message, "x is not a factor".

You need to show the code that generated the error message. 

I am trying to merge my data, but I keep getting the error message, "cannot merge object type list". Here is my code:

```r
x <- data.frame( id=letters[1:10], v1=rnorm(10) )
y <- data.frame( id=letters[1:10], v2=rbinom(10) )
z <- list( x, y )
merge( y, z )
```

#### State Your Goal

Often times people will post code without explaining what they are trying to do. Be clear about your goal so that the problem is easier to spot. 

#### Include Data

You can include data in your questions in a few ways. 

There are some functions that allow you generate random data that can be used to demonstrate the problem.

Many packages include built-in datasets that can be easily referenced with the data() function.

```r
data( Iris )
plot( Iris[,1:2] )
```

If the data is important for your example, you can post a small sample of your data using the dput() function.

```r
x <- 1:100
y <- rnorm(100)
dat <- data.frame( x, y )
dput( head( dat, 10 ) )

> structure(list(x = 1:10, 
> y = c(1.02, 1.28, 0.9, -1.35, 0.5, 0.25, 
> -0.29, 0.33, 1.61, 0.85)), 
> .Names = c("x", "y"), row.names = c(NA, 
> 10L), class = "data.frame"))
```

The output code can be pasted directly into R to re-create the original dataset.




# Stack Overflow Etiquette

When posting on a forum like St

## How do I ask a good question?

We’d love to help you. To improve your chances of getting an answer, here are some tips:

### Search, and research

...and keep track of what you find. Even if you don't find a useful answer elsewhere on the site, including links to related questions that haven't helped can help others in understanding how your question is different from the rest.

### Write a title that summarizes the specific problem

The title is the first thing potential answerers will see, and if your title isn't interesting, they won't read the rest. So make it count:

Pretend you're talking to a busy colleague and have to sum up your entire question in one sentence: what details can you include that will help someone identify and solve your problem? Include any error messages, key APIs, or unusual circumstances that make your question different from similar questions already on the site.

Spelling, grammar and punctuation are important! Remember, this is the first part of your question others will see - you want to make a good impression. If you're not comfortable writing in English, ask a friend to proof-read it for you.

If you're having trouble summarizing the problem, write the title last - sometimes writing the rest of the question first can make it easier to describe the problem.

### Examples:

* Bad: C# Math Confusion
* Good: Why does using float instead of int give me different results when all of my inputs are integers?
* Bad: [php] session doubt
* Good: How can I redirect users to different pages based on session data in PHP?
* Bad: android if else problems
* Good: Why does str == "value" evaluate to false when str is set to "value"?


### Introduce the problem before you post any code
In the body of your question, start by expanding on the summary you put in the title. Explain how you encountered the problem you're trying to solve, and any difficulties that have prevented you from solving it yourself. The first paragraph in your question is the second thing most readers will see, so make it as engaging and informative as possible.

### Help others reproduce the problem
Not all questions benefit from including code. But if your problem is with code you've written, you should include some. But don't just copy in your entire program! Not only is this likely to get you in trouble if you're posting your employer's code, it likely includes a lot of irrelevant details that readers will need to ignore when trying to reproduce the problem. Here are some guidelines:

Include just enough code to allow others to reproduce the problem. For help with this, read How to create a Minimal, Complete, and Verifiable example.

If it is possible to create a live example of the problem that you can link to (for example, on http://sqlfiddle.com/ or http://jsbin.com/) then do so - but also include the code in your question itself. Not everyone can access external sites, and the links may break over time.

### Include all relevant tags
Try to include a tag for the language, library, and specific API your question relates to. If you start typing in the tags field, the system will suggest tags that match what you've typed - be sure and read the descriptions given for them to make sure they're relevant to the question you're asking! See also: What are tags, and how should I use them?

### Proof-read before posting!
Now that you're ready to ask your question, take a deep breath and read through it from start to finish. Pretend you're seeing it for the first time: does it make sense? Try reproducing the problem yourself, in a fresh environment and make sure you can do so using only the information included in your question. Add any details you missed and read through it again. Now is a good time to make sure that your title still describes the problem!

### Post the question and respond to feedback
After you post, leave the question open in your browser for a bit, and see if anyone comments. If you missed an obvious piece of information, be ready to respond by editing your question to include it. If someone posts an answer, be ready to try it out and provide feedback!
