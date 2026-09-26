# paddleocr-vl-root

Minimal derivative of the official PaddleOCR-VL image for a one-off GPU trial:
`FROM ccr-2vdh3abv-pub.cnc.bj.baidubce.com/paddlepaddle/paddleocr-vl@sha256:f5dff380c63636a9fb551877d2011ef6c4a939b2c06054854f83d399245f37ba`,
config changed only by `USER root` and `ENV HOME=/root` (needed by SkyPilot's Runpod bootstrap).
No packages, files or models are added. Built by `.github/workflows/publish.yml` with `crane`
(registry-to-registry copy of the base layers, then a config-only mutation).
