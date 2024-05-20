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

## Findings:

## 
