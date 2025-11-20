This documents are for tests for different RAG systems. Texts with formulas could be easily as simple text without OCR.

Also, other math documents may be picked from [here](https://huggingface.co/datasets/PleIAs/Math-PDF/).

Target document `W1605366104.pdf` was picked [here](https://huggingface.co/datasets/PleIAs/Math-PDF/blob/main/math_pdf_tars/openalex_math_pdf_tar_31.tar). Document with relative text `QKlectures(MSJ23).pdf` was found [here](https://personal.math.vt.edu/lmihalce/QKlectures(MSJ23).pdf).

Questions:

* Give information about K theory
* Write proof of the Pieri-type formula
* What does this formula mean? `v(h) < v(i) < v(l)`
* Show Forbidden subsequences in chains in the k-Bruhat order
* What is `∧i(S) · det(S∨) = ∧k−i(S∨)`

How we calculate right result:
- If document found, +1. If it also shows many wrong documents, +0;
- If document found, but text is correct - ask with "Show needed document". If document is correct, +0.5;
- Otherwise, 0.

Max score: 5