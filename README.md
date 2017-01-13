---
maintainer: lakruzz
---
# How to get it up and running?

## Jekyll flavor

Get code and run with locally installed Jekyll to serve presentations

    git clone git@github.com:Praqma/reveals.git
    cd reveals
    git submodule init
    git submodule update
    jekyll serve

or run with Jekyll from Docker container

    git clone git@github.com:Praqma/reveals.git
    cd reveals
    git submodule update --init    
    docker run --rm --label=jekyll --volume=$(pwd):/srv/jekyll -p 4000:4000 jekyll/jekyll

Then browse your decks like this:

* http://localhost:4000/template
* http://localhost:4000/tdd


# How to get started

To get startet with a new presentation simply copy the template folder to a new project:

    cp template new-project

...and then start hacking the index.html file.


## What's in the template?

The template is the original [`demo.html`](https://github.com/hakimel/reveal.js/blob/master/demo.html) from the reveal.js project with just a very few changes added to make it work in our repository:

* Dependencies are adjusted to `/reveal.js/...`
* Template css is changed to the standard `simple.css`
* The Praqma specifics are located in `/theme/prama.simple.css` which is also added as a dependency.

That's it!

# How to change the themes?

The current theme is selected by these two lines in the html:

    <link rel="stylesheet" href="/reveal.js/css/theme/simple.css" id="theme">
    <link rel="stylesheet" href="/theme/praqma-simple.css" id="theme">

The first css is selecting the theme from reveal that is to be used as the off-set and the second contains the Praqma specific changes (logo, font-face etc.)

Say you wanted to use the `beige.css` theme the comes with reveal:

1: Copy the Praqma specific theme:

    cp /theme/praqma-simple.css /theme/praqma-beige.css

2: Make any necessary changes

3: Link you stylesheets as follows:

    <link rel="stylesheet" href="/reveal.js/css/theme/beige.css" id="theme">
    <link rel="stylesheet" href="/theme/praqma-beige.css" id="theme">

Hmmmm - that's it!
