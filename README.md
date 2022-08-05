# globus-labs

Material for the Globus Labs web site.
https://globus.github.io/globus-labs

## Adding New Publications

Procedure for adding new publication

1. Add the publication as a PDF to `./pubs`
	- No file name format required. Recommended: `<first author surname>-<journal/conference abbreviation>-<year>.pdf`

2. Add bibtex info for the publication at the top of `./pubs/labs-pubs.bib`:
	- For all publications: Add publication name, author names, year, and "note" attribute pointing to the pdf (just `<filename>.pdf`, not the entire path)
	- For journal publications: Add journal name, volume, issue number, and page numbers. DOI and other available identifying information is recommended, but not required
	- For conference and workshop publications: Add conference or workshop name (in the format of `Proceedings of <conference-name-here>`)
	- Note: Only add publication to the top of the bibtex document if it is a new publication. If it is not new, check the dates of the other publications and add yours in its correct chronological place in the document.
	
3. Add both files into the git repo and verify appearance on the [Globus Labs website](https://labs.globus.org/publications.html) within 5 minutes or so.

***

## Running Locally for Testing

### Linux
...

### macOS
Steps are very similar to Linux (see above). First, make sure that `jekyll` is properly installed on your system. This will require installing Ruby and some other packages (information on how to do this can be found [here](https://jekyllrb.com/docs/installation/macos/)).

Once `jekyll` is installed, run the following command in the root directory of the `globus-labs.github.io` project:
```sh
jekyll serve --config _config.yml
```

### Windows
...