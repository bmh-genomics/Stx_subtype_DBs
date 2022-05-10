# Stx_subtype_DBs
Databases for shiga toxin (stx) subtyping in fasta format. 

stx2_nt_subunitA-spacer-subunitB: An stx2 nucleotide sequence database that includes the full CDS of subunit A, a spacer region, and the full CDS of subunit B. Upstream/downstream sequences were removed as appropriate. 

stx2_aa_subunitA: An stx2 amino acid sequence database that includes the full CDS of subunit A.

stx2_aa_subunitB: An stx2 amino acid sequence database that includes the full CDS of subunit B.

stx2_aa_subunitA-B_joinedDB: An stx2 amino acid sequence database that includes the full CDS of subunit A joined to the full CDS of subunit B.

NCBI accession numbers and other information used to generate the databases are in the attached file: 

[database_accessions_and_info_20220510.txt](https://github.com/bmh-genomics/Stx_subtype_DBs/files/8663569/database_accessions_and_info_20220510.txt)

Note: for stx2m sequences, single-end iontorrent reads from strain E75_19 (BioSample # SAMEA7019263) were assembled and BLAST was used to identify the stx2m sequences based on X07865.1

Strain E75_19 assembly (performed by Julie Shay): Ion torrent reads (SRA ERX4245790) were assembled de novo using SPAdes v3.15.4 (--isolate and --iontorrent flags) 
after adapter removal with Sickle v1.33 (default SE parameters except for setting "qual-type" to "sanger") and quality trimming with Trimmomatic v0.39 (LEADING:25 TRAILING:25 MINLEN:50)

stxm sequences: stx2m nt sequence was identified by BLAST of the stx2a gene region (X07865.1) to the draft genome from stx2m strain E75_19 (performed by Julie Shay); stx2a subunit A and B sequences (CAA30714.1, CAA30715.1) were used to confirm the stx2m the start/stop and spacer region and derive stx2m nt and translated aa sequences (performed by Kelly Weedmark). 

