# DigDEGs

DigDEGs is a SeqGeq plug-in for **paired pseudobulk differential expression** between two cell populations. It aggregates RNA counts for each biological replicate and population, then compares the populations across matched replicates such as independent donors.

For data preparation, clustering, visualization, and gene-set scoring in SeqGeq, see the companion [SeuratEM repository](https://github.com/MJMJ666/SeuratEM).

## Install

1. Install SeqGeq and R. Set the plug-ins folder and R location in SeqGeq’s Diagnostics preferences, then install the R packages listed in `DigDEGs_Practical_User_Manual_v1.5.docx`.
2. Place `DigDEGs_v0.5_build15.jar` in your configured SeqGeq plug-ins folder. Keep one installed DigDEGs JAR at a time and store ZIP archives and development folders elsewhere.
3. Restart SeqGeq and open DigDEGs from the **Plugins** menu.

## Run a comparison

1. Select **Population A** and **Population B** from the same SeqGeq data object.
2. Choose the RNA features and a biological replicate parameter, such as donor ID. Review the pairing preflight and confirm which replicates are represented in both populations.
3. Enter descriptive labels for the MDS plot and heatmap. The replicate parameter defines the pairing.
4. Review the result tables, plots, and diagnostic report. Positive log2 fold changes and **Up** indicate higher expression in Population A.

## Documentation and support

- The **DigDEGs Practical User Manual** covers setup, the pairing checks, results files, and saved comparisons.
- The **DigDEGs User Support Handoff** is the starting point for troubleshooting. Include the plug-in version, the comparison step, any exact error message, and the diagnostic report or relevant logs from the results folder.
- The **DigDEGs Source Handoff** contains implementation and build materials for developers.
