#Community Proteome Annotation: Identifying possible parent proteins and consolidating annotations

AEZ

2021 01 22

Summary
The purpose of these scripts recruit and consolidate peptide annotations from a protein sequence (or short read sequence) database by identifying all possible parent sequences for each peptide and retuning the top two most frequent values for either/both taxonomic and functional annotations. These scripts were developed for anlysis of community proteome samples from Station ALOHA.

NOTE: This is the most recent version.

Example data provided.

Above scripts executed the following:
1. Read and format peptide data
  i) PSM level output from MorpheusFromAnotherPlace or ProteomeDiscoverer
2. Get list of unique peptides
3. Use peptide list to recruit sequence IDs from protein fasta database
  i) Generate long table of unique peptide-protein matches
4. Import annotations for protein fasta database
5. Join annotations to peptide-protein table by sequence ID
6. Consolidate functional and taxonomic annotations by peptide to top two most frequent values among all possible parent proteins
7. Recruit complete lineage information for top1 and top2 taxa per peptide
8. Resolved ambiguous taxonomy my recruiting lineage for lowest common ancestor

