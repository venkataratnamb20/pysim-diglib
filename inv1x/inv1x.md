# CMOS Inverter: inv1x

## Directory structure
```
inv1x
    - inv1x.asc
	- inv1x.sym
	- inv1x_tb_op.asc
	- inv1x_tb_dc.asc
	- inv1x_tb_tran.asc
	- inv1x_tb_ac.asc
	- inv1x.md
```

## Schematic

Following Figure shows the schematic of a inverter.

<center>
<img src="https://github.com/Balakrishna-RK/Balakrishna-RK/raw/main/Projects/Design_and_Analysis_of_CMOS_Inverter%3A_Schematic_Design_Layout_Design_and_LVS_Validation_using_SKY130_PDK/assets/images/schematic_circuit/inv_circuit.png" alt="inv1x schematic" />
</center>

**Design parameters**

param|value|Comments|
-----|-----|------|
ln | 180n |Minimum length|
wn | 360n |Twice the Minimum length|
mn | 1 |taken for unit inverter|
lp | 180n |Minimum length|
wp | 720n |Twice the nmos Width|
mp | 1 |taken for unit inverter|


## Symbol

<center>
<img src="https://github.com/Balakrishna-RK/Balakrishna-RK/raw/main/Projects/Design_and_Analysis_of_CMOS_Inverter%3A_Schematic_Design_Layout_Design_and_LVS_Validation_using_SKY130_PDK/assets/images/schematic_circuit/inv_symbol.png" alt="inv1x symbol" />
</center>

## Testbench

<center>
<img src="https://github.com/Balakrishna-RK/Balakrishna-RK/raw/main/Projects/Design_and_Analysis_of_CMOS_Inverter%3A_Schematic_Design_Layout_Design_and_LVS_Validation_using_SKY130_PDK/assets/images/schematic_circuit/inv_circuit.png" alt="inv1x schematic" />
</center>

## Simulation plan
1. DC Op
2. DC Transfer
3. Transient
4. AC Analysis

### DC Transfer Char
This is aimed to plot DC transfer characteristics and find the **gain** and **noise margins**.

<center>
<img src="https://github.com/Balakrishna-RK/Balakrishna-RK/raw/main/Projects/Design_and_Analysis_of_CMOS_Inverter%3A_Schematic_Design_Layout_Design_and_LVS_Validation_using_SKY130_PDK/assets/images/vtc/inv_vtc_tb.png" alt="inv1x schematic" />
</center>

### Transient

fall time constant

$ time constant = Rn*Cout $

```mATH
time\ constant\ (\tau) = Ron_n*C_{out}
```
