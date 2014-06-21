dynamic-CV
==========

Create an academic CV with automatically updating impact metrics using Impactstory. 


## How it works:

1. Everything is written in a R-SWEAVE file (cvdynamic.Rnw)
2. We use Relenium package for R to scrape information of Impactstory.org/your.username page and get newest metrics for our scientific contributions (github, figshare, DOI articles, databases etc.)
2. Rnw file uses R markup to do computation and produces a nicely weaved LaTeX file with our metrics execlty where we want them.
3. LaTeX file generates a final PDF file with your CV and computed altmetrics which can be easily shared /printed/presented to you employer.

## Why do we need it?
IMPACT of your research is now calculated poorly... and "Impact Factor" - is not fit to describe one's real impact on science community or how it influenced it. 
One answer how to change is being provided by Impacstory.org
This service provides us (academics) with up to date metrics of how often our work was read, cited, tweeted, shared and downloaded.
BUT - there is no good way to put this neewly aquired info on paper CV, to present to your potential employer or institution. 
That is why I think this will be helpful

## Please contribute
I am not good at coding (in fact I am a physician) so I will be very greatfull if You could help me with this project. I hope it will be useful to many of you. 


## Acknowledgements:
1. Impactstory.org provides you with great impact metrics for our scientific contributions (aka altmetrics)
2. knitr is an R package that really helped with this job - it facilitates Swaeve integration for R
3. CSS is another R package that helped with coding a lot by extracting elements of the site code.
4. Relenium package provides grat tools for site content scraping!
5. the CV latex style was from http://www.howtotex.com/

