# Yonsei University PhD Thesis LaTeX Template (2026 English form)

This project reproduces the layout rules and sample pages in the uploaded **Yonsei University Graduate School Thesis Formatting Guidelines (2026, English MS Word doctoral form)**.

## Quick start

1. Edit only `metadata.tex` for title, author, department, advisor, degree, dates, and committee names.
2. Replace the sample text in `frontmatter/` and `chapters/`.
3. Compile `main.tex` with **XeLaTeX**.
4. Compile XeLaTeX at least twice for the TOC/list page numbers. The included sample uses a manual bibliography so it compiles without BibTeX. If you switch to a `.bib` workflow, run BibTeX/Biber as required by your bibliography package.

Local command for the included sample:

```bash
xelatex main.tex
xelatex main.tex
```

In Overleaf, select **XeLaTeX** as the compiler.

## Form settings implemented

- A4 paper (210 x 297 mm)
- Times New Roman when installed; Tinos fallback only when TNR is unavailable
- Main body: 10 pt
- Main dissertation title: 18 pt bold on cover
- Section/subheading: 13 pt bold
- Footnotes: 9 pt
- 1.5 line spacing
- Left/right margins: 3.5 cm
- Top/bottom margins: 5.3 cm
- Footer/page-number baseline arranged to correspond to the 3.2 cm footer setting in the Word form
- Centered page numbers
- Preliminary matter uses lower-case Roman numerals; TOC starts at i
- Main text restarts with Arabic page 1
- Cover, title, and signature pages are fixed to one page each
- Cover/title/signature vertical blocks reproduce the fixed row heights in the Word form
- Order: cover -> title -> signature -> acknowledgements (optional) -> TOC -> lists -> English abstract -> text -> appendices -> references -> Korean abstract

## Important notes

- The original Word guide says that the red instructional text/memos must be removed and blue editable text changed to black. This LaTeX version contains only final black content and editable placeholders.
- The supplied guide permits 10 or 11 pt body text. This template defaults to 10 pt because the sample body page is marked 10 pt.
- The guide allows 1.5 or double spacing. This template defaults to 1.5 spacing.
- Bibliography/citation style is discipline-dependent in the guide. `plainnat` is included only as a working example; replace it with the style approved by your department/advisor.
- If exact front-page wording differs for your department or degree, edit `yonsei-thesis.cls` only after confirming the required official wording.
