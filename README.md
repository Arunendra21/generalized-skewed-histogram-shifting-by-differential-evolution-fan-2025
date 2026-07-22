# Generalized Skewed Histogram Shifting via Differential Evolution (Fan 2025)

This is a from scratch reproduction of Generalized Skewed Histogram Shifting via Differential Evolution (Guojun Fan, Lei Lu, Zijing Li, Ping Li, Quan Zhou, Zhibin Pan, IEEE TMM, vol. 27, 2025).

It predicts each pixel from its neighbours and expands the small prediction errors to carry data with very little distortion.

I reimplemented the method from the paper and ran it from start to finish. Every number and every figure in the report is produced by the code in this repo, and reversibility is checked to be bit exact wherever the method claims it.

## Running it

Everything runs with plain Python and a handful of common libraries. From this folder:

```bash
cd source_code
python3 run_experiment.py       # runs the method, writes metrics and figures
python3 build_deliverables.py   # rebuilds the IEEE report and the slides
```

You need numpy, scipy, matplotlib, pillow, python-docx and python-pptx. Install them with `pip install numpy scipy matplotlib pillow python-docx python-pptx`. The report is exported to PDF with headless LibreOffice, so that has to be on the machine if you want the PDF rebuilt.

## What sits in this folder

```
(the original paper stays on my machine and is not republished here, to respect its copyright)
ieee_report.docx/.pdf  my IEEE format reproduction report
presentation.pptx      a short summary deck
source_code/           the scripts that do the actual work
outputs/               metrics.json and the raw numbers behind the report
figures/               the plots and images the code produces
processing_notes.md    what was reproduced, what was not, and the caveats
```

## A note on honesty

I did not fabricate any measurement. Cells labelled reported come from the paper for comparison, and every other value falls out of running the code. Where the exact image set or an unstated hyperparameter differs from the paper, the absolute figures can move a little, but the behaviour and the reversibility hold. The specifics for this paper are in `processing_notes.md`.
