# Genrated instances for carrier collaborative VRP

This repository contains the synthetic benchmark instances used in the computational experiments of the paper:

**[Carrier Collaborative Vehicle Routing Problem with Shared Customer Demands and Vehicle Capacities]**  
(submitted to *Computers & Operations Research*).

The instances are provided in plain text format (`.txt`) and were generated specifically for this study.

---

## File naming convention

Each instance file is named as:


where:
- `C` is the number of carriers,
- `N` is the total number of customers,
- `V` is the total number of vehicles,
- `T` is the seed index used to generate the instance.
---

## Instance file structure

Each instance file follows the structure described below.

### 1. Number of carriers (|C|)
representing the total number of carriers.

---

### 2. Number of customers per carrier (|N_c| , N_c ⊆ N )
where `N_c` is the number of customers associated with carrier `c`.

---

### 3. Number of retained customers per carrier (|N_c^r|)
where `N_c^r` denotes the number of retained customers assigned to carrier `c`.

---

### 4. Indices of retained customers (N_c^r)
For each carrier with retained customers, a line lists the indices of those customers.

---

### 5. Number of indivisible group customer sets per carrier (S_g^c⊆N_c)
where `g` is the number of indivisible group customer sets for carrier `c`.

---

### 6. Definition of indivisible group customer sets 
 the indices of customers belonging to that indivisible set.

---

### 7. Number of vehicles per carrier (V_c)
where `V_c` denotes the number of vehicles available for carrier `c`.

---

### 8. Vehicle capacity (Q)
representing the capacity of each vehicle.

---

### 9. Carrier depot coordinates
representing the geographical coordinates (x, y) of the depot of each carrier.

---

### 10. Customer data
The remaining lines describe the customers. Each line contains three values:
where:
- `x_i` and `y_i` are the geographical coordinates of customer `i`,
- `q_i` is the demand of customer `i`.

---

## Usage

All computational results reported in the paper were obtained using **exactly** the instances provided in this repository.
These instances can be used to reproduce the experiments described in the paper.

---

## Notes
- All instances are synthetic.
- The instance generator is not publicly released.
- Only the final benchmark instances used in the experiments are provided.

---

## Contact
For questions regarding the instances, please contact:  
[hormozzadeparisa@gmail.com]
