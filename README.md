# Yonsei University Graduate School Thesis LaTeX Template (2026 English forms)

Unofficial LaTeX implementation of the 2026 English MS Word thesis forms for **doctoral** and **master's** theses.

## Choose the main file

- Doctoral thesis: `main-phd.tex`
- Master's thesis: `main-master.tex`

The two degree types use separate class and metadata files so that the official degree-specific wording and committee layouts do not need to be edited manually.

```text
main-phd.tex
  ├── yonsei-phd.cls
  └── metadata-phd.tex

main-master.tex
  ├── yonsei-master.cls
  └── metadata-master.tex
```

The thesis body is shared:

```text
frontmatter/
chapters/
backmatter/
references.bib
```

## Quick start

### PhD

1. Edit `metadata-phd.tex`.
2. Set `main-phd.tex` as the main document.
3. Compile with **XeLaTeX**.

```bash
xelatex main-phd.tex
xelatex main-phd.tex
```

### Master's

1. Edit `metadata-master.tex`.
2. Set `main-master.tex` as the main document.
3. Compile with **XeLaTeX**.

```bash
xelatex main-master.tex
xelatex main-master.tex
```

In Overleaf, select **XeLaTeX** as the compiler and choose the appropriate main file.

## Degree-specific differences implemented

### Doctoral thesis

- `A Dissertation Submitted`
- Degree metadata such as `Doctor of Philosophy`
- Signature page: one committee chair + four committee members
- Certification wording: `This certifies that the dissertation ... is approved.`

### Master's thesis

- `A Master's Thesis Submitted`
- Degree metadata such as `Master of Science`
- Signature page: one committee chair + two committee members
- Certification wording: `This certifies that the master's thesis ... is approved.`

## Common form settings

- A4 paper (210 x 297 mm)
- Times New Roman when installed; Tinos fallback when unavailable
- Main body: 10 pt
- Cover title: 18 pt bold
- Main chapter title: 16 pt bold
- Section/subheading: 13 pt bold
- Footnotes: 9 pt
- 1.5 line spacing
- Left/right margins: 3.5 cm
- Top/bottom margins: 5.3 cm
- Centered bottom page numbers
- Preliminary matter uses lower-case Roman numerals
- Main text restarts with Arabic page 1
- Cover, title, and signature pages are each fixed to one page
- Order: cover -> title -> signature -> acknowledgements (optional) -> TOC -> lists -> English abstract -> text -> appendices -> references -> Korean abstract

## Notes

- The templates reproduce the supplied 2026 Yonsei University Graduate School English MS Word forms and are not an official LaTeX distribution of Yonsei University.
- The original form permits 10 or 11 pt body text; these templates use 10 pt to follow the sample manuscript pages.
- The original form permits 1.5 or double spacing; these templates use 1.5 spacing.
- Citation and bibliography style should be selected according to the department/advisor's requirements.
- Verify the final PDF against the latest official Graduate School form before submission.

## Generative AI Declaration

Generative AI (ChatGPT, OpenAI) was used in preparing this LaTeX template.
