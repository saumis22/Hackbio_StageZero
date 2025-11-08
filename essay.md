## **What Single-Cell Data Is Teaching Us About Cancer Evolution**

## **Introduction**

Cancer is a dynamic evolutionary process driven by genetic mutations, clonal selection, and microenvironmental adaptation. Bulk transcriptomic analyses average gene expression across heterogeneous populations, concealing rare subclones with clinical significance (Lei et al., 2021). The tumor microenvironment (TME), including malignant cells, immune infiltrates, stromal components, and endothelial networks, further influences tumor progression, metastasis, and therapy resistance (Hanahan, 2022).

Single-cell RNA sequencing (scRNA-seq) profiles individual cellular transcriptomes, enabling resolution of cellular heterogeneity, reconstruction of lineage hierarchies, and identification of transcriptional plasticity underlying tumor evolution and therapy resistance (Li et al., 2021). This review summarizes scRNA-seq principles, experimental workflows, and key applications, highlighting insights into intratumoral heterogeneity, circulating tumor cells (CTCs), cancer stem cells (CSCs), TME interactions, and translational findings across cancer types.

This study examines how single-cell data has transformed our understanding of cancer evolution by linking scRNA-seq analyses to tumor heterogeneity and mechanisms of therapy resistance.

## **Understanding Cancer as an Evolutionary Process**

Cancer progression mirrors Darwinian evolution, where selective pressures such as hypoxia, immune surveillance, and therapeutic stress drive clonal diversification (Greaves & Maley, 2012). Single-cell studies show that genetic and transcriptomic variability among tumor cells underpins adaptability and survival under treatment stress (Davis et al., 2020). By resolving cellular hierarchies and differentiation trajectories, scRNA-seq enables tracing of clonal evolution and elucidation of how microenvironmental cues shape selection dynamics (Huang et al., 2023).

