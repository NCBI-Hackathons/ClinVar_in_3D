# DeleteriousMutants
Mapping Clinically Relevant Mutations to Protein Structures

## Goal:
To enhance iCn3D (new interactive version of Cn3D at NCBI) by annotating all 3D protein structures with dbSNP rs numbers and connected clinical data from ClinVar.

- iCn3D running with example
- Get data
-- Data Source
--- SNP ftp (rs => gi.snp)
ftp://ftp.ncbi.nlm.nih.gov/snp/organism/human_9606/database/data/organism_data/SNP3D.bcp.gz
(has cgi to get data)
--- ClinVar information - elink: SNP => ClinVar, rs => variant_id
