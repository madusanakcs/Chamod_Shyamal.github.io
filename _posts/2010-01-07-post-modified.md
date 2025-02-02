---
title: " High-Dimensional Volume and Concentration"
date: 2023-11-02T12:00:00-04:00
categories:
  - Blog
tags:
  - Post Formats
  - readability
  - standard
---





# **1. Volume of a $p$-Dimensional Unit Sphere**

### **Definition**
The $p$-dimensional unit sphere $\mathcal{S}_p$ is defined as

![image](https://github.com/user-attachments/assets/04bdacc8-279f-44d8-91e3-7033f07dc55c)


## **Volume Derivation**
The volume $V_{\mathcal{S}_p}$ is computed recursively using polar coordinates and the Beta function:
1. **Recursive Integral**

![image](https://github.com/user-attachments/assets/8d8fa7cb-65c1-443e-9b1a-cea1a608fcb5)

![image](https://github.com/user-attachments/assets/76e76da2-e4f3-4f65-8b6f-8285ea7180bd)


3. **Beta Function Substitution**:
   Using $t = x^2$, the integral becomes

![image](https://github.com/user-attachments/assets/d3200baf-a42f-4be9-aaf2-1a530cdcae86)


5. **Final Formula**


![image](https://github.com/user-attachments/assets/0a19c43f-85c6-45ad-99c8-d43e41f5793a)



# **2. Concentration of Volume Near the Equator**

![image](https://github.com/user-attachments/assets/c9c14e2e-50c3-4e36-91b3-91961194ed90)


## **Spherical Caps and Volume Ratio**
For a spherical cap at distance $\epsilon$ from the equator ($x_1 = 0$), the volume fraction is

![image](https://github.com/user-attachments/assets/bd709aac-d824-482a-9507-8355b35b6c34)


#### **Asymptotic Analysis**
For large $p$, approximate $\left(1 - x_1^2\right)^{\frac{p-1}{2}} \approx e^{-\frac{p-1}{2}x_1^2}$


![image](https://github.com/user-attachments/assets/655b9dce-b4e5-46ac-aa02-782a49ad0a6e)

![image](https://github.com/user-attachments/assets/0375aae1-586f-4e20-b448-283efad4cbbf)


### **Key Result**
For $\epsilon = \frac{c}{\sqrt{p-1}}$

![image](https://github.com/user-attachments/assets/c24e66cb-7150-4e6f-b184-3700256b68e1)

![image](https://github.com/user-attachments/assets/ebaa2c07-739a-4175-92b5-b215fafd4516)

![image](https://github.com/user-attachments/assets/f4949736-0990-4bcc-95ee-bcaa32d280c5)

![image](https://github.com/user-attachments/assets/a76110a5-5af9-4f59-b338-7f219cca76a0)


**Interpretation**: Over 90% of the volume lies within $\mathcal{O}\left(\frac{1}{\sqrt{p}}\right)$ of the equator in high dimensions.


# **3. Concentration in an Annulus at the Boundary**

![image](https://github.com/user-attachments/assets/497716e8-08bd-4bae-ae92-d69fa121c15c)


## **Volume of an Annulus**
The annulus $1 - \epsilon \leq \|\mathbf{x}\| \leq 1$ has volume

![image](https://github.com/user-attachments/assets/726a1753-de35-47ad-8cf0-4b9a1e141629)

## **Exponential Decay**
For small $\epsilon$, $(1 - \epsilon)^p \approx e^{-p\epsilon}$

![image](https://github.com/user-attachments/assets/06d08523-6b18-4ce8-8c69-cf8424415344)

**Interpretation**: For $\epsilon = \frac{c}{p}$, nearly all volume concentrates in a thin shell of thickness $\mathcal{O}\left(\frac{1}{p}\right)$.

![image](https://github.com/user-attachments/assets/46b4fac6-f9bc-4548-85e0-d1b1cb197b0d)






