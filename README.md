# human MDH2
# P40926
# Phosphorylation of S69


## Description

# The study by Eo et al. found that phosphorylation at position 69 in human mitochondrial malate dehydrogenase (hMDH2) significantly alters enzymatic activity and the structural conformation of the active site. While the study did not specifically examine the mutation of serine (S) to aspartate (D), existing literature suggests that this substitution mimics phosphorylation, potentially impacting substrate binding, catalytic efficiency, and protein interactions. The study also highlights the role of phosphate binding in stabilizing hMDH2’s active site, helping maintain enzymatic function. Although it does not provide detailed data on the serine (S) to aspartate (D) transition, it confirms that modifications like this affect the tricarboxylic acid (TCA) cycle and redox balance. Structural analysis reveals that phosphorylation at position 69 destabilizes the active site, altering enzymatic activity and substrate binding. These disruptions can interfere with metabolic regulation, potentially leading to dysfunction. Since position 69 is located near the dimer interface, phosphorylation could impact subunit interactions, affecting oligomerization and enzyme kinetics (Eo et al., 2022). Phosphate binding near the substrate site induces a closed conformation, ensuring efficient catalysis as well. A mutation at position 69 may alter substrate affinity, influencing enzyme function. This modification could also impact NAD/NADH binding, potentially disrupting redox balance and metabolic flux. 
For this specific variant, the unmodified structure of hMDH2 with serine (S) at position 69 has weak interactions with Ala 65, Ala 66, Asp 67, Leu 68, and His 70. The PTM modified structure where phosphate (SEP) replaced serine (S) at position 69 has weak interactions with Ala 65, Asp 67, Leu 68, His 70, and Arg 229. Lastly, the variant structure of aspartate (D) at position 69 has very similar weak interactions compared to the unmodified structure with Ala 65, Leu 68, His 70, and Val 77.

1. image of the unmodified site
![ The weak interactions of the unmodified structure of hMDH2 at position 69 with serine (S).](images/MDH2_normal.png)

2. image of modification site
![ The weak interactions of the modified structure of hMDH2 at position 69 with phosphate (SEP) replacing serine (S).](images/modified.png)
3. image of mimic site
![ The weak interactions of the PTM mimic structure of hMDH2 at position 69 with aspartate (D) replacing serine (S).](image/mimic.png)


## Effect of the sequence variant and PTM on MDH dynamics

# The mimic changed the function of the hMDH2 enzyme by influencing its electrostatic bonding, active site dynamics, and reaction kinetics. Molecular dynamic simulations were used to look at these changes in greater detail. The second Colab analysis looked at the Root Mean Square Fluctuation (RMSF) value of the mimic enzyme as seen in Figure 8. The unmodified enzyme has higher peaks throughout its graph indicating a greater flexibility or greater movement of the residues in unmodified hMDH2. The mimic enzyme has significantly lower peaks meaning that it is less flexible. This could indicate that the variant with aspartate instead of serine at position 69 causes the hMDH2 to become more ridged disrupting the enzyme. The mimic becomes more stable, meaning that metabolic pathways could be hindered. Metabolic pathways rely on the dynamic interactions between enzymes, so increasing rigidity can lead to an overflow of metabolites and energy imbalance throughout the pathway. 
The second Colab analysis also looked at pKa values between the unmodified enzyme and the mimic. Figure 9 shows the mimic enzyme which has a lower pKa value around position 69 indicating that aspartate increased the acidity compared to serine at position 69 of the unmodified hMDH2. Aspartate typically has a pKa around 3.9, which aligns with the observed values in the mimic plot compared to the unmodified plot. The increased acidity of position 69 can affect the local environment of the enzyme which can also affect the weak interactions the amino acids are able to create. This most likely happened with aspartate, and the lower pKa value as well as increasing acidity affected the weak interaction of aspartate compared to serine that has at a neutral pH (Hofer et al., 2020). 

1. Image of aligned PDB files (no solvent)
![The aligned model of the unmodified, modified, and mimic from mol* and alphafold3.](images/MDH2 alignment.png)

2. Image of the site with the aligned PDB files (no solvent)
![The aligned model of the unmodified, modified, and mimic from boltz-1 and alphafold3.](images/Boltz_mimic_modified_superimposed.png)

3. Annotated RMSF plot showing differences between the simulations
![ The molecular dynamics of hMDH2 described by the Root Mean Square Fluctuation (RMSF) value of the mimic enzyme  model from Colab 2. The red vertical line indicates the division of the two subunits of hMDH2, and the active site where the mimic is located is indicated by the green vertical line.](image/RSMF of mimic annotated.jpg)

4. Annotated plots of pKa for the key amino acids
![ The trend in pKa of amino acid Serine 69 from the unmodified hMDH2 (left) and the aspartate 69 mimic of hMDH2 (right).] (images/pKa_69_mimic.jpeg)



