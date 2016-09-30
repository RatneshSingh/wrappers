# wrappers
Few useful wrappers:
parralel_blast.pl : To run blast in parrallel. faster than -num_threads options in original blast.
```
-s sequencefile -db database  [options]
-p Program to run[blastn]
-n NumCpuToUse [20]
-o Outputfile[$fasta.blastn]
-of outputformat [0]
     0 = pairwise,
     1 = query-anchored showing identities,
     2 = query-anchored no identities,
     3 = flat query-anchored, show identities,
     4 = flat query-anchored, no identities,
     5 = XML Blast output,
     6 = tabular,
     7 = tabular with comment lines,
     8 = Text ASN.1,
     9 = Binary ASN.1,
    10 = Comma-separated values,
    11 = BLAST archive format (ASN.1)
    12 = JSON Seqalign output
-f directoryToSaveResults[blastn.tmp]
-a ExtraArgumentforBlastn. Dont put hyphens.eg. -a 'evalue 1e-10' -a 'culling_limit 1' etc..
-r do not remove temp folder
```
