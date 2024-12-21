# Consumer-Behavior-Perfume-Packaging
This project examines the impact of color vs. black-and-white packaging on Dior perfume purchase intent in NYC. Using surveys and simulation data for 384 participants, it analyzes attention, interest, and purchase behavior. Results offer insights into packaging design's influence on luxury consumer behavior.


This project analyzes the impact of color versus black-and-white product packaging on consumers' purchase intent, with a focus on potential Dior perfume consumers in New York City. The research targets adults who can afford luxury goods, including Dior’s current and prospective customers. Through a stratified sampling approach, surveys are distributed both in Dior's physical stores and online, allowing for representation across different customer segments. Participants are incentivized with early access to a Dior product launch.

The project measures variables such as attention to packaging, interest, compelled to purchase, and actual purchase behavior. The primary outcome is whether participants make a purchase based on packaging design. Additionally, I coded simulation data to estimate various outcomes and validate the robustness of the sample size and statistical power assumptions.

The _pwr_ package is used to calculate the required sample size based on:
Population Size: 410,740
Confidence Level: 95%
Margin of Error: 5%
Proportion: 50% (default for maximum sample size)
The formula incorporates finite population correction to ensure accuracy for smaller populations.

**Key Probabilities:**
Treatment Group:
Attention: 70%
Interest: 60%
Compelled: 60%
Purchase: 50%
Control Group:
Attention: 65%
Interest: 55%
Compelled: 45%
Purchase: 40%
No Effect Simulation
Simulates scenarios with no treatment effect to act as a baseline comparison.

**Statistical Analysis**
For each outcome metric, t-tests are performed to compare treatment and control groups:

Captures Attention
Influences Interest
Compelled to Purchase
Purchased Item

Each test provides:
T-statistic
P-value
Mean estimates
Confidence intervals
Degrees of freedom
Testing method

**Dependencies**
This code requires the following R packages:

pwr
data.table
DT
stats (built-in)
base (built-in)

**Install these packages using:** r
Copy code
```bash
install.packages(c("pwr", "data.table", "DT"))
```

**Usage**
Clone this repository.
Install the required R packages.
Run the scripts sequentially:
Power/Sample Size Calculation
Effect and No Effect Data Simulation
Statistical Analysis
Model Fitting
Use the interactive data table (DT) to explore results in detail.
