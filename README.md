someUsefulLatex
===============

various useful non package latex hacks


infinity  \infty


\makeatletter

\def\fullpath{\begingroup\everyeof{\noexpand}\@sanitize

  \edef\x{\@@input|"find `pwd` -name \jobname.tex" }%
  
  \edef\x{\endgroup\noexpand\zap@space\x\noexpand\@empty}\x}
  
\makeatother

