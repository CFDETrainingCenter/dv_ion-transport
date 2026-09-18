# The Ion-Transport Landscape of Human Tissues

Every organ has a hidden current. Cells move ions (sodium, chloride, bicarbonate, protons) to support liver detoxification, pancreatic secretion, and intestinal absorption. Can spatial transcriptomics reveal how ion-transporter programs are organized across human tissues?

We used NIH Common Fund SenNet and HuBMAP data via the CFDE ecosystem: Xenium single-cell spatial transcriptomics from human liver (151,380 cells), pancreas (644,041 cells), and large intestine (24,293 cells), plus GeoMx whole-transcriptome profiling from zonated liver. Pancreas was subsampled to 200,000 cells for performance.

Ion-transporter genes were identified per dataset using UniProt and MyGene queries against ion-transport Gene Ontology terms and keywords (channels, pumps, cotransporters). For each cell, we computed an Ion-transport Expression Aggregate (IEA): a background-corrected, Seurat-style module score. IEA is a transcriptomic proxy for transporter-gene expression, not a measurement of ion flux.

The tool is an interactive HTML5/JavaScript canvas with tissue selection, guided-tour storytelling, zoom, pan, cell-type and IEA color modes, coherence-gated streamlines, and a GeoMx comparison view. Each point is a segmented cell at its true spatial coordinate. Cell groups reflect canonical transporter-marker expression, not reference-validated annotation.

Viewers learn that ion transport is spatially organized, not uniform. Liver shows zonated hepatocytes; pancreas reveals a CFTR-high ductal tree against acinar tissue; intestine shows a crypt-to-surface axis, with DRA/SLC26A3-high surface colonocytes opposite the crypt base. Streamlines trace where the expression rises (a gradient, not flux). The GeoMx arm applies the same screen to the whole transcriptome, recovering 46 ion genes versus a dozen on targeted panels, confirming a periportal-to-pericentral gradient (trend p=0.003).

**This project was submitted for the CFDE Training Center's Data Visualization Competition 2026.**
