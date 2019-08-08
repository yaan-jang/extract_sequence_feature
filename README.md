# Extract sequence feature
Extract position-specific scoring matrix, secondary structure, solvent-accessible surface, psi, and psi from protein sequence.

#### Get the source code
```
git clone https://yaan-jang@bitbucket.org/yaan-jang/extract_sequence_feature.git
```

##### Build 
```
mkdir build
cd build && cd build
cmake ../src
make
```


#### How to use
First of all, extract the [psipred-4.0.2.tar.gz] and [ncbi-blast-2.7.1+.tar.gz] into the directory lib. Then download the BLAST database [nr] at ftp://ftp.ncbi.nlm.nih.gov/blast/db/.

```
leri_extract -i list_protein -o output -f 1 -w 2 -t train
```
where **-i** is the list file of proteins, **-t** is an indicator of creating trainning data, **-f** is for downloading PDB files or not, **-w** is window size, and **-o** is to output the results in the directory. 



