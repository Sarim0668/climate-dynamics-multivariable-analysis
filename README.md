# 🌍 Climate Dynamics: Multivariable Modeling and Analysis

## Temperature Prediction Using Gradient Vectors, Directional Derivatives, and Triple Integrals

### 👥 Team Members

| Name | ID | Section |
|------|-----|---------|
| Abdullah Junaid | 24I-0569 | A |
| Muhammad Usman Mahboob | 24I-0724 | A |
| Muhammad Sarim | 24I-0668 | A |

---

## 📖 Overview

This project explores the relationship between temperature, time, humidity, and altitude using 30-day climate data from major global cities. By applying **multivariable calculus concepts** including gradient vectors, directional derivatives, steepest descent, and triple integrals, we model temperature as a function of three variables and analyze climate dynamics.

---

## 🎯 Objectives

| Objective | Description |
|-----------|-------------|
| **Model Temperature** | Create function T(time, humidity, altitude) using sklearn |
| **Find Extremes** | Predict hottest and coldest conditions |
| **Gradient Analysis** | Compute ∇T to find fastest temperature increase direction |
| **Steepest Descent** | Identify direction of most rapid cooling |
| **Directional Derivatives** | Predict temperature changes in custom directions |
| **Triple Integrals** | Estimate thermal load over defined regions |
| **City Analysis** | Identify hottest and coldest cities globally |

---

## 🧮 Mathematical Framework

### 1. Temperature Function Model

Using sklearn's linear regression, we modeled:
T(t, h, a) = β₀ + β₁·t + β₂·h + β₃·a

Where:
- **t** = Time (hour of day)
- **h** = Humidity (%)
- **a** = Altitude (meters)

### 2. Gradient Vector
∇T(t, h, a) = (∂T/∂t, ∂T/∂h, ∂T/∂a) = (β₁, β₂, β₃)


### 3. Directional Derivative
D_u T = ∇T · û

Where **u** is the direction vector of interest.

### 4. Triple Integral
∫∫∫_R T(t, h, a) dt dh da

Represents accumulated thermal energy over region **R**.

---

## 🛠️ Technical Stack

| Category | Technologies |
|----------|--------------|
| Language | Python |
| Machine Learning | Scikit-learn (Linear Regression) |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib |
| Calculus Operations | Manual computation + Python |

## 📊 Key Results
Model Coefficients
Variable	Coefficient	Interpretation
Time (t)	β₁	Negative relationship
Humidity (h)	β₂	Strongest positive influence
Altitude (a)	β₃	Negative relationship
Hottest & Coldest Conditions
Condition	Time	Humidity	Altitude	Temperature
Hottest	[Value]	[Value]	[Value]	[Value] °C
Coldest	[Value]	[Value]	[Value]	[Value] °C
Gradient Vector Analysis
At point (t₀, h₀, a₀):

∇T = (∂T/∂t, ∂T/∂h, ∂T/∂a) = (β₁, β₂, β₃)
Fastest Increase Direction: ∇T itself

Fastest Decrease Direction: -∇T (Steepest Descent)

Triple Integral Result
Over region R: t ∈ [5,10], h ∈ [40,60], a ∈ [10,500]

∫∫∫_R T(t,h,a) dt dh da = [Value] (thermal load units)
City Rankings
Rank	City	Average Predicted Temperature
Hottest	[City Name]	[Value] °C
Coldest	[City Name]	[Value] °C
📈 Visualizations
Methodology Flowchart
Shows step-by-step approach to solving the climate modeling problem.

Gradient Vector Visualization
Illustrates the direction of fastest temperature increase.

City Temperature Comparison
Bar chart comparing average temperatures across all cities.

## 🔬 Technical Insights
### 1. Humidity Dominance
Humidity emerged as the strongest influence on temperature, with the highest coefficient magnitude. This aligns with real-world physics where moisture content significantly affects heat retention.

### 2. Gradient Interpretation
The gradient vector ∇T points in the direction of greatest temperature increase. By analyzing its components, we can identify which variable (time, humidity, or altitude) most strongly influences temperature at any given point.

### 3. Steepest Descent Application
The negative gradient (-∇T) provides optimal cooling directions. This has practical applications in:

HVAC system optimization

Urban planning for heat reduction

Agricultural cooling strategies

### 4. Directional Derivatives
By selecting custom directions (e.g., increasing altitude while decreasing humidity), we can predict specific temperature changes, useful for:

Mountain weather forecasting

Climate change impact assessment

Travel/activity planning

### 5. Triple Integral Meaning
The triple integral over a region represents total thermal load, which can be interpreted as:

Energy required to cool/heat a region

Heat accumulation over time and space

Climate stress indicator for ecosystems

## 🌍 Real-World Applications
Application	Mathematical Tool Used
Weather Forecasting	Gradient & Directional Derivatives
Climate Change Modeling	Triple Integrals
Urban Heat Island Analysis	Steepest Descent
Agricultural Planning	Temperature Extremes Prediction
HVAC System Design	Gradient Optimization


---

## 🚀 How to Run

### Clone Repository
```bash
git clone https://github.com/your-username/climate-dynamics-multivariable-analysis.git
cd climate-dynamics-multivariable-analysis
