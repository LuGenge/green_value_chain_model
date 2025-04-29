# green_value_chain_model
Repository for the paper "Optimizing Green Value Chains for Fertilizer and Chemical Industry in Europe", including data, code, results, and documentation for modelling cost-optimal sourcing strategies for green ammonia and methanol across Europe.

# Optimizing Green Value Chains for Fertilizer and Chemical Industry in Europe

This repository accompanies the research publication _"Optimizing Green Value Chains for Fertilizer and Chemical Industry in Europe"_ by Lucien Genge, Marius Neuwirth, Khaled Al-Dabbas, Tobias Fleiter, and Felix Müsgens.

## 📘 Overview

This work develops a spatially resolved, techno-economic optimization framework to assess green value chains for ammonia and methanol production in Europe. The study compares three value chain configurations:

- **Domestic Production** (fully local renewable-based production)
- **Hydrogen Imports** (pipeline-based hydrogen import with local synthesis)
- **Commodity Imports** (direct import of green ammonia or methanol)

It evaluates 72 industrial sites across Europe for the years 2030, 2040, and 2050 to identify least-cost sourcing strategies that balance cost-efficiency and energy sovereignty.

## 📂 Repository Structure

```
📁 data/              # Input datasets (demand, renewables, transport, costs)
📁 model/             # Python/MATLAB/GAMS code implementing the optimization models
📁 results/           # Output files (costs, maps, site-level results)
📁 figures/           # Visualizations used in the paper
📄 paper.pdf          # Final paper (or link if published externally)
📄 LICENSE
📄 README.md
```

## ⚙️ Model Description

The framework is a two-step model:

1. **Well-to-Border**: Linear programming model to determine import prices based on global production and transport costs.
2. **Border-to-Consumer**: Mixed-integer model allocating imports vs. domestic production at consumer level, accounting for inland transport and infrastructure.

## 📊 Key Outputs

- Cost-optimal sourcing decisions per site/year/commodity
- Country-level cost maps and savings potential
- Infrastructure needs for pipelines, terminals, and synthesis plants

## 📑 How to Use

1. Clone the repo:
   ```bash
   git clone https://github.com/<your-org-or-user>/green-value-chains-eu.git
   ```
2. Set up dependencies:
   ```bash
   cd model/
   # Install Python packages or set up GAMS environment
   pip install -r requirements.txt
   ```
3. Run the model:
   ```bash
   python run_model.py
   ```

4. Reproduce figures:
   ```bash
   python generate_figures.py
   ```

## 📬 Contact

For questions or collaboration, please contact [lucien.genge@b-tu.de] or open an issue.

---

**Citation**

If you use this code or data, please cite:

```
Genge, L., Neuwirth, M., Al-Dabbas, K., Fleiter, T., & Müsgens, F. (2025). Optimizing Green Value Chains for Fertilizer and Chemical Industry in Europe.
```
