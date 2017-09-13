NCTU Thesis Template for LaTeX
==============================

**nctu-thesis-latex** is a LaTeX template forked from [chiehmin/nctu-thesis](https://github.com/chiehmin/nctu-thesis). Some improvements are added and the format is fune-tuned to meet the requirements of the thesis submitted to National Chiao Tung University.

# Sample

- Version for paper submission: [sample_paper.pdf](sample_paper.pdf)
- Version for electronic submission: [sample_electronic.pdf](sample_electronic.pdf)

![](sample.png)

# Configuration

1. Fill in the thesis title and your name in `thesis.tex`.

```
\newcommand{\chineseTitle}{基於卷積神經網路的論文自動生成技術}
\newcommand{\englishTitle}{A CNN-based Automatic Thesis Generation Technique}

\newcommand{\studentChName}{王大明}
\newcommand{\studentEnName}{Ta-Ming Wang}
\newcommand{\advisorChName}{吳小松}
\newcommand{\advisorEnName}{Xiao-Sung Wu}
```

2. Fill in the time of your submission in `covers/front.tex` and `covers/inside.tex`.

3. In `thesis.tex`, there is a flag called `paper` which can help you switch the format between paper submission and electronic submission.

```
\settoggle{paper}{false} % set to true for paper submission
```

- Paper submission
    - Margin: 2.5cm-2.5cm-2.5cm-2.5cm
    - Without watermark
    - With required documents
- Electronic submission
    - Margin: 2.5cm-2.5cm-3cm-2cm
    - With watermark

4. After oral defense, upload the required forms and documents and update the path in `thesis.tex`.

```
\includepdf{pdf/certification.pdf}
\includepdf{pdf/authorization.pdf}
```

# Environment

I have only tested this template on [Overleaf](https://www.overleaf.com) with XeLaTeX engine. Local LaTeX environment may also work.