## Comparison of the mimic and the authentic PTM

# The model and simulation data on the mimic variant closely align with the PTM-modified protein, show many similarities. Both modifications alter the charge at position 69, impacting electrostatic interactions at the active site. Aspartate and phosphoserine’s negative charge affects weak interactions and nearby residues, particularly His 70, which is critical for enzyme function. Phosphoserine, with its bulky negative charge, disrupts the weak interactions around His 70, leading to a loss of function. Aspartate introduces a negatively charged carboxylate group, which influences weak interactions less by primarily affecting hydrogen bonding and causing minor shifts in catalytic efficiency rather than full impairment. The modified enzyme loses weak interactions with Ala 66, while the mimic enzyme shifts its interaction pattern to Val 77, suggesting structural rearrangement. Both modifications alter interactions with nearby residues, affecting the conversion of oxaloacetate to malate in the citric acid cycle and potentially impacting downstream metabolic pathways. Additionally, both disrupt interactions with Ala 66 and introduce new binding partners, Arg 229 in the modified enzyme and Val 77 in the mimic enzyme, altering local binding dynamics. These suggest that adding a negatively charged residue at position 69 stabilizes interactions to  impair metabolic function. The mimic variant’s rigidity, observed in RMSF analysis, supports the idea that charge modifications at position 69 influence protein flexibility. Since metabolic enzymes rely on controlled movement, this reduced flexibility suggests that both phosphoserine and aspartate substitutions could hinder normal enzymatic function.
There are also notable differences between phosphoserine modification and the aspartate mimic regarding their impact on enzyme structure and function. Phosphoserine significantly disrupts active site stability by altering electrostatic interactions with His 70, potentially leading to enzyme dysfunction, while aspartate maintains a weak interaction pattern like unmodified hMDH2, suggesting it does not drastically destabilize the active site. The phosphoserine modification causes major disruptions, whereas the aspartate variant primarily increases rigidity, reducing flexibility rather than fully destabilizing the enzyme. Additionally, phosphoserine creates stronger electrostatic repulsion near His 70, interfering with proton shuttling in the citric acid cycle, while aspartate affects the electrostatic environment but remains more structurally similar to the unmodified enzyme. The aspartate variant lowers the pKa at position 69, increasing acidity compared to serine, which influences enzymatic efficiency without complete impairment, while phosphoserine’s bulkier structure and stronger charge repulsion have a more drastic impact on active site configuration. Overall, phosphoserine is more disruptive, likely causing enzyme function loss, while the aspartate mimic primarily influences structural rigidity and minor functional shifts. These findings highlight how post-translational modifications and mimics can have varying effects, demonstrating their distinct biochemical impacts.
The mimic variant partially approximates the PTM-modified hMDH2, phosphoserine at position 69, capturing charge effects and electrostatic interactions with His 70. Both introduce a negative charge that  alters weak interactions, but phosphoserine destabilizes the active site due to its bulkier structure and stronger hydrogen bonding. While the mimic increases rigidity, it does not replicate flexibility loss. Further exploration of alternative mimics from a person with a PHD may better approximate PTM effects on hMDH2 function.

### Colab notebook links

Copy_of_Boltz_for_biochemv2.ipynb

Copy_of_MD_simulation_Step1v2.ipynb

Copy_of_MDanalysis_Step2.ipynb



## Authors

Elodie Walton
## Deposition Date

## License

Shield: [![CC BY-NC 4.0][cc-by-nc-shield]][cc-by-nc]

This work is licensed under a
[Creative Commons Attribution-NonCommercial 4.0 International License][cc-by-nc].

[![CC BY-NC 4.0][cc-by-nc-image]][cc-by-nc]

[cc-by-nc]: https://creativecommons.org/licenses/by-nc/4.0/
[cc-by-nc-image]: https://licensebuttons.net/l/by-nc/4.0/88x31.png
[cc-by-nc-shield]: https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg


## References

*1. Moro, J.; Tomé, D.; Schmidely, P.; Demersay, T.-C.; Azzout-Marniche, D. Histidine: A Systematic Review on Metabolism and Physiological Effects in Human and Different Animal Species. Nutrients 2020, 12 (5), 1414. https://doi.org/10.3390/nu12051414. ![ 10.3390/nu12051414]( https://doi.org/10.3390/nu12051414.)

*2. Eo, Y.; Duong, M. T. H.; Ahn, H.-C. Structural Comparison of hMDH2 Complexed with Natural Substrates and Cofactors: The Importance of Phosphate Binding for Active Conformation and Catalysis. Biomolecules 2022, 12 (9), 1175. https://doi.org/10.3390/biom12091175. ![ 10.3390/biom12091175]( https://doi.org/10.3390/biom12091175.)
