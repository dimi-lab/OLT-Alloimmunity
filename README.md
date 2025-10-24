# Processed data storage for "Spatial multiomics of human hepatic lymph nodes reveals early APC bifurcation in liver transplant rejection"
<img width="728" height="518" alt="image" src="https://github.com/user-attachments/assets/5e7aebc3-1248-46cf-a908-45d8a360491c" />

## 📂 Contents

### 🧬 Multiplexed Immunofluorescence (mxIF)
Processed spatial protein expression data from multiplexed immunofluorescence (mxIF) imaging.  
These datasets contain quantified marker intensities, cell-level segmentation results, and associated metadata.

**Files:**
- `OLT_mxIF_Non_Rejection.h5ad` — Processed mxIF data for non-rejection samples  
- `OLT_mxIF_Non_Non_Rejection.h5ad` — Processed mxIF data for non-non-rejection samples  

Format: `.h5ad` (AnnData), compatible with **Scanpy**, **Squidpy**, and related single-cell analysis tools.

---

### 🧫 Nanostring GeoMx Differential Gene Expression
Processed transcriptomic data derived from **Nanostring GeoMx DSP** analysis, representing spatially resolved gene expression profiles and differential expression results across three immune marker segments (**CD3**, **CD20**, and **CD68**). Each segment includes comparisons reflecting either **rejection vs. no rejection** status or **pre- vs. post-transplant** conditions within defined tissue ROIs. Data processed with DeSeq2.

**Files:**
- `cd20_hdln_post_rejection_vs_no_rejection.xls`
- `cd20_hdln_pre_rejection_vs_no_rejection.xls`
- `cd20_post_vs_pre_hdln.xls`
- `cd3_hdln_post_rejection_vs_no_rejection.xls`
- `cd3_hdln_pre_rejection_vs_no_rejection.xls`
- `cd3_post_vs_pre_hdln.xls`
- `cd68_hdln_post_rejection_vs_no_rejection.xls`
- `cd68_hdln_pre_rejection_vs_no_rejection.xls`
- `cd68_post_vs_pre_hdln.xls`

---

## ⚙️ File Access and Usage

Large data files are managed using **Git Large File Storage (LFS)**.  
To clone or pull this repository with data included:

```bash
git lfs install
git clone https://github.com/dimi-lab/OLT-Alloimmunity.git
