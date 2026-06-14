# `docs/assets/`

Put your case-study GIFs and figures here. The `index.html` expects:

- `base.gif`             — base model rollout (top, light-yellow panel)
- `train.gif`            — trained model rollout (bottom, light-green panel)
- `results_valid.png`    — Valid% per map size chart
- `results_optimal.png`  — Optimal% per map size chart

If you generated the GIFs with `generate_mapf_animation.py`:

```bash
# Two single GIFs (recommended: one per panel)
python generate_mapf_animation.py \
    --input video_compare/base.jsonl  --output docs/assets/base.gif
python generate_mapf_animation.py \
    --input video_compare/train.jsonl --output docs/assets/train.gif
```

Optional charts can be exported from your existing plot scripts in `plot/`,
e.g. `plot/plot_4methods_grid.py`, and copied to `docs/assets/`.
