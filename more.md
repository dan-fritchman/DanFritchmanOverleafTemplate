
# An h1 header
\label{first:section}

Paragraphs are separated by a blank line. 

2nd paragraph. *Italic*, **bold**, and `monospace`. Itemized lists
look like:

* this one
* that one
* the other one

> Block quotes are
> written like so.
>
> They can span multiple paragraphs,
> if you like.

Use 3 dashes for an em-dash. Use 2 dashes for ranges (ex., "it's all
in chapters 12--14"). Three dots ... will be converted to an ellipsis (only if you enable the `smartEllipses` option).



An h2 header
------------

Here's a numbered list (use `hashEnumerators` option if you want to use hashes):

#. first item
#. second item
#. third item

Here's a code sample:

    # Let me re-iterate ...
    for i in 1 .. 10 { do-something(i) }

As you probably guessed, indented 4 spaces. 

Or use fenced code (with `markdown` v2.4):

~~~~
# Let me re-iterate ...
for i in 1 .. 10 { do-something(i) }
~~~~

If you have `minted` loaded in your project you get syntax-highlighted code:

~~~~php
<?php
    print("Hello World");
?>
~~~~

### An h3 header ###

Now a nested list:

 1. First, get these ingredients:

      * carrots
      * celery
      * lentils

 2. Boil some water.

 3. Dump everything in the pot and follow
    this algorithm:

        find wooden spoon
        uncover pot
        stir
        cover pot
        balance wooden spoon precariously on pot handle
        wait 10 minutes
        goto first step (or shut off burner when done)

    Do not bump wooden spoon or it will fall.

Here's a link to [a website](http://foo.bar).  And now^[with `markdown` v2.4] you can also use inlined footnotes with `inlineFootnotes`.


A horizontal rule follows.

***

Here's a definition list (with `definitionLists` option):

apples
  : Good for making applesauce.
oranges
  : Citrus!
tomatoes
  : There's no "e" in tomatoe.

and images can be specified like so, and cross-referencing works if you add a \texttt{fig:} to the label: \textbf{Figure~\ref{fig:exampleimage}}

% Use \setkeys{Gin} if you need to change an image's display size

\setkeys{Gin}{width=.5\linewidth}

![exampleimage](example-image.jpg "An exemplary image")

If you enable the `hybrid` option, You can mix \LaTeX{} code in Markdown! Inline math equations go in like so: $\omega = d\phi / dt$. Displaymath too:

\begin{equation}
I = \int \rho R^{2} dV
\end{equation}

And note that you can backslash-escape any punctuation characters
which you wish to be displayed literally, ex.: \`foo\`, \*bar\*, etc.

Citations are now supported with `markdown` v2.4; but beware of underscores in BibTeX keys (best avoided)! 
When they work, they look like [@novotny:2017] or [see @novotny:2019 p.26]. 

As of `markdown` v2.8.0 you can use PHP's pipe table syntax, if you load the `pipeTables` option. You don't have to line up the pipes exactly; somehow it works out. If you also add the `tableCaptions` option, you can add a caption too! Note that there must be an empty line after the caption.


| Right | Left | Default | Center |
|------:|:-----|---------|:------:| 
|  12   |  12  |  12     |   12   | 
| 123   |  123 |   123   |  123   | 
|   1   |    1 |     1   |    1   | 

  : Demonstration of pipe table syntax.