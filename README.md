# Semantic-Plagiarism-Detection-Agent

The Semantic Plagiarism Detection Agent is an AI-powered system designed to identify non-literal plagiarism, such as deep paraphrasing, structural reorganization, and idea theft, which conventional exact-match detectors routinely miss. Tailored for academic institutions, the system evaluates documents based on underlying contextual meaning rather than literal keyword overlap.Project OverviewStandard plagiarism checkers perform well on direct copy-pasting but fail against sophisticated rewriting tactics—which account for roughly 75% of academic integrity violations. This project solves that gap by combining dense vector embeddings with autonomous LLM reasoning to flag disguised borrowing, sentence repositioning, and voice shifts while preserving low false-positive rates for legitimate writing.Key Technical CapabilitiesContext-Aware Document Chunking: Parses unstructured documents (PDFs, DOCX, plain text) and splits them into overlapping semantic blocks to preserve context across boundaries.High-Dimensional Vector Embedding: Converts text chunks into mathematical embeddings, enabling rapid vector similarity searches across external databases and prior submissions.LLM-Powered Paraphrase Reasoning: Uses an intelligent agent to analyze suspect matches, evaluating complex structural edits like active/passive voice conversion and sentence repositioning.  Granular Source Mapping: Pinpoints local similarity zones, linking rewritten or restructured passages back to their precise origin in reference materials.Automated Diagnostic Reporting: Generates a full plagiarism report displaying an aggregated similarity percentage, side-by-side chunk comparisons, and source attribution.Architecture & Workflow[ Document Upload ] 
       │
       ▼
[ Preprocessing & Semantic Chunking ] 
       │
       ▼
[ Dense Vector Embedding ] ──► [ Vector Database Indexing ]
       │
       ▼
[ Cosine Similarity Filtering ] 
       │
       ▼
[ LLM Paraphrase Verification ] ──► (Filters out false positives & coincidental phrasing)
       │
       ▼
[ Diagnostic Report & Visual Mapping ]
