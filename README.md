# Junxiang Gong | Selected Projects

Cornell University Master of Regional Planning candidate focused on AI-enabled decision products, data analytics, optimization, and solution design.

This repository presents selected projects that demonstrate how I translate complex real-world problems into structured analytical models, product prototypes, and actionable recommendations.

## Featured Projects

### 1. Stay or Return

**An explainable decision tool for Chinese international students choosing between staying in the U.S. and returning to China.**

[Live Website](https://stayorreturn.com) · [Source Code](https://github.com/Sidbaobao/stay-or-return-decision-support)
Choosing where to build a life is too personal for a black box. Stay or Return breaks the decision into 24 questions across six dimensions, then shows users what is pulling them in each direction and how confident that result really is.

The result is based on a transparent weighted-gap model rather than two artificial “scores.” Users can adjust what matters to them, inspect each dimension, test how sensitive the result is to their priorities, and generate a decision memo.

#### Highlights

* Six-step questionnaire covering career, finances, immigration, family, lifestyle, and long-term development
* Interactive bubble-based weighting with fine-grained controls
* Bipolar result view showing direction, confidence range, key drivers, and uncertain dimensions
* Local profiles and result history stored only on the user’s device
* Private sharing through URL fragments, so shared answers never reach the server
* Anonymous statistics limited to aggregated direction and confidence counts
* Print-friendly decision memo with a side-by-side comparison

#### Built with

Next.js 15 · TypeScript · Tailwind CSS · d3-hierarchy · Vercel KV · Vercel

Designed and built independently from product definition through deployment, with team collaboration on promotion

---

### 2. Vehicle–Drone Fulfillment Network Optimization

**A network optimization model for coordinating ground vehicles and delivery drones across a multi-node fulfillment system.**

[View Full Report](./Research%20on%20Optimization%20of%20Urban%20Logistics%20Network%20Based%20on%20Low%20Altitude%20Economy%3A%20Path%20Planning%20and%20Traffic%20Impact%20Analysis%20of%20Collaborative%20Distribution%20Mode%20Between%20Drones%20and%20Ground%20Vehicles)

The difficult part of mixed-fleet delivery is not simply whether drones are faster. It is deciding which orders they should handle, how they should coordinate with ground vehicles, and whether that additional complexity creates enough operational value.

I translated the delivery process into a network model covering order locations, travel distance, vehicle capacity, drone endurance, task allocation, and fulfillment time. Python was used to prepare the node and order data, while Gurobi handled the routing and assignment constraints.

The model was tested under different order volumes and fleet configurations. Comparing fulfillment time, transportation cost, and equipment utilization showed that the coordinated solution could improve overall efficiency by approximately 5% over the baseline.

#### Highlights

* Joint routing and task allocation for vehicles and drones
* Capacity, endurance, distance, and fulfillment-time constraints
* Multi-scenario comparison across different demand and fleet settings
* Performance evaluation based on time, cost, and equipment utilization
* Operational recommendations derived from the model results

#### Built with

Python · Gurobi · pandas · Jupyter Notebook

### 3. Multi-Modal Accessibility Analysis in Shenzhen

A spatial data analysis project evaluating access to essential public services through walking, cycling, driving, and public transportation.

I integrated transport networks, public facilities, and spatial data to measure service coverage, identify underserved areas, and translate analytical results into planning and resource-allocation recommendations.

**Key areas:** Multi-source data integration, accessibility analysis, spatial visualization, decision support

**Tools:** ArcGIS Pro, GIS network analysis, spatial data visualization

[View Full Report](./A%20Multi-Modal%20Accessibility%20Analysis%20of%20Essential%20Services%20in%20Shenzhen_Junxiang%20Gong_jg2582.pdf)

## Additional Research and Planning Work

* [Strategic Analysis of the 15-Minute City in China](./Strategic%20analysis%20on%20improving%20the%20proximity%20and%20accessibility%20in%20China%20an%20exploratory%20development%20based%20on%20the%20study%20of%20the%2015-minute%20city.pdf)
* Classen Corridor Transit-Oriented Development Plan
* Haikou Mission Hills Community Satisfaction Research

## Skills

**Product and Solution Design:** User needs analysis, product requirements, information architecture, prototyping, testing and iteration

**Data and Optimization:** Python, SQL, Gurobi, scenario analysis, statistical analysis, Excel

**Spatial Analytics:** ArcGIS Pro, accessibility analysis, spatial visualization

**Communication:** Industry research, structured problem-solving, presentation development, English and Chinese professional communication

## About Me

I am interested in AI application products, enterprise solutions, digital transformation, product strategy, and data-driven consulting. My background combines urban systems, industry research, product prototyping, and quantitative analysis.
