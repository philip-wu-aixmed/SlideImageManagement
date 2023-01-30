# Scanned Slide Images Management

#### © 2022-2023 AIxMed, Inc. All Rights Reserved

### Purpose
To record metadata of scanned slide images for each customer.
The metadata includes slide label, scanned image filename, scanner information (model, MPP, ICC profile, ..., etc.), inference model version, inference 

### Naming Convention
This naming covention was defined by clinical team at Octocer 21, 2022.
#### Slide ID
The naming convention for Slide ID is `Internal ID`+`profile number`, broken down into following fields:
+ Internal ID
  + serial number, hospital institution, years, category, preparation&ROI
+ profile number
  + scanner&location, layers&interval, ICC profile, focus type, date, round (scanned times)

| Field              | Description |
| :---               | :---        |
| Serial No.         | 6-digit number |
| Hospital | TN: Tungs<br> VP: VGHTPE<br> VT: VGHT |
| Years | 22: 2022, 23: 2023, ... |
| Category | N: NHGUC<br> A: Atypia<br> S: SHGUC<br> H: HGUC |
| Preparation & ROI  | C_: Cytospin<br> CR: Cytospin right<br> CL: Cytospin left<br> S_: Surepath<br> T_: Thinprep<br> TU: Thinprep urocyte |
| Scanner & Location | L1: Leica(AixMed)<br> H1: Hamamatsu(VGH) |
| Layers & Interval | 0101: 1 layer with 0.1um<br> 2110: 21 layers with 1um |
| ICC profile | AT2, SS1, XXX, ... |
| Focus type | D: Default<br> X: maximum<br> M: manual |
| Date | 4-digit number, i.e. mmdd |
| Round | R1: first scan<br> R2: re-scan |

### Note
#### De-Identification
It needs to do the de-identification process on this data sheet, espcially on the fields of `Slide Label` and `Patient ID`|  ss
