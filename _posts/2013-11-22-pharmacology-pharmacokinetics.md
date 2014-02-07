---
layout: post
title:  "Pharmacokinetics"
date:   2013-11-22 7:37:58
categories: fundo2 exam3 pharmacology
---

### Pharmacokinetics Overview
- Pharmacokinetics is a quantitative approach to the behavior of drugs or chemicals in the body
- Mathematical models based on assumptions and evidence of the absorption and excretion are applied to predict drug disposition in the body
- Knowing the mathematical models allows you to follow drug disposition after administration
- Drugs may be modified within the organism into various states:

<span><br></span> 
1. **Compartmentalization** (movement from primary site to compartment)
2. **Metabolism** (chemical or enzymatic change to metabolite)
3. **Elimination** (appearance of drug or metabolite in elimination products, e.g., urine, feces, expired air)

<div style="text-align:center;" markdown="1">
![]({{site.baseurl}}/assets/state-change-diagram.png)
</div>

### One Compartment Open Model with Rapid IV Injection
- Simplest model of drug disposition, depicts body as one homogenous compartment with constant volume **V**
- **S<sub>0</sub>** is the dose of drug injected at time = 0.
- It is assumed there is instantaneous mixing throughout **V**
- **S** is the amount of drug remaining in the body at a given time t
- **C** is the concentration of drug in the body at a given time t, calculated by **C =  S/V**
- **k** is the first order rate constant of *elimination* of the drug from the body, has units time<sup>-1</sup>
- **S<sub>e</sub>** is the cumulative amount of drug excreted at any time
- Thus: **S = S<sub>0</sub>e<sup>-kt</sup>**
- Also: **C = C<sub>0</sub>e<sup>-kt</sup>**
- This formula allows you to calculate the expected amount of drug (**S**) at any time (t) when the initial dose (**S<sub>0</sub>**) and the rate constant for drug elimination (**k**) are known .
- Calculation of the initial dose based on amount excreted: **S<sub>e</sub> = S<sub>0</sub>\(1- e<sup>-kt</sup>\)**

<span><br></span> 
### Biological Half-Time
- **t<sub>1/2</sub>** is defined as the time required for **S** == 0.5 **S<sub>0</sub>**
- **t<sub>1/2</sub> = 0.693 / k**

<span><br></span>
### One Compartment Open Model with Constant Dose Rate
- Rate of change of the amount of drug on board given by **Rate of Change (dS/dt) = Rate of Input (A) - Rate of Output (E)**
- A constant franction (**f**) of a constant dose rate (**m**) is absorbed such that **A = fm**
- First-order excretion process (**E**) is proportional (**k**) to the instantaneous body burden (**S**) such that **E = kS**
- Thus, **dS/dt = fm - kS**
- Integrate: **S = fm/k\*\(1-e<sup>-kt</sup>\)**
- Note that at a rate of 2m, any given concentration will be reached faster; the steady state concentration will be double; but, the rate of equilibration will be the same.

<div style="text-align:center;" markdown="1">
![]({{site.baseurl}}/assets/plasma-concentration-during-constant-iv-infusion.png)
</div>

- Steady state \(**SS**\) may be defined as a time of no net change in **S**, thus input rate = output rate \(**A**=**E**\)
- At t = SS, e<sup>-kt</sup>=0; thus, **S<sub>SS</sub> = fm/k**
- And, if **f** and **k** are constant; **S<sub>SS</sub> ~ m**
- Thus, **\(S<sub>SS</sub> - S\) = S<sub>SS</sub>e<sup>-kt</sup>**

<span><br></span>
### Multiple Dose Case
- A common administration technique is to use multiple doses separated by some time interval
- This is analogous to the constant dose rate model, but the curve will be saw-tooth instead of smooth
- Constant dose rate **m** now expressed as individual doses **D** separated by time **t**, \(**D/t**\)
- **S<sub>SS</sub> = fD/kt**
- **S<sub>SS</sub><sup>max</sup> - S<sub>SS</sub><sup>min</sup> = Dose**
- Priming dose: give a larger dose than required initially in order to reach steady state concentration more rapidly

<div style="text-align:center;" markdown="1">
![]({{site.baseurl}}/assets/multiple-dose-model.png)
</div>
