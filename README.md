# DeleteriousMutants

## Intro statement

iCn3D is an interactive protein viewer with which users can highlight desired amino acids or domain features on a 3D protein structure simply by highlighting the corresponding amino acids in the sequence pane. If variants in dbSNP and ClinVar could be linked to proteins in iCn3D, they could be viewed directly on the 3D protein structure. We propose See How Variants End In Traits (SHoVEIT), which enables the retrieval and display of known dbSNP and ClinVar annotations for all PDB proteins with viewable structures in iCn3D.

## What's the problem?

iCn3D users currently cannot see where known variants, including those that are clinically relevant, are located within visible protein structures.

## Why should we solve it?

iCn3D is would be exponentially more awesome and useful if it could display annotations of known variants, particularly those with known clinical relevance. If we add these annotations, iCn3D users could ask (and answer) biological questions and potentially learn how certain variants cause disease, based on their effects on protein function.

# What is SHoVEIT?
(ideas: ClinProt, ClinProtView, SeeHowVariantsEndInTraits - SHoVEIT)

Overview Diagram

# How to use ShoVEIT

## Installation options:

We provide two options for installing <this software>: Docker or directly from Github.

### Docker

The Docker image contains <this software> as well as a webserver and FTP server in case you want to deploy the FTP server. It does also contain a web server for testing the <this software> main website (but should only be used for debug purposes).

1. `docker pull ncbihackathons/<this software>` command to pull the image from the DockerHub
2. `docker run ncbihackathons/<this software>` Run the docker image from the master shell script
3. Edit the configuration files as below

### Installing <this software> from Github

1. `git clone https://github.com/NCBI-Hackathons/<this software>.git`
2. Edit the configuration files as below
3. `sh server/<this software>.sh` to test
4. Add cron job as required (to execute <this software>.sh script)

### Configuration

```Examples here```

# Testing

We tested four different tools with <this software>. They can be found in [server/tools/](server/tools/) . 

# Additional Functionality

### DockerFile

<this software> comes with a Dockerfile which can be used to build the Docker image.

  1. `git clone https://github.com/NCBI-Hackathons/<this software>.git`
  2. `cd server`
  3. `docker build --rm -t <this software>/<this software> .`
  4. `docker run -t -i <this software>/<this software>`
  
### Website

There is also a Docker image for hosting the main website. This should only be used for debug purposes.

  1. `git clone https://github.com/NCBI-Hackathons/<this software>.git`
  2. `cd Website`
  3. `docker build --rm -t <this software>/website .`
  4. `docker run -t -i <this software>/website`
  
  
  
  # Old text:

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
