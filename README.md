# Awesome ML paper writing style guide
A curated guide to ML paper writing style guide — structure, style, examples, checklists, and templates for NeurIPS/ICML/ICLR/ACL/AAAI (and beyond).

## Table of contents
- [Writing](#writing)
- [Reference](#reference)
- [Figures and tables](#figures-and-tables)
- [LaTeX requirements](#laTeX-requirements)

## Writing

1. **Heading capitalization**
   - **NeurIPS**: All headings should be lower case (a.k.a. sentence case, down style) — except for the first word and proper nouns — flush left, and bold. *Example:* Methodology and results [Style guide (Overleaf)](https://www.overleaf.com/latex/templates/neurips-2024/tpsbbrdqcmsh.pdf)
   - **ACL**: All headings should be in title case (a.k.a. up style, headline style), flush left, and bold. *Example:* Methodology and Results [Style guide (Overleaf)](https://www.overleaf.com/latex/templates/association-for-computational-linguistics-acl-conference/jvxskxpnznfj.pdf)
   - **CVPR**: Same as NeurIPS — headings use sentence case (down style), flush left, and bold. *Example:* Methodology and results [Style guide (Overleaf)](https://www.overleaf.com/latex/templates/cvpr-2022-author-kit/qbmjsdxryffn.pdf)
   - **ICLR**: First-level headings are written in small caps, flush left. *Example:* <span style="font-variant: small-caps;">Methodology and Results</span> [Style guide (Overleaf)](https://www.overleaf.com/latex/templates/template-for-iclr-2025-conference-submission/gqzkdyycxtvt.pdf)
   - **AAAI**: Same as ACL — headings use title case (headline style), flush left, and bold. *Example:* Methodology and Results [Style guide (Overleaf)](https://www.overleaf.com/latex/templates/aaai-press-latex-template/jymjdgdpdmxp.pdf)
  
2. **Page limit**
   - **NeurIPS**: 9 pages of main text for submission (figures/tables included in those 9); references don’t count. If accepted, you get +1 page (10 pages) for camera-ready. Appendix allowed and unlimited.
   - **CVPR**: 8 pages total for main text (including figures/tables) in the CVPR style; additional pages for references only are allowed. Appendix allowed and unlimited (Same as NeurIPS).
   - **ACL**: Long papers: up to 8 pages of content for review, plus unlimited references; final versions get +1 page (up to 9). Short papers: 4 pages for review; final gets +1 (to 5). Appendix allowed and unlimited (Same as NeurIPS).
   - **ICLR**: Submission: main text ≤ 9 pages. During discussion & camera-ready: main text limit increases to 10 pages. References do not count; over-limit is desk-rejected. Appendix allowed and unlimited (Same as NeurIPS).
   - **AAAI**: Up to 7 pages of technical content, plus additional pages solely for references (submission). Proceedings allocation remains 7 content pages (+refs). AAAI allows a technical appendix during review, but for camera-ready the supplementary is not included in AAAI’s proceedings. 

## Reference

**Where to put citations:**
   - If you name the authors … “Smith et al. (2024) …”
   - If multiple works support the sentence … “(Doe, 2021; …)”
   - If different clauses are supported by different papers … split the sentence.
   - **Tips**
     - Be **consistent** (style, ordering, and format) within the paper.
     - **Cite close to the claim**: place the citation right where the reader needs it—after the author name (textual) or after the claim (parenthetical). If a sentence mixes multiple claims/sources, split it.
    
## Figures and tables

**Caption conventions:**
   - **ACL:** captions **below** both figures and tables. *(Source: acl-org.github.io)*
   - **AAAI:** captions **below** for both figures and tables. *(Source: AAAI Press Formatting Instructions for Authors)*
   - **NeurIPS:** **figures → below**; **tables → above**. *(Source: Formatting Instructions for NeurIPS)*
   - **ICML:** same as NeurIPS — **figures below**, **tables above**. *(Source: Submission and Formatting Instructions for ICML)*
   - **ICLR:** same as NeurIPS — **figures below**, **tables above**. *(Source: Formatting Instructions for ICLR Conference Submissions)*
   - **CVPR/WACV:** same as NeurIPS — **figures below**, **tables above**. *(Source: Formatting Instructions for CVPR/WACV Conference Submissions)*
   - **Tips**
        - When in doubt, follow the **current year’s** official template/author kit for that venue. Some details can change year to year.

## LaTeX requirements
- **NeurIPS**:
	- Citations: natbib is loaded by default; you can opt-out with \usepackage[nonatbib]{neurips_2024} (the nonatbib option). 
	- Tables: strongly recommend booktabs. 
	- Math fonts: don’t use \bbold; use AMS fonts (amsfonts / amssymb). 
	- Figures: use graphicx and specify widths as a fraction of \linewidth. 

- **ACL**:
	- Base fonts: \usepackage{times}; txfonts/newtx acceptable alternatives. 
	- Figures: use graphicx. 
	- Citations: style is based on natbib (supports \citet, \citep, etc.). 
	- Hyperlinks: DOIs/URLs appear as hyperlinks (uses hyperref). 
	- BST: ships an ACL bibliography style (acl_natbib.bst). 

- **CVPR**:
	- Cross-refs: template tells you to use \cref{...} (from cleveref) for figures/tables/equations/sections. 
	- Figures: show \usepackage{graphicx} and \includegraphics[width=...]{...} usage. 
	- Notes: The author kit does not publish a ban list like AAAI; it focuses on style compliance (two-column, numbered refs, etc.). References are numeric and listed in 9-pt Times. 

- **ICLR**:
	- Citations: use natbib for in-text citations. 
	- Figures: use graphicx with width set as a multiple of \linewidth. 
	- Style/BST files: the kit provides iclr2025_conference.sty and iclr2025_conference.bst. 

- **AAAI**:
	- Required packages: aaai, times, helvet, courier in the preamble. 
	- What’s not allowed / restricted:
		- No embedded links or bookmarks → effectively no hyperref in the proceedings PDFs. 
		- titlesec is not allowed; spacing hacks and page-layout changes (e.g., \parindent, \parskip, etc.) are flagged. 
		- Do not use [T1]fontenc (they suggest CM-Super if you need Type-1 CM). 
		- Must compile with pdfLaTeX; no .ps/.eps figures (use .pdf/.png/.jpg). 
		- Single .tex source file (excluding .bib); \input not allowed. 
	- Fonts: Times/Nimbus for text (no Computer Modern for body text). 
	- BST: use aaai.bst.

## License
- Code: MIT
- Docs & images: CC BY-NC 4.0
