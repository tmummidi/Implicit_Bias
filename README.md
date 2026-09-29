# Implicit bias research notebooks

Research notebooks for news-source bias classification and representation analysis. The repository includes a classical TF-IDF/logistic-regression baseline and experimental transformer/contrastive pipelines.

## Verified state, 2026-09-29

The classical baseline cells 0, 1 and 3-6 of Drift_Score.ipynb executed with unused embedding imports omitted. The included CSV contained 21,754 rows; the evaluated split contained 2,552 rows. The resulting rounded accuracy was 0.42. This is an execution check of that split, not a generalization claim.

Full transformer training was not executed. Other notebooks depend on Colab mounts, separately stored Missouri data and downloaded model weights. analysis_constrastive.ipynb contains a stored NameError for clf. Stored notebook output is not proof that an end-to-end run works today.

## Research repair priorities

1. Split by news story or source before fitting representations to avoid related-story leakage.
2. Package one baseline with pinned dependencies and a seed-controlled command.
3. Document dataset and model terms, provenance, class definitions and label limitations.
4. Restore the external evaluation dataset through an authorized local acquisition path.
5. Run contrastive and transformer methods only after a reproducible baseline and leakage-resistant evaluation are established.

Consolidated_pipeline.ipynb is the intended full pipeline; the other notebooks preserve experiments. Source bias labels do not establish the truth or falsity of individual statements. Existing history is retained. No new license is asserted for third-party text or model weights.
