    wget ftp://ftp.flybase.net/genomes/Drosophila_melanogaster/current/gtf/dana-all-chromosome-r1.06.gtf.gz
    gunzip dana-all-chromosome-r1.06.gtf.gz
    md5sum dana-all-chromosome-r1.06.fasta 
628e85bcaab158593acc3e74a5c43d29  dana-all-chromosome-r1.06.fasta
    
    faSize dana-all-chromosome-r1.06.fasta 
230993012 bases (17074195 N's 213918817 real 213918817 upper 0 lower) in 13749 sequences in 1 files
Total size: mean 16800.7 sd 387178.2 min 55 (scaffold_13714) max 23697760 (scaffold_13340) median 1517
N count: mean 1241.8 sd 9836.0
U count: mean 15558.9 sd 382128.9
L count: mean 0.0 sd 0.0
%0.00 masked total, %0.00 masked real

### I see the values here now. Seems like you did everything correct but did not download the correct assembly. You downloaded dana instead of dmel. Also please make sure you at least say where your readme file is for hw3. I kind of had to dig for this file. Other than that, good work.

        wget ftp://ftp.flybase.net/genomes/Drosophila_melanogaster/current/gtf/dmel-all-r6.24.gtf.gz
        md5sum dmel-all-r6.24.gtf.gz
5cd5dcfbfff952ea7ce89e26cba89bbd  dmel-all-r6.24.gtf.gz
       
      gunzip dmel-all-r6.24.gtf.gz
      grep -v "^#" dmel-all-r6.24.gtf | \cut -f3 | \sort | \uniq -c | \sort -rn
 187315 exon
 161014 CDS
  46339 5UTR
  33358 3UTR
  30591 start_codon
  30533 stop_codon
  30507 mRNA
  17772 gene
   2961 ncRNA
    485 miRNA
    334 pseudogene
    312 tRNA
    299 snoRNA
    262 pre_miRNA
    115 rRNA
     32 snRNA

        cut -f 1 dmel-all-r6.24.gtf | sort | uniq -c
  97461 2L
 110522 2R
 101180 3L
 126710 3R
   7839 4
  97543 X
    639 Y

    
    
