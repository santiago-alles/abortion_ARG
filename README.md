Two Abortion Rights Bills in Argentina, 2018-2020</br >
Roll Call Votes
===============================================

Last update:
------------------
12-30-2020

</br >The Argentine Congress voted two different bills on Abortion Rights over the last couple of years.

The first bill in 2018 was narrowly passed by the House on a 129-125 vote, but it later on failed to pass in the Senate by 31-38. The second bill, now with the open support of the Executive, was passed by both chambers of Congress, thanks to a 131-117 vote in the House, and a 38-29 vote in the Senate.

This repository provides the roll call votes of both bills.

The sources of this data are:

<blockquote>
House: Honorable Cámara de Diputados de la Nación, https://votaciones.hcdn.gob.ar/</br >
Senate: Honorable Senado de la Nación, https://www.senado.gov.ar/votaciones/
</blockquote>

Data Availability
------------------

Data can be directly called from the repository using Hadley Wickham's <a href="https://cran.r-project.org/web/packages/readr/readr.pdf" target="_blank">readr</a> package:

<pre><code>require(readr)
url <- 'https://raw.githubusercontent.com/santiago-alles/abortion_ARG/master/'
file <- 'abortion_rollcall.csv'
read_csv(paste(url, file, sep='/')) -> dat
</code></pre>

Special characters may appear in string variables (e.g., name and last name, party labels, etcetera). Character strings might be converted to <code>UTF-8</code> encoding using <code>iconv</code>:

<pre><code>iconv(x, from = 'latin1', to = 'UTF-8')</code></pre>

Suggested Citation
------------------

I guess that you can cite the original Congress sources. (I barely cleaned the data before uploading it.)
