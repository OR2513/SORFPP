# SORFPP
Background: Genome sequencing has enabled us to find functional peptides encoded by short open read frames (sORFs) in long non-coding RNAs (lncRNAs). sORFs encoded peptides (SEPs) differ from conventional peptides because they play roles in various cellular processes, including gene expression and signaling regulation. Therefore, it is necessary to build a computational method to predict sORFs encoded peptides in a high-throughput way.
Results: In this paper, we propose a computational framework, SORFPP, for predicting SEPs by mining feature information from multiple perspectives using an experimentally validated dataset constructed by TranLnc. SORFPP utilizes a method that combines traditional encoding with the protein language model ESM to fully extract the sequence information of SEPs. SORFPP addresses the sparsity issue of traditional encoding methods using the CatBoost model. Moreover, SORFPP processes the attention maps extracted during the pre-training process of the ESM model with the Self-attention model. Finally, an ensemble learning framework is used to combine the results of the two models and input them into Logistic Regression to obtain accurate and stable prediction outcomes. Compared with other state-of-the-art models, SORFPP gets a higher Matthew correlation coefficient with an improvement of 12.2%-24.2% on three benchmark datasets.
Conclusion: Experimental comparisons demonstrate that SORFPP shows superior performance on the TransLnc dataset, surpassing the ESM model's capability to fully extract the sequence information of SEPs. Additionally, utilizing an ensemble learning framework to integrate the results of foundational models helps improve prediction outcomes. Experiments demonstrate that SORFPP is a reliable method for identifying whether SEPs are active.