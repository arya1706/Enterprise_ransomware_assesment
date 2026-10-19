# Enterprise Ransomware Risk Assessment Using NIST CSF 2.0

**Author:** Arya  
**Project type:** Educational cybersecurity risk assessment

## Project description

This project demonstrates a simple ransomware risk assessment for a fictional company, ABC Technologies Pvt. Ltd. The Jupyter Notebook defines eight hypothetical ransomware-related risk scenarios, validates likelihood and impact scores, calculates risk scores, assigns risk levels, visualizes the risk distribution and likelihood-impact matrix, and exports the results to CSV.

### Important data note

The dataset is **synthetic and hypothetical**. It is created in the notebook and is not sourced from a real company, public incident dataset, or real security audit. Scores are illustrative assumptions, not measured probabilities. The scoring thresholds are project-defined and are not official NIST-mandated thresholds.

## Files

- `Arya_RansomwareAssessment.ipynb` — complete notebook and implementation.
- `requirements.txt` — required Python packages.
- `Arya_ProjectReport.docx` — project report.
- `README.md` — project overview and instructions.

## Technologies used

- Python 3
- Jupyter Notebook
- pandas
- matplotlib
- NIST Cybersecurity Framework (CSF) 2.0 as a risk-management reference

## Dataset

No external dataset is required. The eight illustrative records are defined directly in the notebook so the project can run offline after dependencies are installed.

## Setup and run instructions

1. Install Python 3.10 or newer.
2. Open a terminal in the project folder.
3. (Optional but recommended) Create and activate a virtual environment.

   **Windows**
   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   ```

   **macOS/Linux**
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

4. Install dependencies:

   ```bash
   python -m pip install -r requirements.txt
   ```

5. Launch Jupyter:

   ```bash
   jupyter notebook
   ```

6. Open `Arya_RansomwareAssessment.ipynb` and choose **Kernel → Restart & Run All**.

The notebook creates `ransomware_risk_assessment_results.csv` in the current working directory.

## Risk scoring

`Risk Score = Likelihood × Impact`, where both inputs range from 1 to 5.

- 1–4: Low
- 5–9: Moderate
- 10–16: High
- 17–25: Critical

These bands are defined for this educational project.

## Limitations

This is a demonstration risk-assessment tool, not a ransomware detector, penetration test, or audit of a real company. The recommendations should be validated against an actual organization's assets, controls, risk appetite, and regulatory requirements before operational use.

## References

- NIST IR 8374 Rev. 1, Ransomware Risk Management: https://csrc.nist.gov/pubs/ir/8374/r1/final
- NIST Cybersecurity Framework: https://www.nist.gov/cyberframework
- CISA StopRansomware Guide: https://www.cisa.gov/stopransomware/ransomware-guide
