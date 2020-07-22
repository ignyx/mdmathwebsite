# mdmathwebsite
Generates a static website with pdfs from markdown files containing latex equations. Based on [mdwebsite](https://github.com/Paulao17/mdwebsite). Will include by default French Math Class summaries.

## Requirements
Depends on `pandoc` and `texlive`. You might need `texlive-lang-french`, `texlive-latex-extra` and `texlive-latex-extra`.
```
sudo apt-get install pandoc texlive texlive-lang-french texlive-latex-extra texlive-latex-extra
```
Note: This might be a hefty install.

To use the webhook you will need Nodejs.

## Usage
Use the shellscripts. Source markdown files in `./src` and resulting built files in `./build`.

Try `sh buildFull.sh '-M base-url:"https://example.com"'`. The First parameter is passed to pandoc, so all builds receive these parameters. Here it sets the url for OpenGraph and the "Students" link.
