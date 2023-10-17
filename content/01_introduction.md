# Introduction

This is just some basic markdown formatting, nothing special.

Just mention papers with their citation key, like so [@Schnepf_2022]. Use square brackets whenever you want the reference in parentheses [e.g., even when you want to add something else in the parentheses, @Schnepf_2022]. Without the parentheses, formatting also works, as can be seen in @Schnepf_2022. **Note:** This is based on the ```style/apa-style.csl``` citation style file, you can find matching files for your usage on the web.

There is some more stuff mentioned in section \ref{sub-heading}.

Change the title page by editing ```style/before-body.tex```.

## Sub-headings work, too {#sub-heading}

For images, I recommend falling back to Tex. This might look as follows (Fig. \ref{figure-label}). Using ```width=\textwidth```, you get an image using the full textwidth of the page. Adapt this by adding a scale, for example to fit two images next to each other: ```width=.5\textwidth```. Photo by [Robert Pügner](https://www.pexels.com/de-de/foto/insekt-grunes-gras-bestauber-gehockt-13127343/).

\begin{figure}[h!]
  \centering
  \includegraphics[width=.7\textwidth]{content/images/example.jpg}
  \slcaption{Example image. Everything before the first period will be automatically used as the labelk for this image in the list of figures.}
  \label{figure-label}
\end{figure}

Of course, any Latex stuff works, so you can add mathematical formulas as well (e.g., $\alpha=.05$)^[Footnotes are placed in the text like this.].