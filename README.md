# Designing A Biosensor for Small Molecules in Bacterial System  

## **Introduction**  
This project aims to develop a **vitamin B12 biosensor** by genetically modifying **E. coli DH5 Alpha** cells. The biosensor utilizes the **ethanolamine utilization pathway** (Eut pathway), which is regulated by vitamin B12 and ethanolamine. By introducing the eutR and peutS genes into the **PQE60-GFP plasmid**, we constructed a genetic circuit that responds to vitamin B12 by inducing GFP expression as a detectable signal.  

---

## **Aim**  
To design and create a vitamin B12 biosensor by cloning and genetically modifying an E. coli DH5 Alpha strain using the PQE60 GFP plasmid.  

---

## **Construct Design**  
The Eut pathway functions as follows:  
1. **EutR protein** acts as a transcription factor and forms a complex with **ethanolamine** and **vitamin B12**.  
2. This complex activates the **eutS gene**, which produces the EutS protein.  
3. By coupling this system with GFP (Green Fluorescent Protein) in the **PQE60 plasmid**, GFP expression serves as a reporter for vitamin B12 presence.  

### **Steps Involved**  
1. **Gene Selection**:  
   - Target genes: **eutR** and **peutS**.  
2. **Vector Selection**:  
   - Plasmid: Modified **PQE60-GFP** plasmid carrying GFP.  
3. **In-Silico Construct**:  
   - Constructed using **SnapGene** for primer design and gene insertion mapping.  

---

## **Materials and Methods**  

### **1. Gene Amplification via PCR**  
- Independent amplification of **eutR** and **peutS** genes.  
- PCR protocol included:  
   - Denaturation at 95°C, Annealing at 60°C, and Extension at 72°C.  
- **Cell Lysate PCR** was performed to amplify genes directly from E. coli DH5 Alpha genome.  

### **2. Vector Preparation (PQE60 GFP)**  
- Plasmid isolation involved alkaline lysis and ethanol precipitation steps.  
- Vector digestion using restriction enzymes **EcoRI** and **NcoI**.  

### **3. Ligation and Transformation**  
- Digested genes were ligated into the digested PQE60 GFP plasmid.  
- **CaCl₂-mediated transformation** of competent E. coli DH5 Alpha cells with recombinant plasmid.  
- Successful transformants were screened using **ampicillin resistance**.  

### **4. GFP Expression Induction (IPTG Protocol)**  
- **IPTG** was used to induce GFP expression in transformed E. coli cells.  
- IPTG concentrations tested: **0, 1 µM, 10 µM, 100 µM, 1 mM**.  
- GFP fluorescence was measured in two growth media:  
   - **Tryptone Broth (TB)**  
   - **M9 Minimal Media**  

---

## **Results**  

### **1. PCR Amplification**  
| **Sample**        | **Expected Size (bp)** | **Observed Size (bp)** |  
|--------------------|-----------------------|-----------------------|  
| Plasmid (PQE60)   | 3000                  | 3000                  |  
| eutR Gene         | 1053                  | ~1053                 |  
| peutS Gene        | 1500                  | ~1500 (with anomaly)  |  

### **2. IPTG Induction**  
Upon IPTG induction, GFP fluorescence increased significantly in TB media compared to M9 media:  

| **IPTG (µM)**     | **TB Media (Fluorescence)** | **M9 Media (Fluorescence)** |  
|--------------------|----------------------------|----------------------------|  
| 0                 | 943                        | 63                         |  
| 1                 | 4210                       | 876                        |  
| 1000              | Highest Recorded Value     | Lower Value                |  

**Observation**: GFP fluorescence was more prominent in TB media, highlighting the role of media composition in expression levels.  

### **3. Microscopy Results**  
- Fluorescence microscopy confirmed GFP expression in transformed E. coli cells.  
- Higher IPTG concentrations resulted in stronger GFP signals.  

---

## **Challenges and Troubleshooting**  
- Initial PCR for **peutS** showed unexpected band sizes due to mismatched primers designed using the wrong genome sequence.  
- Troubleshooting steps:  
   - Re-design primers.  
   - Validate amplification using appropriate conditions.  

---

## **Conclusion**  
This project successfully developed a vitamin B12 biosensor using genetically modified **E. coli DH5 Alpha**. The eutR and peutS genes were integrated into the PQE60 GFP plasmid, enabling GFP expression upon induction with IPTG. This demonstrates the feasibility of using the Eut pathway for small-molecule detection in bacterial systems.  

---

## **Future Directions**  
- Optimize sensor sensitivity for lower vitamin B12 concentrations.  
- Extend the biosensor design to detect other small molecules.  
- Use alternative reporter systems like RFP or enzymatic markers.  

---

## **Tools and Resources**  
- **Vector Design**: SnapGene  
- **PCR and Gene Amplification**: Thermal cycler, NCBI Primer-BLAST  
- **Plasmid Isolation**: Alkaline lysis protocol  
- **Transformation**: CaCl₂-mediated heat shock method  
- **Reporter Measurement**: Fluorescence microscopy  

---

## **References**  
1. **NCBI ORF Finder**: [https://www.ncbi.nlm.nih.gov/orffinder/](https://www.ncbi.nlm.nih.gov/orffinder/)  
2. **SnapGene Software**: [https://www.snapgene.com/](https://www.snapgene.com/)  
3. IPTG Induction Protocols  
