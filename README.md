<div align="center">

# Gleb Cherniy

B.S. Software Engineering · RTU MIREA (expected 2027) · Moscow

[![Email](https://img.shields.io/badge/Email-g.chernii08%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:g.chernii08@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-nursekak-181717?style=flat-square&logo=github)](https://github.com/nursekak)
[![Moscow](https://img.shields.io/badge/Moscow-Russia-1F6FEB?style=flat-square)](https://github.com/nursekak)

</div>

---

<table>
  <tr>
    <td valign="top" width="55%">

I build backends that companies actually run, and I measure computer-vision problems instead of wrapping another detector. About three years of that mix. Applying to MS programs.

The production side is CRM, orders, attendance — schema, API, auth, UI, Docker, then someone uses it at work. The CV side is class confusion vs model scale, a C++ MOSSE lock on a detector box, and Raspberry Pi when the path has to leave the laptop.

    </td>
    <td valign="top" width="45%">

**Focus**

- Research: pairwise class confusion vs detector scale, not another mAP table
- Production: tools a shop or crew actually clicks
- Right now: MS applications

    </td>
  </tr>
</table>

## Research

<table>
  <tr>
    <td valign="top">

**[finegrained-yolo-scale](https://github.com/nursekak/finegrained-yolo-scale)** — at which YOLO scale do visually similar categories stop being confused?

mAP is not the claim. Primary metric is pairwise confusion on a held-out split. Sources are open-licensed only; the split is *inside each source*, so one photographer does not leak into test. After the box exists, a C++ MOSSE tracker has to lock, go Lost on a blank frame, and reacquire — a check that the box is usable in time, not only on a still.

The n→s→m sweep is not finished. Empty cells in that table are empty on purpose.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)

    </td>
  </tr>
</table>

## Production

People click these at work.

<table>
  <tr>
    <td valign="top" width="50%">

**[CRM](https://github.com/nursekak/CRM)**

3D-print shop: printers, consumables, product / part / model tree, warehouse, shipments. In use at the company.

    </td>
    <td valign="top" width="50%">

**[OrderTrack](https://github.com/nursekak/OrderTrack)**

Several client databases on one deploy, JWT / RBAC, React / TypeScript.

    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">

**[GERMES_LK](https://github.com/nursekak/GERMES_LK)**

QR check-in, report approval, scheduled backups.

    </td>
    <td valign="top" width="50%">

**[DefectTrack](https://github.com/nursekak/DefectTrack)**

Construction defects: statuses, assignees, attachments.

    </td>
  </tr>
</table>

<table>
  <tr>
    <td valign="top">

**[hh-assistant](https://github.com/nursekak/hh-assistant)** is a full product, not a script: embeddings for matching, cover-letter generation, Playwright, FastAPI dashboard, Telegram. LLM pipeline with a real UI, not a notebook.

    </td>
  </tr>
</table>

## Stack

<div align="center">

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white)

</div>

<details>
<summary>Coursework and edge hardware</summary>

Coursework, not a paper: [PharmKursovaya](https://github.com/nursekak/PharmKursovaya) — small DNN for glaucoma progression (binary classification, accuracy + AUC).

On a Raspberry Pi I wrote C for SPI / RSSI and an OpenCV preview path ([rpiskanC](https://github.com/nursekak/rpiskanC)). Radio + video on a weak ARM board, no cloud GPU in that loop.

</details>
