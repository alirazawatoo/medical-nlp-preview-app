# Medical NLP Preview App

A Streamlit demonstration that applies medspaCy processing and custom rule patterns to supplied clinical text, then previews extracted entities and contextual annotations.

## Local setup

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
streamlit run medspacy_streamlit_final.py
```

`rush_rules.tsv` contains the rule definitions consumed by the application. `medspacy.jpg` is a project illustration used by the interface.

## Intended use

The app is an NLP exploration interface for synthetic or de-identified text. It helps inspect how rule-based clinical pipelines label spans; it is not a diagnostic system and does not establish clinical accuracy.

## Boundaries

- Output quality depends on the installed model, medspaCy pipeline, and the included rules.
- Rule matches can miss relevant concepts or produce false positives.
- Do not paste protected health information into an unreviewed local or hosted deployment.
- The application and models were not run during the portfolio review.
