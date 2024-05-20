# MyGenome
CS485 - Kevin J. Ramirez

## Research Questions

A new diversal fungal genus identified as Pyricularia Oryzae has found itself into Lexington, bringing along consequential diseases such as wheat blast, affecting crop life. The following research questions are posed for this project:

1. Where did this new disease originate from?
2. How did wheat blast and other similar fungal diseases (grey leaf spot) accumulate so much diversity in so little time?

## Sequence Trimming:

The F1 and R1 sequence datasets were analyzed using FastQC:

```$env:DISPLAY = 'localhost:0'
ssh -Y ukyID@ukyID.cs.uky.edu
cd rnaseq
fastqc &
```

Below are the forward sequence quality and adaptor reads:

![ForwardReadQuality.PNG](/data/ForwardReadQuality.PNG)
![ForwardReadAdaptor.PNG](/data/ForwardReadAdaptor.PNG)

Below are the reverse sequence quality and adaptor reads:

![ReverseReadQuality.PNG](/data/ReverseReadQuality.PNG)
![ReverseReadAdaptor.PNG](/data/ReverseReadAdaptor.PNG)

The following line of code was used to trim the sequences down after the previous findings (Do not include the slashes at the end of each line):

``` java -jar ~/sequences/trimmomatic-0.38.jar /
PE -threads 2 -phred33 -trimlog /
UFVPY657_errorlog.txt A24/A24_CKDL230042317-1A_HGC52DSX7_L2_1.fq.gz /
A24/A24_CKDL230042317-1A_HGC52DSX7_L2_2.fq.gz UFVPY657_1_paired.fastq UFVPY657_1_unpaired.fastq /
UFVPY657_2_paired.fastq UFVPY657_2_unpaired.fastq /
ILLUMINACLIP:adaptors.fasta:2:30:10 SLIDINGWINDOW:20:20 MINLEN:100
```

## Findings:

## 
