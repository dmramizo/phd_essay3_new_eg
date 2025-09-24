## PhD Essay 3 — Trade Policy & Environmental Goods
# PhD Essay 3 — Trade Policy & Emerging Environmental Goods

**Research question.** What is the impact of **trade policy**—both **tariffs** and **non-tariff measures (NTMs)**—on an **emerging basket of environmental goods** (low-carbon tech: EVs, batteries, hydrogen, solar PV, wind, circular/e-waste, etc.)?

**This repo contains** a Jupyter notebook (`merge_final.ipynb`) that screens the literature, then produces descriptive figures and tables to motivate the gap and novelty of the study.

---

## View the notebook

- **GitHub (one-click):**  
  `https://github.com/<your-username>/<your-repo>/blob/main/merge_final.ipynb`
- **If GitHub is slow:** nbviewer renders reliably  
  `https://nbviewer.org/github/<your-username>/<your-repo>/blob/main/merge_final.ipynb`

> Tip: The notebook already includes rendered charts (Restart & Run All → Save before committing).

---

## Figures at a glance

All charts are saved to the `charts/` folder and embedded in the notebook:

1. **Time trend:** `chart_time_trend_tariff_vs_ntm.png`  
   Publications on environmental goods by **policy type** (Tariff vs NTM) over time.
2. **EG coverage (econometrics subset):** `bar_eg_econometrics.png`  
   Which **EG subdomains** (EV, hydrogen, PV, wind, batteries, circular/e-waste) are studied with **econometric methods**?
3. **Country/region coverage (econometrics subset):** `bar_countries_econometrics.png`  
   Top countries/regions studied, including **Global / Multi-country**.
4. **(Optional) Policy focus table (econometrics subset):** `econometrics_policy_focus.csv`  
   Split of **Tariff-only / NTM-only / Both** among econometrics papers (easy to plot).
5. **(Optional) Intersection figure:** if you ran the intersection cell,  
   `bar_intersection_causal_policy_eg.png` (or your updated *econometrics* version) shows how few papers are at the **intersection of econometrics × policy (tariff/NTM) × EG subdomain**.

---

## What the figures suggest (one-slide storyline)

- **Policy shift:** NTMs (standards/TBT/SPS/CBAM-type) dominate the recent EG literature; tariff-focused work is thinner.  
- **Topic imbalance:** Econometrics papers cluster in **circular/e-waste**, with relatively fewer on **hydrogen, EVs, batteries, PV, wind**—the very tech where trade policy is evolving fastest.  
- **Geography:** Evidence concentrates on a few actors (**China, EU, US**) and global panels; many developing regions are under-represented.  
- **Intersection gap:** Very few studies sit at **econometrics × (tariff/NTM) × specific EG subdomains**.  
- **Your contribution:** A **PPML/HDFE gravity framework** that jointly considers **tariffs + NTMs** on a **curated, emerging EG basket**, with robustness and heterogeneity (e.g., OECD vs. developing Asia, capability/ECI, extensive vs. intensive margins).

---

## Data & screening (PRISMA-consistent)

- Start from `master_dedup.csv` (duplicates removed).  
- **Field-of-Study (FoS) screening:** keep FoS aligned with **trade/economics/policy** and **environmental goods**; exclude overtly medical/clinical topics.  
- Optional tightening: require both **policy** and **EG** terms to appear in FoS (or in title/abstract), with **word-boundary** matching to avoid false positives.  
- Outputs:
  - `master_screened_by_fos.csv` (kept)  
  - `removed_by_fos.csv` (excluded)  
  - `screening_audit_by_fos.csv` (matched keywords, side labels)  
  - `prisma_counts.txt` (stepwise counts)  
  - `scr
