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
- `S` is the seed index used to generate the instance.

For example:
denotes an instance with:
- 2 carriers,
- 15 customers in total,
- 2 vehicles,
- seed number 3.

---

## Instance file structure

Each instance file follows the structure described below.

### 1. Number of carriers
The first line contains a single integer:
representing the total number of carriers.

---

### 2. Number of customers per carrier
The second line contains `C` integers:
where `n_i` is the number of customers associated with carrier `i`.

---

### 3. Number of exclusive customers per carrier
The next line contains `C` integers:
where `e_i` denotes the number of exclusive customers assigned to carrier `i`.

---

### 4. Indices of retained customers
For each carrier with retained customers, a line lists the indices of those customers.

---

### 5. Number of indivisible group customer sets per carrier
The next line contains `C` integers:
where `s_i` is the number of indivisible group customer sets for carrier `i`.

---

### 6. Definition of indivisible group customer sets
For each indivisible set, a line is provided in the following format:
where:
- `k` is the number of customers in the set,
- `c_j` are the indices of customers belonging to that indivisible set.

---

### 7. Number of vehicles per carrier
The next line contains `C` integers:
where `v_i` denotes the number of vehicles available for carrier `i`.

---

### 8. Vehicle capacity
The next line contains a single integer:
representing the capacity of each vehicle.

---

### 9. Carrier depot coordinates
The following `C` lines contain two columns:
representing the geographical coordinates (x, y) of the depot of each carrier.

---

### 10. Customer data
The remaining lines describe the customers. Each line contains three values:
where:
- `x_j` and `y_j` are the geographical coordinates of customer `j`,
- `d_j` is the demand of customer `j`.

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
