# Decoding Spatial Pain Anticipation from EEG

This repository contains the analysis notebooks developed for my master’s thesis:

**Decoding Spatial Pain Anticipation from EEG in a Pavlovian Threat-Learning Paradigm**

The project investigates whether cue-period EEG can decode the expected spatial content of pain, distinguishing **left-threat**, **right-threat**, and **safety** under a subject-wise evaluation framework.


## Main result

The strongest held-out result was obtained by the **alpha-only Attention TCN**:

- Test accuracy: **40.27%**
- Macro-F1: **0.3975**
- Chance level: **33.33%**

The strongest full-band model was the **Full-band Attention TCN**, with **39.93%** test accuracy and **0.3867** macro-F1.

The results are reported as held-out decoding performance.


## Thesis and links

- Full thesis PDF: [`Bahar_Hamzehei_MSc_Thesis.pdf`](./Bahar_Hamzehei_MSc_Thesis.pdf)
- LinkedIn: [linkedin.com/in/Bahar-Hamzehei](https://linkedin.com/in/Bahar-Hamzehei)
- Contact: bahar.hamzehei@studio.unibo.it


## Project overview

The thesis focuses on EEG recorded during the cue period of a Pavlovian threat-learning task.  
The analysis pipeline includes:

- signal-based estimation of DC-related recovery,
- contamination-aware dataset construction,
- export of cleaned time-domain and time–frequency representations,
- grouped subject-wise train/validation/test splitting,
- deep-learning modelling in full-band and restricted-input settings.

The main empirical results are based on the **Block 1** analysis.  
Additional exploratory and auxiliary analyses are also included for completeness.



## Repository structure

The notebooks are arranged in the approximate order of the analytical workflow:

### DC recovery and threshold estimation
1. `01_dc_tail_estimation_block1.ipynb`  
   Signal-based DC recovery analysis for Block 1.

2. `02_dc_tail_estimation_block1&block2.ipynb`  
   Combined-block DC recovery analysis used for comparison and shared threshold estimation.

### Dataset auditing and construction
3. `03_dataset_audit_block1.ipynb`  
   Block 1 dataset audit, segment statistics, and cleaning summaries.

4. `04_dataset_audit_block1&block2.ipynb`  
   Combined-block dataset audit used as a consistency check.

### Main and exploratory modelling analyses
5. `05_main_fullband_block1.ipynb`  
   Main Block 1 full-band modelling analysis.

6. `06_alpha_restricted_block1.ipynb`  
   Alpha-restricted Block 1 modelling analysis.

7. `07_theta_restricted_block1.ipynb`  
   Theta-restricted Block 1 modelling analysis.

8. `08_c3c4_restricted_block1.ipynb`  
   C3/C4-restricted Block 1 modelling analysis.

9. `09_auxiliary_block1_block2.ipynb`  
   Auxiliary Block 1+Block 2-labelled modelling analysis.



## Data availability

The raw EEG / BrainVision recordings are **not included** in this repository.

This repository is intended to document the analytical workflow and modelling code used in the thesis.  
Reproducing the full pipeline requires access to the original experimental dataset and corresponding local path configuration.



## Notes on execution

Some notebooks were originally developed within a local project directory structure.  
To run them on a different machine, local paths, data locations, and output directories may need to be adapted.

The repository therefore provides the **analysis logic and notebook structure**, but not a turnkey public reproduction package with bundled raw data.



## Scope of the analyses

The repository includes code for:

- DC-recovery analysis,
- dataset auditing and contamination-aware cleaning,
- time-domain modelling,
- time–frequency modelling,
- alpha-restricted, theta-restricted, and C3/C4-restricted analyses,
- an auxiliary Block 1+Block 2-labelled branch.

The **main thesis conclusions** are based on the **Block 1** analyses under grouped subject-wise evaluation with train-only normalization.  
The auxiliary Block 1+Block 2-labelled branch is included as supplementary material and is not the primary empirical basis of the thesis.



## Thesis context

This repository accompanies a master’s thesis submitted in the context of the:

**Second Cycle Degree in Artificial Intelligence**  
**University of Bologna**

Research was carried out in collaboration with the Department of Psychology, Center for Studies and Research in Cognitive Neuroscience.



## Author

**Bahar Hamzehei**  
Master’s Degree in Artificial Intelligence  
University of Bologna



## Additional note

Internal project materials, private experimental assets, and raw data files are not distributed in this repository.



## License

This repository is shared for academic and research documentation purposes.
