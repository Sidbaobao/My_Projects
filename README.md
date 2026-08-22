# Junxiang Gong — Selected Projects

Cornell University Master of Regional Planning candidate working across product design, data analysis, optimization, and solution development.

Most of my work sits somewhere between understanding a real-world problem and building something that makes the decision easier. Some projects become web products, while others take the form of optimization models, GIS analyses, or decision reports.

## Featured Projects

### 1. Stay or Return

**An explainable decision tool for Chinese international students choosing between staying in the U.S. and returning to China.**

[Live Website](https://stayorreturn.com) · [Source Code](https://github.com/Sidbaobao/stay-or-return-decision-support)

Choosing where to build a life is too personal for a black box. Stay or Return breaks the decision into 24 questions across six dimensions, then shows users what is pulling them in each direction and how confident that result really is.

The result is based on a transparent weighted-gap model rather than two artificial scores. Users can adjust what matters to them, inspect each dimension, test how sensitive the result is to their priorities, and generate a decision memo.

#### What it includes

* Six-step questionnaire covering career, finances, immigration, family, lifestyle, and long-term development
* Interactive bubble-based weighting with fine-grained controls
* Bipolar result view showing direction, confidence range, key drivers, and uncertain dimensions
* Local profiles and result history stored only on the user’s device
* Private sharing through URL fragments, so shared answers never reach the server
* Anonymous statistics limited to aggregated direction and confidence counts
* Print-friendly decision memo with a side-by-side comparison

**Built with:** Next.js 15 · TypeScript · Tailwind CSS · d3-hierarchy · Vercel KV · Vercel

Designed and built independently from product definition through deployment, with team collaboration on promotion.

---

### 2. Vehicle–Drone Fulfillment Network Optimization

**A network optimization model for coordinating ground vehicles and delivery drones across a multi-node fulfillment system.**

[View Full Report](./Research%20on%20Optimization%20of%20Urban%20Logistics%20Network%20Based%20on%20Low%20Altitude%20Economy%3A%20Path%20Planning%20and%20Traffic%20Impact%20Analysis%20of%20Collaborative%20Distribution%20Mode%20Between%20Drones%20and%20Ground%20Vehicles)

The difficult part of mixed-fleet delivery is not simply whether drones are faster. It is deciding which orders they should handle, how they should coordinate with ground vehicles, and whether the additional complexity creates enough operational value.

I translated the delivery process into a network model covering order locations, travel distance, vehicle capacity, drone endurance, task allocation, and fulfillment time. Python was used to prepare the node and order data, while Gurobi handled the routing and assignment constraints.

The model was tested under different order volumes and fleet configurations. Comparing fulfillment time, transportation cost, and equipment utilization showed that the coordinated solution could improve overall efficiency by approximately 5% over the baseline.

#### Model scope

* Joint routing and task allocation for vehicles and drones
* Capacity, endurance, distance, and fulfillment-time constraints
* Multi-scenario comparison across different demand and fleet settings
* Performance evaluation based on time, cost, and equipment utilization
* Operational recommendations derived from the model results

**Built with:** Python · Gurobi · pandas · Jupyter Notebook

---

### 3. Multi-Modal Accessibility Analysis in Shenzhen

**A GIS-based study of how easily people can reach essential services by walking, cycling, driving, and public transport.**

[View Full Report](./A%20Multi-Modal%20Accessibility%20Analysis%20of%20Essential%20Services%20in%20Shenzhen_Junxiang%20Gong_jg2582.pdf)

A facility may look close on a map and still be difficult to reach once street connections, travel modes, and station entrances are taken into account. This project examines that difference across Shenzhen Bay, Qianhai, and Houhai.

I combined origin points, road networks, public transport stops, station entrances, and the locations of hospitals, schools, and parks. Separate accessibility measurements were created for each travel mode and compared against 15-minute service thresholds.

The results revealed clear differences between facility types and neighborhoods. Parks generally had stronger coverage, while access to hospitals was the most limited. The final maps were used to identify underserved locations and suggest where transport connections or public-service provision could be improved.

#### Analysis

* Combined transport, facility, and spatial data from multiple sources
* Compared accessibility across four travel modes
* Measured service coverage using mode-specific travel assumptions
* Identified gaps in hospital, school, and park access
* Turned the analysis into maps and location-specific recommendations

**Built with:** ArcGIS Pro · Network Analysis · Spatial Analysis · Data Visualization

---

## Other Research and Planning Work

* [Strategic Analysis of the 15-Minute City in China](./Strategic%20analysis%20on%20improving%20the%20proximity%20and%20accessibility%20in%20China%20an%20exploratory%20development%20based%20on%20the%20study%20of%20the%2015-minute%20city.pdf)
* [Classen Corridor Transit-Oriented Development Plan](./%EF%BC%88%E5%B7%B2%E5%8E%8B%E7%BC%A9%EF%BC%89Classen%20Corridor%20Transit-Oriented%20Development%20Plan%20Oklahoma%20City,%20OK.pdf)
* [Haikou Mission Hills Community Satisfaction Research](./Research%20on%20Overall%20Satisfaction%20of%20Haikou%20Mission%20Hills%20New%20CityCommunity%20-%20From%20The%20Perspectives%20of%20Residents%20And%20Tourists.pdf)

## Toolkit

* **Product:** User research, requirements, information architecture, prototyping, usability testing
* **Data and optimization:** Python, SQL, Gurobi, pandas, statistical analysis, Excel
* **Spatial analysis:** ArcGIS Pro, network analysis, accessibility analysis, spatial visualization
* **Frontend:** Next.js, TypeScript, Tailwind CSS, Vercel
* **Communication:** Industry research, structured problem-solving, presentation development, Chinese and English

## Current Focus

I am interested in 2027 graduate opportunities in AI application products, enterprise solutions, product strategy, business analysis, and technology consulting.
