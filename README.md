# CAVA Lab Assets

Public image assets used by CAVA Lab documentation pages (Notion).

## Detector Benchmark 2026-04-30

Folder `detector-benchmark-2026-04-30/` — visual assets for the detector benchmark week.

- `chart_ranking.png`: macro-AUC ranking across 15 models.
- `chart_heatmap.png`: per-target AUC heatmap.
- `chart_roc_milk.png`: ROC curves for the `milk` target.
- `chart_auc_concept.png`: explanatory AUC diagram.
- `sample_photo.jpg`: representative Google Glass evaluation image.

## Reliability Ranking 2026-05-07

Folder `reliability-ranking-2026-05-07/` — visual assets for the localisation-accuracy week. Builds on the previous benchmark by adding manual review of top-1 boxes and the combined Reliability metric.

- `chart_combined_ranking.png`: AUC vs LocAcc vs Reliability bars for the top 5 reviewed models.
- `chart_verdict_dist.png`: stacked bar of correct / partial / wrong / ambiguous per reviewed model.
- `chart_locacc_heatmap.png`: localisation accuracy heatmap per (model, target).
- `chart_problem_example.png`: real failure case — CLIP+SKU at 0.997 confidence pointing to the wrong box.
- `Lab-meeting-2026-05-07-Reliability-ranking.pptx`: full slide deck.

## Scene Predicates 2026-05-14

Folder `scene-predicates-2026-05-14/` — Glass deployment, OWLv2-B threshold analysis, and the move from "detector + threshold" to "evidence + predicates + voice policy".

- `owlv2_base_negative_distribution.png`: D⁻ exponential fit + 95%-FPR threshold curve (the global one, aggregated across all targets).
- `owlv2_base_item_thresholds.png`: per-item recommended thresholds (Codex version).
- `per_target_thresholds_detailed.png`: same per-target analysis, alternate layout — for each of the 17 targets shows the D⁺ range (green bar), the worst false positive (red dot), and the safe threshold (green diamond = `max(D⁻) × 1.05`). Demonstrates that even inside ONE model the safe threshold ranges from 0.206 (pineapple) to 0.568 (orange juice) — a 2.8× ratio.
- `per_target_thresholds_cards.png`: alternative compact view of the per-target threshold table.
- `scene_predicates_architecture.png`: updated system architecture with scene-recognition + LLM block and the new predicates.
- `Lab-meeting-2026-05-14-Glass-deploy-and-predicates.pptx`: full slide deck.
