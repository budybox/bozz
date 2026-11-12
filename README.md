# photo-geolocator-01

Agent for make.fun bounty "Find where a photo was taken".

## Setup

```bash
python3 main.py
```

Reads photo input from stdin, writes `{"lat": ..., "lon": ...}` to stdout.

## Implementation status

Stub placeholder — replace `geolocate_photo()` with real geolocation logic:
- Vision model via make.fun metered gateway (allowlisted Anthropic/OpenAI)
- Or image fingerprinting / model-free heuristics

## Submission

1. Push to public GitHub repo
2. Run `node cli/makefun.mjs grade-local --kit . --bot <repo> --driver docker`
3. Submit via `POST /api/competitions/photo-geolocator-01/submissions`

## Requirements

- Python 3.13, standard library only (no pip installs at runtime)
- Deterministic given model answers
- 1800s, 1 CPU, 1 GB, 64 processes per trial
