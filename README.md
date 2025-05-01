# Persistence Entropy Relates Rest-Activity During Pregnancy to Unfavorable Health Outcomes in Maternal and Newborn Health

This repository contains the thesis and supporting code for the Master’s thesis submitted by **Sashiel Vagus** to **San Diego State University** in Spring 2024, in partial fulfillment of the requirements for the degree **Master of Science in Applied Mathematics**, with a concentration in **Dynamical Systems**.

📄 **Full Thesis**: [`2024_Math_Thesis_Template.pdf`](./2024_Math_Thesis_Template.pdf)  
📊 **Main Notebook**: [`Rips_dim1_extended.ipynb`](./Rips_dim1_extended.ipynb)

---

## 🧠 Project Summary

This thesis applies **topological data analysis (TDA)** — specifically **persistent entropy** — to actigraphy data collected from pregnant women during gestation weeks 22 and 32. Persistent entropy quantifies disorder in temporal patterns and is used here to assess correlations between **rest-activity rhythms** and **maternal and newborn health outcomes**.

Key findings show that:
- High persistent entropy (>8.22) at gestation week 22 was associated with increased pregnancy complications.
- Greater **day-to-day variability** in entropy was linked to **more frequent adverse outcomes**.
- Women with **high BMI and high entropy** were most likely to experience complications.


---

## 🔬 Methodology

- **Data**: Actigraphy wrist-worn device (30-sec epoch) from G22 (n=41) and G32 (n=44)
- **Processing Steps**:
  1. Resample actigraphy point clouds using **Greedy Permutation**
  2. Apply **Vietoris–Rips filtration** via `ripser`
  3. Compute persistence diagrams (dimension 0)
  4. Calculate entropy using `persim` and `numpy`
  5. Compare across groups using Mann-Whitney U and Fisher tests

---

## 🛠 Technologies Used

- Python 3.8+
- Libraries:
  - `ripser`, `persim`, `scikit-tda`
  - `numpy`, `pandas`, `matplotlib`

---

## 🧪 Results

- Women with entropy values **above 8.22** were significantly more likely to have pregnancy complications.
- The **variability** in entropy across days was also strongly associated with maternal or newborn complications.
- Persistent entropy captures latent structure in actigraphy data missed by standard statistical measures.

---

## 👥 Thesis Committee

- **Chair**: Dr. Uduak George (Mathematics & Statistics)  
- **Committee Members**:
  - Dr. Jérôme Gilles (Mathematics & Statistics)  
  - Dr. Emily Schmied (Public Health)  
- **Data Provider**: Dr. Theresa Casey (Purdue University)

---

## 📚 Citation

> Vagus, S. (2024). *Persistence Entropy Relates Rest-Activity During Pregnancy to Unfavorable Health Outcomes in Maternal and Newborn Health* (Master’s thesis, San Diego State University).

---

## 📩 Contact

**Sashiel Vagus**  
Email: svagus@sdsu.edu  
GitHub: [@sashielvagus](https://github.com/sashielvagus)

---

## 🪪 License

This repository is shared for academic, educational, and research purposes. For reuse or collaboration, please contact the author.
