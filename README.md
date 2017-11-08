# Viewing ClinVar & dbSNP Variants on 3D Protein Structures

## Introduction

iCn3D is an interactive WebGL-based 3D protein structure viewer that displays a given protein in 1D (amino acid sequence), 2D (interaction diagram), and 3D (rotating 3D model) simultaneously. Users can interact with a protein by, for example, highlighting several amino acid residues in the sequence view; the corresponding residues in the remaining views are automatically highlighted. Our goal in this hackathon is to enhance the functionality of iCn3D by importing annotations from other rich sources of information about proteins, such as dbSNP rs numbers, ClinVar assertions of pathogenicity, and known structural features such as ligand binding pockets, protein interaction surfaces, and other functional domains.

## What's the problem?

In order for annotations to be viewed in iCn3D they must be retrieved from databases (e.g., dbSNP and ClinVar) using Ajax calls. _(more needed here)_

## Why should we solve it?

Without the aid of a 3D protein structure viewer like iCn3D, researchers and clinicians may be limited in their attempts to evaluate a variant's role in causing disease by the information at their disposal, such as whether a particular amino acid change is a conservative one, or on various estimates of evolutionary conservation. If they could instead view variants in the context of a protein's biological 3D structure, they might gain a deeper understanding of how a variant is likely to affect the protein, and thus better understand the mechanism by which it may cause disease. This could in turn lead to an ability to make more informed choices in asking research questions, and even in making more appropriate treatment choices for patients.

## Method:

dbSNP developers provided us access to a [cgi](https://www.ncbi.nlm.nih.gov/projects/SNP/beVarSearch.cgi?appname=iCn3D&format=bed&report=pdb2bed&gi=809237) that retrieves ClinVar and dbSNP data for annotations. _(more needed here)_

## Test Page:

A test page can be viewed [here](https://test.ncbi.nlm.nih.gov/Structure/icn3d2/seq.html?id=809237l). Novel annotations resulting from the achievements of this hackathon are shown at the bottom of the page. Users can highlight desired SNP residues or domains on the 3D protein structure simply by selecting the corresponding amino acids in the sequence pane. _(more needed here)_