![Diagram1](https://github.com/LuciaUchegbu/Hackbio_StageZero/raw/main/Diagram%201.png)

Figure 1:  Tumor evolution and intratumor heterogeneity. Adapted from Sabaawy (2013).

## **Principles of scRNA-seq**

scRNA-seq captures RNA transcripts from individual cells, converts them into complementary DNA (cDNA), amplifies, sequences, and quantifies expression. The number of reads per gene reflects its expression level, providing a digital measurement of transcript abundance (Tang et al., 2009). Because single cells contain minimal RNA, sensitive amplification techniques are critical to ensure coverage without introducing bias (Haque et al., 2017). Modern protocols, such as Smart-seq2 and droplet-based 10x Genomics systems, balance sequencing depth and throughput, enabling large-scale tumor profiling with single-cell precision.

## **Experimental Workflow of scRNA-seq Techniques**

The standard scRNA-seq workflow includes sample preparation, cell isolation, reverse transcription, amplification, library preparation, sequencing, and data analysis. Sample dissociation is critical; dense tumor tissues require enzymatic digestion (e.g., collagenase, trypsin) and mild agitation to avoid excessive lysis (Li et al., 2021). Single-cell capture can be performed through limiting dilution, micromanipulation, fluorescence-activated cell sorting (FACS), or microfluidic droplet systems. FACS remains the preferred method for balancing purity and throughput, while droplet-based platforms enable parallel analysis of thousands of cells (Haque et al., 2017).

Subsequent bioinformatics pipelines include quality control, normalization, clustering, differential expression, and trajectory inference to explore cellular heterogeneity and lineage relationships. Challenges such as dropout events and batch effects are addressed using computational corrections (Stuart et al., 2019).

![Diagram2](https://github.com/LuciaUchegbu/Hackbio_StageZero/blob/main/Diagram%202.png)

Figure 2: Workflow of single-cell RNA sequencing (scRNA-seq) techniques (Tang et al., 2009).

## **Applications of scRNA-seq in Cancer Research and Treatment**

**Intratumoral Heterogeneity**

Tumor heterogeneity, both inter- and intratumoral, drives metastasis and therapy resistance (Xu et al., 2021). scRNA-seq has revealed prognostically distinct subpopulations in hepatocellular and pancreatic cancers, highlighting aggressive clusters that influence disease progression and patient outcomes (Xie et al., 2022; Peng et al., 2019).

**Circulating Tumor Cells (CTCs)**

CTCs are rare intermediates in metastasis. scRNA-seq enables profiling of individual CTCs, uncovering gene programs that promote survival, immune evasion, and distant colonization. For example, EMT and stemness pathways in breast cancer CTCs correlate with poor prognosis (Chen et al., 2023; Zhao et al., 2023).

**Cancer Stem Cells (CSCs)**

CSCs are pivotal for tumor maintenance and therapy resistance. scRNA-seq has revealed transcriptional plasticity and metabolic heterogeneity among CSCs, linking lineage trajectories to recurrence and aggressiveness in glioblastoma and HCC (Nguyen et al., 2022; Cancer Cell International, 2024).

**Tumor Microenvironment (TME)**

The TME shapes tumor progression and therapy response. scRNA-seq, often combined with spatial transcriptomics, maps immune and stromal cell heterogeneity, identifying immunosuppressive states and angiogenic niches (Lei et al., 2021; Zhao et al., 2023; Song et al., 2025). This integration highlights interactions between cancer, immune, and stromal cells that drive heterogeneity and therapeutic outcomes.

## **Translational Insights Across Cancer Types**

scRNA-seq has profoundly advanced our understanding of tumor heterogeneity and therapeutic resistance across cancers, revealing transcriptional subpopulations that drive relapse, metastasis, and drug resistance.

- **Breast Cancer:** Subclonal populations with differential expression of EMT and stemness-associated genes reveal mechanisms behind metastatic spread and chemoresistance (Kim et al., 2022).  

- **Lung Cancer:** Resistant cell states persist following EGFR inhibitor therapy, highlighting non-genetic adaptive mechanisms (Maynard et al., 2020; Li et al., 2021).  

- **Hepatocellular Carcinoma (HCC):** Malignant and immune subclusters correlate with prognosis, immune evasion, and spatial organization within the TME (Zhang et al., 2022).  

- **PDAC:** Integration with spatial transcriptomics uncovers stromal-tumor interactions promoting aggressive phenotypes and chemotherapy resistance (Moncada et al., 2020).  

- **Melanoma:** Resistant subpopulations pre-exist before therapy; transcriptional plasticity drives treatment escape rather than de novo mutations (Rambow et al., 2018).  

- **Colorectal Cancer:** Prognostic models link specific subpopulations to patient outcomes, including survival, disease recurrence, and therapy response (Song et al., 2025).

## **Integration with Other Single-Cell Methods**

 scRNA-seq captures transcriptomes but lacks direct protein-level or post-translational information. Integration with mass cytometry (CyTOF) enables high-dimensional single-cell protein profiling (Li et al., 2021). Imaging mass cytometry (IMC) preserves spatial context, mapping multiple protein markers across tissues. Spatial transcriptomics and in situ sequencing (ISS) bridge gene expression and spatial organization (Gyllborg et al., 2020; Asp et al., 2019). Moncada et al. (2020) demonstrated the synergy of scRNA-seq and spatial transcriptomics in pancreatic tumors, revealing co-enriched cancer, immune, and stromal networks

## **Challenges and Emerging Barriers**

Despite progress, scRNA-seq faces several challenges:

- **Technical limitations:** Dissociation bias, low RNA capture efficiency, and dropout events can distort cell representation (Huang et al., 2023).  

- **Data integration challenges:** Multi-omic and spatial datasets require advanced computational pipelines (Stuart et al., 2019).  

- **Cost and scalability:** High sequencing costs limit clinical translation and large-cohort studies (Yan et al., 2022).  

- **Standardization gaps:** Lack of unified analytical standards hampers reproducibility and cross-study comparisons (Lei et al., 2021).

## **Future Perspectives and Conclusion**

## To translate scRNA-seq discoveries into precision oncology, priorities include

- Developing standardized, cost-effective workflows for clinical labs.  

- Integrating longitudinal multi-omic datasets to track clonal evolution during therapy.  

- Validating single-cell biomarkers in multicenter clinical trials.  

- Expanding AI-driven computational tools for spatial and temporal modeling of tumor dynamics.

scRNA-seq has transformed understanding of cancer evolution by resolving cellular heterogeneity, tracing clonal hierarchies, and uncovering resistance mechanisms. Its integration with proteomic, spatial, and epigenomic data is shifting oncology toward personalized, adaptive therapies. Cross-disciplinary innovation in technology, computation, and clinical validation is essential to translate these insights from bench to bedside.




## **References**

Asp, M., Giacomello, S., Larsson, L., Wu, C., Fürth, D., Qian, X., ... & Lundeberg, J. (2019). _A spatiotemporal organ-wide gene expression and cell atlas of the developing human heart._ _Cell, 179_(7), 1647-1660.e19. <https://doi.org/10.1016/j.cell.2019.11.025>

Cancer Cell International. (2024). _Single-cell RNA sequencing reveals the landscape of the cellular ecosystem of primary hepatocellular carcinoma._ _Cancer Cell International, 24_(379). <https://doi.org/10.1186/s12935-024-03574-0>

Chen, Z., Huang, A., Sun, J., Jiang, T., Qin, F. X., & Huang, G. (2023). _Single-cell RNA sequencing in cancer research: Advances and applications._ _Frontiers in Oncology, 13_, 1123456. <https://doi.org/10.3389/fonc.2023.1123456>

Davis, R. T., Blake, K., Ma, D., Gabra, M. B. I., Hernandez, G. A., Phung, A. T., ... & Ewald, A. J. (2020). Transcriptional diversity and bioenergetic shift in human breast cancer metastasis revealed by single-cell RNA sequencing. _Nature Cell Biology, 22_(3), 310-320. <https://doi.org/10.1038/s41556-020-0477-0>

Greaves, M., & Maley, C. C. (2012). _Clonal evolution in cancer._ _Nature, 481_(7381), 306-313. <https://doi.org/10.1038/nature10762>

Haque, A., Engel, J., Teichmann, S. A., & Lönnberg, T. (2017). _A practical guide to single-cell RNA-sequencing for biomedical research and clinical applications._ _Genome Medicine, 9_(1), 75. <https://doi.org/10.1186/s13073-017-0467-4>

Hanahan, D. (2022). _Hallmarks of cancer: New dimensions._ _Cancer Discovery, 12_(1), 31-46. <https://doi.org/10.1158/2159-8290.CD-21-1059>

Huang, D., Ma, N., Li, X., Gou, Y., Duan, Y., Liu, B., ... & Zhang, X. (2023). _Advances in single-cell RNA sequencing and its applications in cancer research._ _Journal of Hematology & Oncology, 16_(98). <https://doi.org/10.1186/s13045-023-01494-6>

Journal of Biomedical Science. (2022). Spatial mapping of cancer-associated fibroblast heterogeneity in solid tumors. _Journal of Biomedical Science, 29_(115). <https://doi.org/10.1186/s12929-022-00893-1>

Kim, C., Gao, R., Sei, E., Brandt, R., Hartman, J., Hatschek, T., … & Navin, N. E. (2022). Chemoresistance evolution in triple-negative breast cancer delineated by single-cell sequencing. _Cell_, 185(3), 556-573.e18. <https://doi.org/10.1016/j.cell.2021.12.015>

Lei, Y., Tang, R., Xu, J., Wang, W., Zhang, B., Liu, J., ... & Yang, C. (2021). Applications of single-cell sequencing in cancer research: Progress and perspectives. _Human Cell, 34_(5), 1276-1295. <https://doi.org/10.1007/s13577-021-00583-2>

Li, X., Li, C., Jin, H., & Zhang, T. (2021). _Single-cell RNA sequencing in cancer: Applications, advances, and emerging challenges._ _Molecular Therapy - Oncolytics, 21_, 183-200. <https://doi.org/10.1016/j.omto.2021.04.006>

Maynard, A., McCoach, C. E., Rotow, J. K., Harris, L., Haderk, F., Kerr, D. L., … & Doebele, R. C. (2020). Therapy-induced evolution of human lung cancer revealed by single-cell RNA sequencing. _Cell_, 182(5), 1232-1251.e22. <https://doi.org/10.1016/j.cell.2020.07.017>

Moncada, R., Barkley, D., Wagner, F., Chiodin, M., Devlin, J. C., Baron, M., … & Regev, A. (2020). Integrating microarray-based spatial transcriptomics and single-cell RNA-seq reveals tissue architecture in pancreatic ductal adenocarcinomas. _Nature Biotechnology_, 38(3), 333-342. <https://doi.org/10.1038/s41587-019-0392-8>

Nguyen, Q. H., Pervolarakis, N., Nee, K., & Kessenbrock, K. (2022). Experimental approaches for defining tumor ecosystems using single-cell and spatial technologies. _Cancer Cell, 40_(6), 606-620. <https://doi.org/10.1016/j.ccell.2022.04.013>

Peng, J., Sun, B. F., Chen, C. Y., Zhou, J. Y., Chen, Y. S., Chen, H., ... & Yang, Y. G. (2019). Single-cell RNA-seq highlights intra-tumoral heterogeneity and malignant progression in pancreatic ductal adenocarcinoma. _Cell Research, 29_(9), 725-738. <https://doi.org/10.1038/s41422-019-0195-y>

Rambow, F., Marine, J. C., & Goding, C. R. (2018). Melanoma plasticity and phenotypic diversity: therapeutic barriers and opportunities. _Genes & Development_, 33(19-20), 1295-1318. <https://doi.org/10.1101/gad.329771.119>

Sabaawy, H. (2013). A simplified diagram displaying the different tumor evolution processes under review. In _Genetic heterogeneity and clonal evolution of tumor cells and their impact on precision cancer medicine_. _Journal of Leukemia_, 1(4), 1000124. CC BY 2.0.[https://www.researchgate.net/figure/A‑simplified‑diagram‑displaying‑the‑different‑tumor‑evolution‑processes‑under‑review_fig1_260372563](https://www.researchgate.net/figure/A%E2%80%91simplified%E2%80%91diagram%E2%80%91displaying%E2%80%91the%E2%80%91different%E2%80%91tumor%E2%80%91evolution%E2%80%91processes%E2%80%91under%E2%80%91review_fig1_260372563)

Song, W., Wang, Y., Zhou, M., Li, X., Liu, J., Qian, Z., ... & Liu, X. (2025). _Spatial transcriptomics and scRNA-seq: Decoding tumor complexity and constructing prognostic models in colorectal cancer._ _Human Genomics, 19_(92). <https://doi.org/10.1186/s40246-025-00805-x>

Stuart, T., Butler, A., Hoffman, P., Hafemeister, C., Papalexi, E., Mauck, W. M., ... & Satija, R. (2019). _Comprehensive integration of single-cell data._ _Cell, 177_(7), 1888-1902. <https://doi.org/10.1016/j.cell.2019.05.031>

Tang, F., Barbacioru, C., Wang, Y., Nordman, E., Lee, C., Xu, N., ... & Surani, M. A. (2009). mRNA-Seq whole-transcriptome analysis of a single cell. _Nature Methods, 6_(5), 377-382. <https://doi.org/10.1038/nmeth.1315>

Xie, Y., Yin, T., Wiegand, C., Lin, C., & Chen, J. (2022). Single-cell RNA-seq identifies novel cell populations in hepatocellular carcinoma with prognostic significance. _Frontiers in Oncology, 12_, 911048. <https://doi.org/10.3389/fonc.2022.911048>

Xu, J., Zhang, C., & Xie, H. (2021). Single-cell RNA sequencing reveals intratumoral heterogeneity in hepatocellular carcinoma. _Cancer Cell International, 21_(379). <https://doi.org/10.1186/s12935-021-02067-8>

Yan, C., et al. (2022). _Single-cell analysis reveals metabolic plasticity driving melanoma resistance to BRAF inhibition._ Nature Communications, 13(1), 4785. <https://doi.org/10.1038/s41467-022-32454-4>

Zhang, Q., He, Y., Luo, N., Patel, S. J., Han, Y., Gao, R., … & Zhang, Z. (2022). Landscape and dynamics of single immune cells in hepatocellular carcinoma. _Cell_, 185(1), 101-119.e25. <https://doi.org/10.1016/j.cell.2021.12.012>

Zhao, J., Shi, Y., & Cao, G. (2023). _The application of single-cell RNA sequencing in the inflammatory tumor microenvironment._ _Biomolecules, 13_(344**). [](https://doi.org/10.3390/biom13020344)** <https://doi.org/10.3390/biom13020344>
