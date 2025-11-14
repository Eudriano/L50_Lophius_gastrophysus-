
 
</head>

<body>

<h1>Manuscript</h1>

<h2><em>Reproductive biology of the monkfish <i>Lophius gastrophysus</i> in the southwestern Atlantic: 
histology, size at maturity, and fecundity</em></h2>

<h3>Costa et al. (2025)</h3>

<p>
This R script performs a complete reproductive-biology analysis to estimate size at sexual 
maturation (Ct₅₀) for male and female <i>Lophius gastrophysus</i> using the logistic model of King (1995). 
The workflow includes dataset import, cleaning, standardization of ovarian-phase categories, and 
conversion of maturation status into a binary variable. The dataset is then separated by sex, and 
a logistic regression (<code>mature ~ Ct</code>) is fitted independently for males and females.
</p>

<p>
Using the estimated coefficients, the script computes the maturation steepness parameter <em>r</em> 
and the length at 50% sexual maturity (Ct₅₀). A bootstrap procedure is performed to produce 
confidence intervals for both parameters and for the predicted ogive curve. Length-class 
groupings are generated to obtain observed proportions of mature individuals, which are then 
plotted alongside the modeled predictions.
</p>

<p>
The plotting routine produces a four-panel figure showing (1) the maturity ogive and (2) length-frequency 
distribution for each sex. These plots include uncertainty bands, model parameters, and 
maturity-stage shading. Finally, the script exports high-resolution TIFF and PDF figures and saves 
a text summary of all statistical outputs, including Ct₅₀ estimates, confidence intervals, and 
metrics of sexual dimorphism.
</p>

<figure>
  <img 
    src="https://github.com/user-attachments/assets/a18447c2-e639-41c7-aca5-0a3f24f802b0" 
    alt="Figure 3: Maturity ogives and length distributions for Lophius gastrophysus" 
    width="100%">
  <figcaption>
    <strong>Figure 3.</strong> Length at first maturity (L₅₀) and size distribution for 
    <i>Lophius gastrophysus</i>.  
    <br>A — Maturity ogives for males;  
    B — Maturity ogives for females;  
    C — Length-frequency distribution of male maturity stages;  
    D — Length-frequency distribution of female maturity stages.  
    <br>In panels A and B, solid curves show the fitted logistic model and shaded bands 
    indicate 95% confidence intervals.  
    In panels C and D, light bars represent immature individuals, dark bars represent 
    mature individuals; the solid vertical line indicates L₅₀, and dashed vertical lines 
    represent the 95% CI bounds.
  </figcaption>
</figure>

</body>
</html>
