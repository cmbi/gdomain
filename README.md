# A tool for identifiying the G-domain in PDB files that contain MHC.

## dependencies
 - pymol==3.0.0
 - biopython==1.84

## running the script

The script has its own reference pdb file. You only have to provide the unknown pdb file.

```
scripts/find_gdomain pdb_path_1 pdb_path_2 ...
```

gives output:

```
pdb_path_1 M 2-180
pdb_path_2 A 1-179
...
```

Each row corresponds to an unknown PDB file.
The rows are whitespace separated, the first column indicates filename, the second column indicates chain ids, the third column indicates residue numbers.
