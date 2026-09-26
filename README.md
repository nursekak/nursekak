# Gleb Cherniy

B.S. Software Engineering, RTU MIREA (expected 2027) · Moscow  
[g.chernii08@gmail.com](mailto:g.chernii08@gmail.com)

I build backends that companies actually run, and I measure computer-vision problems instead of wrapping another detector. About three years of that mix. Applying to MS programs.

The production side is CRM, orders, attendance — schema, API, auth, UI, Docker, then someone uses it at work. The CV side is class confusion vs model scale, a C++ MOSSE lock on a detector box, and Raspberry Pi when the path has to leave the laptop.

## Research / systems

**[finegrained-yolo-scale](https://github.com/nursekak/finegrained-yolo-scale)** — at which YOLO scale do visually similar categories stop being confused?

mAP is not the claim. Primary metric is pairwise confusion on a held-out split. Sources are open-licensed only; the split is *inside each source*, so one photographer does not leak into test. After the box exists, a C++ MOSSE tracker has to lock, go Lost on a blank frame, and reacquire — a check that the box is usable in time, not only on a still.

The n→s→m sweep is not finished. Empty cells in that table are empty on purpose.

Coursework, not a paper: [PharmKursovaya](https://github.com/nursekak/PharmKursovaya) — small DNN for glaucoma progression (binary classification, accuracy + AUC).

On a Raspberry Pi I wrote C for SPI / RSSI and an OpenCV preview path ([rpiskanC](https://github.com/nursekak/rpiskanC)). Radio + video on a weak ARM board, no cloud GPU in that loop.

## Production

People click these at work.

- **[CRM](https://github.com/nursekak/CRM)** — 3D-print shop: printers, consumables, product / part / model tree, warehouse, shipments. In use at the company.
- **[OrderTrack](https://github.com/nursekak/OrderTrack)** — several client databases on one deploy, JWT / RBAC, React / TypeScript.
- **[GERMES_LK](https://github.com/nursekak/GERMES_LK)** — QR check-in, report approval, scheduled backups.
- **[DefectTrack](https://github.com/nursekak/DefectTrack)** — construction defects: statuses, assignees, attachments.

**[hh-assistant](https://github.com/nursekak/hh-assistant)** is a full product, not a script: embeddings for matching, cover-letter generation, Playwright, FastAPI dashboard, Telegram. LLM pipeline with a real UI, not a notebook.

## Stack

Go, Python, C/C++ · PostgreSQL · Docker · React / TypeScript · OpenCV, YOLO, MOSSE · Raspberry Pi
