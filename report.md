---
event: 'OHBM Brainhack 2020'

title:  'This is an example report'

author:
- initials: AK
  surname: Karakuzu
  firstname: Agah
  email: agahkarakuzu@gmail.com
  affiliation: aff1, aff2
  corref: aff1
  url: https://agahkarakuzu.github.io
  # Please make sure that you set corref (corresponding aff) if you have
  # multiple afiliations

affiliations:
- id: aff1
  orgname: 'NeuroPoly, Polytechnique Montreal'
  street: some street 
  postcode: H3T 1Z9
  city: Montreal
  state: Quebec
  country: Canada
- id: aff2
  orgname: 'MRI Core Lab, Montreal Heart Institute'
  street: another street 
  postcode: H5T Y2D
  city: Montreal
  state: Quebec
  country: Canada

summary: This is a dummy report created during the sprint :) 

url: http://github.com/repo_owner/repo_name

coi: Please add if there are competing interests. Otherwise, type None.

acknow: The authors would like to thank the organizers and attendees of OHBM Brainhack 2020.

contrib: AK did something.

tags:
  - MRI
  - Publishing
  - Report

supplemental:
  - Material 1
  - Material 2 

bibliography: report
---

# Introduction
The bibliography (\code{report.bib}) must respect \href{http://www.bibtex.org/Using/}{BibTeX} format. 
You can cite entries in your bibliography using their tags:

\begin{itemize}
  \item Cite an article: \cite{author:2010}
  \item Cite a GitHub repository: \cite{githubrepo:2020}
\end{itemize}

\smallskip
\noindent You can use \code{inline code highlight}. This paragraph shows how to add blank lines and how to start a paragraph without indentation.

# Section
You can create additional sections as you prefer. Section title levels are determined by the number of hastags as in a traditional markdown file.

## Subsection
Subsection content goes here. You can create numerated lists:

\begin{enumerate}
  \item The labels consists of sequential numbers.
  \item The numbers starts at 1 with every call to the enumerate environment.
\end{enumerate}

### SubSubsection
You can add mathematical formulas. Single dollars ($) are required for inline mathematics e.g. $f(x) = e^{\pi/x}$.
\smallskip

\noindent You can also use plain \LaTeX for equations:

\begin{equation}\label{eq:fourier}
\hat f(\omega) = \int_{-\infty}^{\infty} f(x) e^{i\omega x} dx
\end{equation}
and refer to \autoref{eq:fourier} from text.


# Results
Figure files must be placed at the \code{figures} folder. You can include figures using the following block:

\begin{figure}[h!]

  \includegraphics[width=.47\textwidth]{brainhack.png}

  \caption{\label{fig1} Your caption goes here.}

\end{figure}

To refer a figure in the text, you need to use the respective label defined in its caption: Fig. \ref{fig1}
