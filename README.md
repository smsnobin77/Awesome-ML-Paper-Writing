# Awesome ML Paper Writing Style Guide
A curated guide to ML paper writing stylde guide — structure, style, examples, checklists, and templates for NeurIPS/ICML/ICLR/ACL/AAAI (and beyond).

## Table of Contents
- [Writing](#writing)
- [Reference](#reference)
- [Figures and Tables](#figures-and-tables)

## Writing

1. **Heading capitalization**
   - **NeurIPS**: All headings should be lower case (a.k.a. sentence case, down style) — except for the first word and proper nouns — flush left, and bold. *Example:* **Methodology and results** [Style guide (Overleaf)](https://www.overleaf.com/latex/templates/neurips-2024/tpsbbrdqcmsh.pdf)
   - **ACL**: All headings should be in title case (a.k.a. up style, headline style), flush left, and bold. *Example:* **Methodology and Results** [Style guide (Overleaf)](https://www.overleaf.com/latex/templates/association-for-computational-linguistics-acl-conference/jvxskxpnznfj.pdf)
   - **CVPR**: Same as NeurIPS — headings use sentence case (down style), flush left, and bold. *Example:* **Methodology and results** [Style guide (Overleaf)](https://www.overleaf.com/latex/templates/cvpr-2022-author-kit/qbmjsdxryffn.pdf)
   - **ICLR**: First-level headings are written in small caps, flush left. *Example:* **METHODOLOGY AND RESULTS** [Style guide (Overleaf)](https://www.overleaf.com/latex/templates/template-for-iclr-2025-conference-submission/gqzkdyycxtvt.pdf)
   - **AAAI**: Same as ACL — headings use title case (headline style), flush left, and bold. *Example:* **Methodology and Results** [Style guide (Overleaf)](https://www.overleaf.com/latex/templates/aaai-press-latex-template/jymjdgdpdmxp.pdf)

## Reference

1. **Where to put citations**
   - If you name the authors … “Smith et al. (2024) …”
   - If multiple works support the sentence … “(Doe, 2021; …)”
   - If different clauses are supported by different papers … split the sentence.
   - **Tips**
     - Be **consistent** (style, ordering, and format) within the paper.
     - **Cite close to the claim**: place the citation right where the reader needs it—after the author name (textual) or after the claim (parenthetical). If a sentence mixes multiple claims/sources, split it.
    
## Figures and Tables

1. **Caption conventions: ACL · AAAI · NeurIPS · ICML · ICLR**
   - **ACL:** captions **below** both figures and tables. *(Source: acl-org.github.io)*
   - **AAAI:** captions **below** for both figures and tables. *(Source: AAAI Press Formatting Instructions for Authors)*
   - **NeurIPS:** **figures → below**; **tables → above**. *(Source: Formatting Instructions for NeurIPS)*
   - **ICML:** same as NeurIPS — **figures below**, **tables above**. *(Source: Submission and Formatting Instructions for ICML)*
   - **ICLR:** same as NeurIPS — **figures below**, **tables above**. *(Source: Formatting Instructions for ICLR Conference Submissions)*
   - **CVPR/WACV:** same as NeurIPS — **figures below**, **tables above**. *(Source: Formatting Instructions for CVPR/WACV Conference Submissions)*
   - **Tips**
        - When in doubt, follow the **current year’s** official template/author kit for that venue. Some details can change year to year.

## License
- Code: MIT
- Docs & images: CC BY-NC 4.0
