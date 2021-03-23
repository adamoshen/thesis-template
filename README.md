# A (Xe)LaTeX Thesis Template

A (Xe)LaTeX thesis template to be compiled to either PDF or PDF/A. Tested with `Texmaker` for Windows.

## Regular PDF

Compile order: `XeLaTeX` &rightarrow; `BibTeX` &rightarrow; `XeLaTeX` &rightarrow; `XeLaTeX` &rightarrow; `View PDF`

## PDF/A

As per the [`pdfx` documentation](https://ctan.org/pkg/pdfx), `-shell-escape` needs to be added as an option for XeLaTeX. 

1.  In `Texmaker`, go to `User` &rightarrow; `User Commands` &rightarrow; `Edit User Commands`.

2.  Create a new command like below

![](./readme_img/newcommand.png)

by borrowing the default options from `XeLaTeX` (can be auto-populated by using the `wizard`) and appending `-shell-escape` to the
end.

New compile order: `XeLaTeX (PDFA)` &rightarrow; `BibTeX` &rightarrow; `XeLaTeX (PDFA)` &rightarrow; `XeLaTeX (PDFA)` &rightarrow;
`View PDF`.
