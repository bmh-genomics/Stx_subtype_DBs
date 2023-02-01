# Stx_subtype_DBs
Databases for shiga toxin (stx) subtyping in fasta format containing representative stx2 subtype sequences (i.e. not all variants are included). NCBI accession numbers and other information used to generate the databases are in: database_accessions_and_info_20230110.txt

stx2_nt_subunitA-spacer-subunitB: An stx2 nucleotide sequence database that includes the full CDS of subunit A, a spacer region, and the full CDS of subunit B. Upstream/downstream sequences were removed as appropriate. 

stx2_aa_subunitA: An stx2 amino acid sequence database that includes the full CDS of subunit A.

stx2_aa_subunitB: An stx2 amino acid sequence database that includes the full CDS of subunit B.

stx2_aa_subunitA-B_joinedDB: An stx2 amino acid sequence database that includes the full CDS of subunit A joined to the full CDS of subunit B.

stx1_nt_JS_20230131.fasta: an stx1 nt dabase that includes subunit A and subunit B sequences as per database_accessions_and_info_20230110.txt

Note: for stx2m sequences, single-end iontorrent reads from strain E75_19 (BioSample # SAMEA7019263) were assembled and stx2m sequences identified as follows: 

1. Strain E75_19 assembly (performed by Julie Shay): Ion torrent reads (SRA ERX4245790) were assembled de novo using SPAdes v3.15.4 (--isolate and --iontorrent flags) after adapter removal with Sickle v1.33 (default SE parameters except for setting "qual-type" to "sanger") and quality trimming with Trimmomatic v0.39 (LEADING:25 TRAILING:25 MINLEN:50). The resulting draft genome was deposited into NCBI (GCA_025984515.1) and annotated with PGAP. 

2. stx2m sequences: stx2m nt sequence was identified by BLAST of the stx2a gene region (X07865.1) to the draft genome from stx2m strain E75_19 (performed by Julie Shay); stx2a subunit A and B sequences (CAA30714.1, CAA30715.1) were used to confirm the stx2m the start/stop and spacer region and derive stx2m nt and translated aa sequences (performed by Kelly Weedmark). Sequences were verified by Torsten Seeman. 
