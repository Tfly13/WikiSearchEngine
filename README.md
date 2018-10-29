

This is a tutorial for the IR lecture of the Mastère BigData at Ensimag (Grenoble), aiming at developing a simple search engine for a subset of wikipedia pages.

Author: Clovis Galiez, 2018.

License GNU/GPL. 


# Crawl a wikipedia category

`python3 crawl.py > listPages.lst`

# Download the XML of the pages

`./dw.sh listPages.lst`

This will fetch pages from the API https://en.wikipedia.org/wiki/Special:Export to teh directory dws

# Parse the XML pages

`python3 parsexml.py dws/*`

This will create dictionnaries containing the token and link information

# Search :)

`python3 search.py "evolution bacteria"`


