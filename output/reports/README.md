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

        wget ftp://ftp.flybase.net/genomes/Drosophila_melanogaster/current/gtf/dmel-all-r6.24.gtf.gz
         md5sum dmel-all-r6.24.gtf.gz
5cd5dcfbfff952ea7ce89e26cba89bbd  dmel-all-r6.24.gtf.gz
        
        gunzip dmel-all-r6.24.gtf.gz
        cut -f 1 dmel-all-r6.24.gtf | sort | uniq -c
  97461 2L
 110522 2R
 101180 3L
 126710 3R
   7839 4
    151 mitochondrion_genome
     67 rDNA
     43 Unmapped_Scaffold_8_D1580_D1567
  97543 X
    639 Y
