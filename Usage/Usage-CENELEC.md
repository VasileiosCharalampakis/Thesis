# Usage Guide for the CENELEC Standard

## Prerequisites

To successfully use the Safety Assessment Software with the CENELEC standard, please ensure the following steps are completed:

### 1. MATLAB Installation
Make sure you have MATLAB installed on your computer. You can download it from the official [MathWorks website](https://www.mathworks.com/products/matlab.html).

### 2. Required Files - [AppFiles](../AppFiles/)
Ensure the following files are in the same directory or project folder within MATLAB:
- `SafetyAssessmentSoftware.mlapp`
- `UTp(tf).txt`
- `ZT(UTp).txt`
- `Test.txt`
- `Test2.txt`
- `Test3.txt`

### 3. Setting Up the Environment
- Launch MATLAB.
- Create a new project or working folder.
- Copy all the required files into the folder.
- Verify that MATLAB's **Current Folder** is set to the folder containing these files.
- `SafetyAssessmentSoftware.mlapp`
- Select from above the CENELEC option.

You are now ready to proceed with the steps specific to the CENELEC standard.

## How to Use
### Input Data

1. **(user input)** Time-current characteristic(s) of the protective device(s). You can use `Test.txt`, `Test2.txt`, `Test3.txt` for inputs here as an example.
2. **(user input)** Geometric proportionality factor, kg.
3. **(user input)** Touch voltage proportionality factor, kt.
4. **(user input)** Step voltage proportionality factor, ks.
5. Calculation of maximum allowable voltage limit according to CENELEC EN 50522. **Selection by the user, Yes or No:** Use of high resistivity surface material?
6. If yes: **(user input)** resistivity, ρs.
7. **(user input)** Resistance of footwear, RF1 (typical value 1000 Ω).
8. Curves from the IEC standard: (I) IB(tf), (II) ZT(UT). Code using `UTp(tf)_new.txt` and `ZT(UTp)_new.txt`. 
9. **(user input)** Heart current factor, HF, and body factor BF.
10. **(user input)** Maximum value of maximum grid current for the construction of the figures showing the safety performance curves. Input of the minimum value as well.

**Up to this point here: The safety performance curves can be plotted.
The above refer to a specific typical configuration.**

11. **Selection by the user** of the case to be evaluated: soil resistivity ρ (or ground resistance Rg).
12. **Selection by the user Yes or No:** Calculation of the maximum grid current IG according to IEEE Std 80?
13. If no: **(user input)** maximum grid current, IG.
14. If yes: **(user input)** symmetrical ground fault current fault current, If, division factor, Sf, and decrement factor, Df.
15.  **Selection by the user Yes or No:** Calculation of the decrement factor Df according to IEEE Std 80?
16. If no: **(user input)** decrement factor, Df.
17. If yes: **(user input)** X/R ratio, fault duration, tf.

**The above refer to specific installations of the typical grounding configuration. 
There could be several of those in a system.**


### Output Data

1. Plotting of Time-Current characteristic(s) of the protective device(s) curve.

2. Plotting of the basic safety performance curves (IG-ρtouch curve) and (IG-Rg,touch curve).
   
3. Addition of point showing the corresponding case examined.

