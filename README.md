# Junxiang Gong — Selected Work

Master of Regional Planning candidate at Cornell University, working at the intersection of
**AI application products, data-driven decision systems and urban mobility**.  I like the part
between a messy real-world problem and something people can actually use: a product, a model,
a map, or a clear recommendation.

This repository is the index of my work.  Code lives in its own repositories; reports are in
[`reports/`](reports/).

| | Project | What it is | Links |
|---|---|---|---|
| 1 | [Stay or Return](#1-stay-or-return) | Explainable decision tool for Chinese international students — a live web product | [live](https://stayorreturn.com) · [code](https://github.com/Sidbaobao/stay-or-return-decision-support) |
| 2 | [Truck–drone collaborative delivery](#2-truckdrone-collaborative-delivery) | MILP + genetic-algorithm routing model, Shenzhen case study | [code](https://github.com/Sidbaobao/low-altitude-vrpd) · [paper](reports/low-altitude-logistics-vrpd.pdf) |
| 3 | [Mobility access and equity in Manhattan](#3-mobility-access-and-equity-in-manhattan) | Network analysis, clustering and spatial regression over 303 census tracts | [code](https://github.com/Sidbaobao/manhattan-mobility-access) · [report](reports/manhattan-mobility-access.pdf) |
| 4 | [Multi-modal accessibility in Shenzhen](#4-multi-modal-accessibility-of-essential-services-in-shenzhen) | GIS network analysis of hospital, school and park access by four modes | [report](reports/shenzhen-multimodal-accessibility.pdf) |
| 5 | [Planning reports](#5-planning-and-research-reports) | TOD plan, historic-district design guidelines, 15-minute city, community research | [`reports/`](reports/) |

---

## 1. Stay or Return

**A transparent decision tool for Chinese international students weighing whether to stay in the
U.S. or return to China.**  [stayorreturn.com](https://stayorreturn.com) ·
[source](https://github.com/Sidbaobao/stay-or-return-decision-support)

Stay or Return breaks a deeply personal decision into 24 questions across career, finances,
immigration, family, lifestyle and long-term development.  Users decide how much each dimension
matters, see what is pulling them in either direction, and leave with a decision memo rather than
a black-box recommendation.

The first version displayed "stay" and "return" as separate scores.  Because the two values were
mathematically complementary, that presentation exaggerated the information in the result.  I
rebuilt the experience around a single **weighted-gap model** with a bipolar scale, a confidence
range, key drivers, uncertain dimensions and a sensitivity analysis.

- Designed the product flow, questionnaire, weighting system, scoring explanation and report
- Local profiles and a ten-result history without user accounts
- Shared results are encoded in URL fragments, so the server never receives the answers
- Backend statistics limited to coarse anonymous counts by direction and confidence
- Homepage video cut from 56.4 MB to 2.6 MB with lazy loading

*Next.js 15 · TypeScript · Tailwind CSS · d3-hierarchy · Vercel KV · Vercel.*  Designed and
developed independently; team collaboration on promotion.

## 2. Truck–drone collaborative delivery

**A routing and task-allocation model that compares three ways of serving the same urban
delivery network — trucks only, drones only, and a coordinated truck + drone fleet.**
[code](https://github.com/Sidbaobao/low-altitude-vrpd) ·
[paper](reports/low-altitude-logistics-vrpd.pdf)

One depot, 50 customers with fixed demand, and an efficiency indicator that weights delivery
time against transport cost.  The three fleets are formulated as mixed-integer linear programs
(capacity, drone range, routing and assignment constraints); the collaborative case is solved
with a two-stage method — warm-start seeds → genetic algorithm → warm-started Gurobi MILP.

- In the Shenzhen case study the coordinated fleet reaches the lowest efficiency indicator
  (Z = 56.77 against 57.54 truck-only and 58.14 drone-only): it finishes the round 20 % faster
  than trucks alone for 0.5 % more total cost, with the drones taking the two outlying clusters
- The ranking holds for every time weight ≥ 0.52, for values of time above ≈ 270 CNY/min, and on
  10 of 10 random instances in a robustness study
- The repository is a tested reproduction package: one instance for all groups, an independent
  feasibility verifier, tables and figures regenerated from code, continuous integration

*Python · Gurobi · mixed-integer linear programming · genetic algorithm · matplotlib.*

## 3. Mobility access and equity in Manhattan

**To what extent do tract-level socioeconomic characteristics explain inequalities in access to
public and shared mobility in Manhattan?**
[code](https://github.com/Sidbaobao/manhattan-mobility-access) ·
[report](reports/manhattan-mobility-access.pdf)

OpenStreetMap mobility data (1,677 local bus stops, 842 subway entrances, 702 bike-share
stations) combined with ACS 2020 5-year estimates and TIGER/Line boundaries for the 303 census
tracts of Manhattan.  Walking times are computed on an OSMnx pedestrian network with
multi-source Dijkstra shortest paths; K-means (elbow method) identifies four accessibility
typologies; mode-specific OLS models with spatial-lag controls relate them to poverty, density,
race and commuting.

- Subway entrances take longer to reach than bus stops or bike-share stations; access is weakest
  along river-edge tracts and, for the subway, in East Harlem
- Midtown and the Financial District form the high-access cluster (≈ 1 min to a bus stop,
  2.7 min to a subway entrance, 1.4 min to a bike-share station)
- Poverty is associated with longer walking times to buses and subways; racial composition is
  not statistically significant in the models

*Python · OSMnx · GeoPandas · networkx · scikit-learn · statsmodels · libpysal.*

## 4. Multi-modal accessibility of essential services in Shenzhen

**How evenly can residents of Shenzhen Bay, Qianhai and Houhai reach hospitals, schools and
parks by walking, cycling, driving and metro?**
[report](reports/shenzhen-multimodal-accessibility.pdf)

An ArcGIS Pro network analysis that measures travel time from residential hexagons to the
nearest hospital, school and park by four modes, then quantifies the "privilege gap" between
car and metro access for every neighbourhood.

*ArcGIS Pro · Network Analyst · OD cost matrix · Python (pandas, matplotlib).*

## 5. Planning and research reports

| Report | Topic |
|---|---|
| [Classen Corridor transit-oriented development plan](reports/classen-corridor-tod-plan.pdf) | Corridor-scale TOD proposal for Oklahoma City connecting land use, street design, mobility and the public realm |
| [Shamian Historic District signage design guidelines (excerpt)](reports/shamian-signage-guidelines-excerpt.pdf) | Selected contribution to a 256-page implementation guide covering sign placement, materials, lighting and approval for 157 buildings in Guangzhou |
| [The 15-minute city in China](reports/15-minute-city-china.pdf) | Exploratory study of proximity, accessibility and implementation strategies |
| [Haikou Mission Hills community satisfaction](reports/haikou-mission-hills-satisfaction.pdf) | Survey research comparing how residents and visitors experience a tourism-oriented new community |

## Toolkit

| | |
|---|---|
| Product & AI-assisted development | user research, requirements, information architecture, prototyping, usability testing, Next.js, TypeScript |
| Data & machine learning | Python, SQL, pandas, clustering, regression, statistical analysis, data visualization |
| Optimization | Gurobi, mixed-integer linear programming, routing models, heuristic algorithms, scenario analysis |
| Spatial analytics | ArcGIS Pro, OSMnx, GeoPandas, network analysis, accessibility analysis |
| Communication | industry research, structured problem-solving, client-facing reports, presentations, Chinese and English |

## Current focus

Exploring 2027 graduate opportunities in AI application products, enterprise solutions, product
strategy, business analysis and technology consulting.
