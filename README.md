Junxiang Gong — Selected Work

I am a Master of Regional Planning candidate at Cornell University, interested in AI application products, data-driven decision systems, and enterprise solutions. My work ranges from shipping a privacy-first web product to modeling vehicle-drone delivery and studying urban mobility with machine learning.

I enjoy the part between identifying a messy real-world problem and turning it into something people can actually use: a product, a model, a map, or a clear recommendation.

Featured Projects

1. Stay or Return

A transparent decision tool for Chinese international students weighing whether to stay in the U.S. or return to China.

Live Website · Source Code

Stay or Return breaks a deeply personal decision into 24 questions across career, finances, immigration, family, lifestyle, and long-term development. Users decide how much each dimension matters, see what is pulling them in either direction, and leave with a decision memo rather than a black-box recommendation.

The first version displayed “stay” and “return” as separate scores. Because the two values were mathematically complementary, that presentation exaggerated the amount of information in the result. I rebuilt the experience around a single weighted-gap model, with a bipolar scale, confidence range, key drivers, uncertain dimensions, and sensitivity analysis.

Designed the product flow, questionnaire, weighting system, scoring explanation, and report

Built local profiles and a ten-result history without requiring user accounts

Encoded shared results in URL fragments so the server never receives the underlying answers

Limited backend statistics to coarse anonymous counts by direction and confidence

Reduced the homepage video from 56.4 MB to 2.6 MB and added lazy loading

Built with: Next.js 15 · TypeScript · Tailwind CSS · d3-hierarchy · Vercel KV · Vercel

Designed and developed independently, with team collaboration on promotion.

2. Mobility Accessibility and Equity in Manhattan

A machine-learning and spatial analysis of walking access to bus stops, subway entrances, and bike-share stations across Manhattan.

View Full Report

This study asks whether Manhattan’s dense transportation network is equally accessible at the neighborhood level. I combined OpenStreetMap mobility data with ACS socioeconomic estimates and TIGER/Line boundaries for 303 census tracts, covering 3,221 bus stops, subway entrances, and bike-share stations.

Walking times were calculated on an OSMnx network with multi-source Dijkstra shortest paths. I then used robust scaling and K-means clustering to identify four accessibility patterns, followed by mode-specific OLS models with spatial-lag controls to test how those patterns relate to poverty, population density, race, and commuting behavior.

Built a tract-level dataset from three public data sources

Measured network-based walking time instead of straight-line proximity

Used K-means to identify four mobility-access typologies

Found persistent access gaps along river-edge tracts and weaker subway access in East Harlem

Found that poverty was associated with longer access times for buses and subways, while racial composition was not statistically significant in the models

Methods: Python · OSMnx · GeoPandas · Network Analysis · K-means Clustering · Spatial Regression

3. Vehicle–Drone Fulfillment Network Optimization

A routing and task-allocation model for coordinating ground vehicles and delivery drones in a multi-node fulfillment network.

View Full Report

The project compares three ways to serve the same 50-customer network: vehicles only, drones only, and a coordinated mixed fleet. I modeled capacity, range, travel distance, service time, cost, and task allocation, then designed a hybrid solution method combining mixed-integer linear programming, nearest-neighbor initialization, a genetic algorithm, and Gurobi warm starts.

In the Shenzhen case study, the coordinated model assigned high-demand areas to vehicles and scattered or remote orders to drones. Compared with vehicle-only delivery, it reduced completion time by 42%, vehicle travel distance by 16%, and total cost by 2%. The composite efficiency measure improved by 4% over vehicle-only delivery and 5% over drone-only delivery.

Formulated CVRP, UAVRP, and coordinated vehicle-drone scenarios

Built capacity, endurance, routing, and assignment constraints

Combined exact optimization with heuristic search for a practical solve process

Compared time, distance, cost, and fleet utilization across operating models

Built with: Python · Gurobi · Mixed-Integer Linear Programming · Genetic Algorithm · pandas

Additional Research and Planning Work

Multi-Modal Accessibility Analysis in Shenzhen — Compared access to hospitals, schools, and parks by walking, cycling, driving, and public transit across Shenzhen Bay, Qianhai, and Houhai.

Shamian Historic District Signage Design Guidelines — Selected contribution to a 256-page implementation guide covering sign placement, dimensions, materials, color, lighting, approval, and ongoing supervision across 157 buildings in Guangzhou’s Shamian Historic District.

Strategic Analysis of the 15-Minute City in China — An exploratory study of proximity, accessibility, and implementation strategies for 15-minute-city development in China.

Classen Corridor Transit-Oriented Development Plan — A corridor-scale TOD proposal connecting land use, street design, mobility, and public-realm improvements in Oklahoma City.

Haikou Mission Hills Community Satisfaction Research — Survey-based research comparing how residents and visitors experience a tourism-oriented new community.

Toolkit

Product and AI-assisted development: User research, requirements, information architecture, prototyping, usability testing, Next.js, TypeScript

Data and machine learning: Python, SQL, pandas, clustering, regression, statistical analysis, data visualization

Optimization: Gurobi, mixed-integer linear programming, routing models, heuristic algorithms, scenario analysis

Spatial analytics: ArcGIS Pro, OSMnx, GeoPandas, network analysis, accessibility analysis

Communication: Industry research, structured problem-solving, client-facing reports, presentation development, Chinese and English

Current Focus

I am exploring 2027 graduate opportunities in AI application products, enterprise solutions, product strategy, business analysis, and technology consulting.
