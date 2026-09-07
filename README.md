# APA 7th Edition Dissertation Template in LaTeX

A comprehensive LaTeX template for dissertations formatted according to APA 7th Edition guidelines.

## Features

- ✅ APA 7th Edition formatting
- ✅ Double spacing throughout
- ✅ Proper margins (1 inch on all sides)
- ✅ Times New Roman font (12pt)
- ✅ Automatic page numbering and headers
- ✅ Table of Contents, List of Tables, List of Figures
- ✅ Front matter pages (title page, approval, abstract, acknowledgments)
- ✅ Chapter structure (5 sample chapters)
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
│   └── abstract.tex                # Abstract
├── chapters/
│   ├── chapter1.tex                # Introduction
│   ├── chapter2.tex                # Literature Review
│   ├── chapter3.tex                # Methodology
│   ├── chapter4.tex                # Results
│   └── chapter5.tex                # Discussion & Conclusion
├── references/
│   └── references.bib              # Bibliography in BibTeX format
├── appendices/                      # Optional appendices
└── README.md                        # This file
```

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

## Tips

- **Keep chapters modular**: Edit chapters separately for better organization
- **Use labels**: Label figures, tables, and sections for easy cross-referencing
- **Backup your work**: Use version control (Git) to track changes
- **Compile frequently**: Check for errors as you write
- **Line numbering**: Uncomment the `lineno` package in `main.tex` if your institution requires line numbers

## Troubleshooting

**Issue**: Bibliography not appearing
- **Solution**: Run `bibtex main` and then recompile with `pdflatex` twice more

**Issue**: Figures/tables not showing
- **Solution**: Check file paths and ensure files exist in the specified locations

**Issue**: Formatting doesn't match APA style
- **Solution**: Verify that all packages are loaded and commands are correctly used

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