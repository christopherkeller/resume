While I've heavily  tweaked the format to my own tastes, it's an amalgamation of things I've found via Hacker News and random searching, so credit goes to those individuals. If you don't want to do your own fonts, you don't need xelatex as the processor.

Why this format? In short, conditional file inclusion during compilation using:

      \IfFileExists{}{%
          \input{}
      }

This lets me open source while still hiding contact information and defense related clearances.

Main files are: 

* index.tex handles the document formatting
* main.tex contains the actual content

Job specific resume? Branch!

Compile with:

      xelatex index.tex

