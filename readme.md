#Subgroup Determination

##Blast

`for i in *.txt; do
name=`echo $i | awk -F "." '{print $1}'`
blastn -db nr -query $i -remote -out ${name}.out
done`

Or blast using Geneious (although batch blast does not work)

##Alignment

1. Make reverse compliment of R2 sequences in geneious
2. Use geneious alignment to align forward and reverse reads with known 1A, 1B, and 1C samples
3. Use the following table to identify SNPs in each sample:

|Subgroup|125 bp|143 bp|162 bp|
|--------|------|------|------|
|1A|T|C|TT|
|1B|G|C|GC|
|1C|G|T|GC|



