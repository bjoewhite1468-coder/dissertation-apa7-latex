# APA 7th Edition Dissertation Template in LaTeX

A comprehensive LaTeX template for dissertations formatted according to APA 7th Edition guidelines.

## Features

- ✅ APA 7th Edition formatting
- ✅ Double spacing throughout
- ✅ Proper margins (1 inch on all sides)
- ✅ Times New Roman font (12pt)
- ✅ Automatic page numbering and headers
- ✅ Table of Contents, List of Tables, List of Figures
- ✅ Complete front matter (title page, approval, abstract, acknowledgments, prefatory materials)
- ✅ Six-chapter structure
- ✅ APA-formatted bibliography
- ✅ Support for citations, tables, figures, and equations

## Structure

```
.
├── main.tex                          # Main document file
├── frontmatter/
│   ├── titlepage.tex               # Title page
│   ├── approval.tex                # Approval/signature page
│   ├── copyright.tex               # Copyright page (optional)
│   ├── dedication.tex              # Dedication (optional)
│   ├── acknowledgments.tex         # Acknowledgments
│   ├── pretext.tex                 # Pre-text (optional)
│   ├── prefatory_note.tex          # Prefatory Note (optional)
│   ├── preface.tex                 # Preface (optional)
│   ├── prologue.tex                # Prologue (optional)
│   └── abstract.tex                # Abstract
├── chapters/
│   ├── chapter1.tex                # Introduction
│   ├── chapter2.tex                # Literature Review
│   ├── chapter3.tex                # Methodology
│   ├── chapter4.tex                # Results
│   ├── chapter5.tex                # Discussion and Conclusion
│   └── chapter6.tex                # Conclusions and Recommendations
├── references/
│   └── references.bib              # Bibliography in BibTeX format
├── appendices/                      # Optional appendices
└── README.md                        # This file
```

## Front Matter Organization

Your dissertation includes comprehensive prefatory materials:

1. **Title Page** - Standard dissertation title page with author, institution, and date
2. **Copyright Page** - Optional copyright statement
3. **Approval Page** - Signature page for dissertation committee
4. **Dedication** - Optional personal dedication
5. **Acknowledgments** - Thank those who supported your research
6. **Pre-text** - Optional introductory material and context
7. **Prefatory Note** - Optional disclaimers, permissions, or important notes
8. **Preface** - Optional personal introduction to your work
9. **Prologue** - Optional thematic or narrative introduction
10. **Abstract** - Required summary of your dissertation
11. **Table of Contents**, **List of Tables**, **List of Figures** - Auto-generated

## Six-Chapter Structure

1. **Chapter 1: Introduction** - Background, problem statement, research questions, significance, and organization
2. **Chapter 2: Literature Review** - Theoretical frameworks, previous research, gaps, and conceptual model
3. **Chapter 3: Methodology** - Research design, setting, participants, data collection, analysis, and ethical considerations
4. **Chapter 4: Results** - Overview, findings by research question, quantitative/qualitative results, and summary
5. **Chapter 5: Discussion and Conclusion** - Interpretation of findings, theoretical/practical implications, limitations, recommendations, and conclusions
6. **Chapter 6: Conclusions and Recommendations** - Summary of findings, contributions, limitations, recommendations for practice/policy/future research, and final reflections

## Getting Started

### Prerequisites

- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- PDF reader
- Text editor or LaTeX IDE (e.g., Overleaf, TeXstudio, VS Code with LaTeX Workshop)

### Compilation

1. **Using Overleaf** (Recommended for beginners):
   - Upload files to Overleaf
   - Click "Recompile" to generate PDF

2. **Using command line**:
   ```bash
   pdflatex main.tex
   bibtex main
   pdflatex main.tex
   pdflatex main.tex
   ```

3. **Using LaTeX IDE**:
   - Open `main.tex`
   - Click compile/build button

## Customization

### Edit Title Page Information

Edit these commands in `main.tex`:

```latex
\newcommand{\dissertationtitle}{Your Dissertation Title}
\newcommand{\authorname}{Your Name}
\newcommand{\degreeawarded}{Doctor of Philosophy}
\newcommand{\universityname}{Your University Name}
\newcommand{\dissertationyear}{2026}
\newcommand{\departmentname}{Your Department Name}
\newcommand{\chairname}{Dr. Chair Name}
\newcommand{\committeemembertwo}{Dr. Committee Member 2}
\newcommand{\committeememberthree}{Dr. Committee Member 3}
```

### Adding Chapters

1. Create a new `.tex` file in the `chapters/` directory
2. Add `\include{chapters/chapterX}` in `main.tex`

### Optional Prefatory Materials

To use the optional prefatory sections, simply uncomment or modify the corresponding files:
- `frontmatter/pretext.tex` - Pre-text
- `frontmatter/prefatory_note.tex` - Prefatory Note
- `frontmatter/preface.tex` - Preface
- `frontmatter/prologue.tex` - Prologue

To exclude them, comment out or remove the `\include` lines in `main.tex`.

### Adding References

1. Add your citations to `references/references.bib` in BibTeX format
2. Use `\cite{key}` in your document to cite references

### Including Figures and Tables

**Figures:**
```latex
\begin{figure}[H]
  \centering
  \includegraphics[width=0.8\textwidth]{path/to/figure}
  \caption{Figure caption here}
  \label{fig:label}
\end{figure}
```

**Tables:**
```latex
\begin{table}[H]
  \centering
  \caption{Table caption here}
  \label{tab:label}
  \begin{tabular}{lcc}
    % Table content
  \end{tabular}
\end{table}
```

## APA 7th Edition Requirements Met

- ✅ Double spacing
- ✅ 1-inch margins on all sides
- ✅ Times New Roman, 12-point font
- ✅ Page numbers in top-right corner
- ✅ Running head (optional, commented out)
- ✅ Proper heading hierarchy
- ✅ APA citation style
- ✅ Proper table and figure formatting
- ✅ Comprehensive front matter

## Tips

- **Keep chapters modular**: Edit chapters separately for better organization
- **Use labels**: Label figures, tables, and sections for easy cross-referencing
- **Backup your work**: Use version control (Git) to track changes
- **Compile frequently**: Check for errors as you write
- **Line numbering**: Uncomment the `lineno` package in `main.tex` if your institution requires line numbers
- **Prefatory materials**: Use only the sections your institution requires

## Troubleshooting

**Issue**: Bibliography not appearing
- **Solution**: Run `bibtex main` and then recompile with `pdflatex` twice more

**Issue**: Figures/tables not showing
- **Solution**: Check file paths and ensure files exist in the specified locations

**Issue**: Formatting doesn't match APA style
- **Solution**: Verify that all packages are loaded and commands are correctly used

**Issue**: Page numbers not appearing
- **Solution**: Ensure `\pagestyle{fancy}` is set before `\begin{document}`

## Resources

- [APA Publication Manual (7th Edition)](https://apastyle.apa.org/)
- [Overleaf Documentation](https://www.overleaf.com/learn)
- [LaTeX Documentation](https://www.latex-project.org/help/documentation/)

## License

This template is provided as-is for educational purposes. Feel free to modify and use for your dissertation.

## Support

For issues or questions, please refer to the resources above or consult with your institution's graduate writing center.

---

**Good luck with your dissertation! 🎓**
