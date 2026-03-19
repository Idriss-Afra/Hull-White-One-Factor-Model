# Hull-White One Factor Model

A quantitative finance repository focused on implementing the **Hull-White one-factor short-rate model** for interest-rate derivatives.

This project develops the **Hull-White model dynamics**, calibrates the model to **European swaption quotes**, and applies it to the pricing of **Bermudan swaptions through a PDE-based approach**.

---

## Repository Structure

```text
Hull-White-One-Factor-Model/
├── Hull-White One Factor Model.ipynb
└── Hull-White One Factor Model Documentation.pdf
```

---

## Project Overview

This notebook focuses on the **Hull-White one-factor model** for interest-rate derivatives.

It starts from the standard short-rate dynamics under the risk-neutral measure and derives the associated **zero-coupon bond pricing formula**. The model is first applied to the pricing of **European swaptions** through **Jamshidian’s decomposition**, before being extended to an **analytical calibration framework** and a **PDE-based pricing method** for **Bermudan swaptions**.

The model calibration is performed on a basket of **European swaptions**. In this implementation, the **mean-reversion parameter** is fixed, while the short-rate volatility is modeled as **piecewise constant across expiries**. The notebook first calibrates the short-rate total variance term structure and then strips the corresponding volatility curve.

---

## Documentation

The repository also includes a dedicated PDF:

* `Hull-White One Factor Model Documentation.pdf`

This document provides the theoretical derivation supporting the European swaption pricing formula under the Hull-White model.

---

## Example Output

**EURIBOR-6M European diagonal ATM swaptions with an expiry/tenor structure of 2Y/13Y, 3Y/12Y, ..., 14Y/1Y**:

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/c9f8a208-4933-4d89-bed8-4f48e1677a72" />

---

## Best use case

Use this notebook when working with **interest-rate derivatives** and building a **Hull-White pricing framework** for calibration and the valuation of **European** and **Bermudan swaptions**.

---

## How to Use

Clone the repository:

```bash
git clone https://github.com/Idriss-Afra/Hull-White-One-Factor-Model.git
cd Hull-White-One-Factor-Model
jupyter notebook
```

Then open:

* `Hull-White One Factor Model.ipynb`

---

## Author

**Idriss Afra**
