These are notes gernated through a conversation with Gemini AI.

Update LaTeX first, the tagged pdf requires it to be as up to date as possible
- Run sudo tlmgr update --self --all

Once the LaTeX is uptodate, compile with lualatex first to generate bib files
- lualatex --shell-escape html_main.tex

Make4ht Notes:

Use the following command for the build:

- ?????

This ensures that it 
- uses luatex -l
- saves to a separate build directory -d
- uses mathjax for best web visibility
- uses html5 for most up to date content tags
- is supposed to put temp build files in a separate directory -b
- to include extra configuration file -e
- material for build is in mybuild.mk4

Or if using Pandoc:

- pandoc filename.tex -o filename.html --mathjax -s

