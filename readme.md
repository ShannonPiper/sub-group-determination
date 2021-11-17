#Subgroup Determination
##Blast
`for i in *.txt; do
name=`echo $i | awk -F "." '{print $1}'`
blastn -db nr -query $i -remote -out ${name}.out
done`
