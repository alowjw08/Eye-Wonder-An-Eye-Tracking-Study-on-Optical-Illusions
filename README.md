# 👁️ Eye Wonder: Eye-Tracking Analysis on Optical Illusions

This repository contains the full data analysis pipeline for a cognitive science research project investigating **gender differences in fixation behavior** and **pupil dilation as an indicator of cognitive load** using Tobii eye-tracking data.

## 📊 Project Overview

Using gaze data from **85 participants** collected via the **Tobii Pro Fusion** (120Hz) and **Tobii Lab** software, we analyzed:

- 🧠 **RQ1**: Are there gender-based differences in fixation durations and visual scanning patterns?
- 👁️ **RQ2**: Does pupil diameter significantly differ between high and low cognitive load illusions?

Our pipeline includes:
- Participant ID normalization
- Merging fixation events with gender metadata
- Event filtering (60–1200ms)
- Statistical analysis (Welch’s t-test, Mann–Whitney U)
- Power analysis using Cohen's d and `statsmodels`
- Visualizations with Seaborn and Matplotlib

## 🧪 Key Results

- **Fixation Duration**: Significant gender difference (t = 3.17, p = 0.0022), with males showing longer average fixations.
- **Pupil Diameter**: Significantly larger under mental-power illusion stimuli (p < 0.001), indicating increased cognitive load.
- **Power Analysis**: Sample size per group (34–55) confirmed sufficient statistical power for observed effects.

## ⚙️ Technologies Used
- Python (pandas, scipy, statsmodels, seaborn, matplotlib)
- Google Colab
- Tobii Pro Lab + Pro Fusion (Eye-tracking hardware and software)
- Jupyter Notebook

## 📌 Notes

- Raw data collected via Tobii Lab and exported in TSV format.
- Fixation events were defined using the Tobii I-VT algorithm.
- Analysis strictly followed pre-registered hypotheses and included filtering for valid gaze/pupil records only.

## 📢 Citation

If you use or reference this work, please cite:
> "Eye Wonder: An Eye-Tracking Study on Optical Illusions" – University of Malaya Cognitive Science T2G3, Semester 2, 2024/2025.

---

Feel free to adapt this if you're including code, datasets, or exporting this for academic credit.
