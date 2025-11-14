<h1>Manuscript:
  
# Reproductive biology of the monkfish Lophius gastrophysus in the southwestern Atlantic: histology, size at maturity, and fecundity #

<p>This R script performs a full reproductive-biology analysis to estimate size at sexual maturation (Ct₅₀) for male and female specimens using the King (1995) logistic model. It begins by importing and cleaning the dataset, standardizing ovarian-phase categories, and converting maturation status into a binary variable. The data are then split by sex, and a logistic regression (mature ~ Ct) is fitted separately for males and females. Using the regression coefficients, the script calculates the maturation steepness parameter r and the length at 50% maturity (Ct₅₀), and applies a bootstrap procedure to generate confidence intervals for both estimates as well as for the predicted ogive curve. Length-class groupings are created to compute observed proportions of mature individuals, which are later plotted alongside model predictions. The plotting function generates a four-panel figure showing maturation ogives and length-frequency distributions for each sex, including uncertainty bands and model parameters. Finally, the script exports high-resolution TIFF and PDF figures and saves a text summary of all statistical results, including Ct₅₀ estimates, confidence intervals, and sexual dimorphism metrics.<p>


<img width="2189" height="1364" alt="Figure_3" src="https://github.com/user-attachments/assets/a18447c2-e639-41c7-aca5-0a3f24f802b0" />
