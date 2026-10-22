# bioinformatics-portfolio
Bioinformatics coursework portfolio - William Gottschalk
William Gottschalk
BIOL 2406 — Introduction to Bioinformatics
Fall 2026

This repository documents the bioinformatics skills I developed during my
introductory bioinformatics course, including:

- Unix command line navigation and cluster computing
- Quality control and trimming of sequencing data
- Read alignment and mapping
- Differential gene expression analysis
- Phylogenetic analysis


Each folder corresponds to a unit of the course and contains scripts,
summary results, and documentation of the methods used.


Explore Module

The purpose of this work to showcase the work completed in the four Explore modules working on the Northeastern HPC

Module 1:  /courses/BIOL2406.202710/students/gottschalk.w/bioinformatics-portfolio/Explore_module_01
        This file contains the code of the tasks from the 1_Genomes_tutorial.md module on github along with # comments, most work was done locally,
Module 2:  /courses/BIOL2406.202710/students/gottschalk.w/bioinformatics-portfolio/Explore_module_02
        This file contains the code of the tasks from the 2_bowtie2_tutorial.md module on github along with # comments, work was done on the Northeastern HPC
Module 3:  /courses/BIOL2406.202710/students/gottschalk.w/bioinformatics-portfolio/Explore_module_03
        This file contains the code and results from the 3_Variants_tutorial.md module on github along with # comments, work was done on the Northeastern HPC
Module 4: /courses/BIOL2406.202710/students/gottschalk.w/bioinformatics-portfolio/Explore_module_04
	This file contains the code and results from the 4_Mapping_tutorial.md module on github along with # comments, work was done on the Northeastern HPC	
Across all files extraneous lines of directories and sequences were deleted.

In the Northeastern HPC bash commands were used with the following

GNU bash, version 5.1.8(1)-release (x86_64-redhat-linux-gnu)
Copyright (C) 2020 Free Software Foundation, Inc.
License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>

This is free software; you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.

Module Credits

bowtie2 module

/shared/EL9/explorer/modulefiles/bowtie2/2.5.4:

module-whatis   {Loads bowtie2/2.5.4 module.

This module was built on Thu Oct 31 11:50:48 AM EDT 2024

bowtie2

The script used to build this module can be found here: https://github.com/northeastern-rc-software-modules/bowtie2-2.5.4

To load the module, type:
module load bowtie2/2.5.4

}
conflict        bowtie2
prepend-path    PATH /shared/EL9/explorer/bowtie2/2.5.4/src/bowtie2-2.5.4-linux-x86_64
prepend-path    PATH /shared/EL9/explorer/bowtie2/2.5.4/src/bowtie2-2.5.4-linux-x86_64/scripts
-------------------------------------------------------------------

fastqc module

/shared/EL9/explorer/modulefiles/fastqc/0.12.1:

module-whatis   {Loads fastqc/0.12.1 module.

This module was built on Mon Jan 13 02:08:39 PM EST 2025

fastqc

The script used to build this module can be found here: https://github.com/northeastern-rc-software-modules/FastQC-0.12.1

To load the module, type:
module load fastqc/0.12.1

}
conflict        fastqc
prepend-path    PATH /shared/EL9/explorer/fastqc/0.12.1/src/FastQC
module-whatis   {Loads fastqc/0.12.1 module.

This module was built on Thu Jan 30 02:27:01 PM EST 2025

fastqc

The script used to build this module can be found here: https://github.com/northeastern-rc-software-modules/FastQC-0.12.1

To load the module, type:
module load fastqc/0.12.1

}
module          load OpenJDK/22.0.2
module          load perl/5.40.0
conflict        fastqc
prepend-path    PATH /shared/EL9/explorer/fastqc/0.12.1
-------------------------------------------------------------------

bamtools module
-------------------------------------------------------------------
/shared/EL9/explorer/modulefiles/bamtools/2.5.2:

module-whatis   {Loads bamtools/2.5.2 module.

This module was built on Thu Nov  7 09:23:46 AM EST 2024

bamtools

The script used to build this module can be found here: https://github.com/northeastern-rc-software-modules/bamtools-2.5.2

To load the module, type:
module load bamtools/2.5.2

}
conflict        bamtools
prepend-path    PATH /shared/EL9/explorer/bamtools/2.5.2/bin
prepend-path    PATH /shared/EL9/explorer/bamtools/2.5.2/lib64
prepend-path    PATH /shared/EL9/explorer/bamtools/2.5.2/include
module-whatis   {Loads bamtools/2.5.2 module.

This module was built on Thu Nov  7 11:43:54 AM EST 2024

bamtools

The script used to build this module can be found here: https://github.com/northeastern-rc-software-modules/bamtools-2.5.2

To load the module, type:
module load bamtools/2.5.2

}
conflict        bamtools
prepend-path    PATH /shared/EL9/explorer/bamtools/2.5.2/bin
prepend-path    PATH /shared/EL9/explorer/bamtools/2.5.2/lib64
prepend-path    PATH /shared/EL9/explorer/bamtools/2.5.2/include
-------------------------------------------------------------------

samtools module
-------------------------------------------------------------------
/shared/EL9/explorer/modulefiles/samtools/1.21:

module-whatis   {Loads samtools/1.21 module.

This module was built on Fri Oct 25 02:14:35 PM EDT 2024

samtools

The script used to build this module can be found here: https://github.com/northeastern-rc-software-modules/samtools-1.21

To load the module, type:
module load samtools/1.21

}
conflict        samtools
prepend-path    PATH /shared/EL9/explorer/samtools/1.21/bin
prepend-path    LIBRARY_PATH /shared/EL9/explorer/samtools/1.21/lib
prepend-path    LD_LIBRARY_PATH /shared/EL9/explorer/samtools/1.21/lib
prepend-path    CPATH /shared/EL9/explorer/samtools/1.21/include
-------------------------------------------------------------------

module star
-------------------------------------------------------------------
/shared/EL9/explorer/modulefiles/star/2.7.11b:

module-whatis   {Loads star/2.7.11b module.

This module was built on Fri Jan 17 09:53:10 AM EST 2025

Spliced Transcripts Alignment to a Reference (STAR) is a fast RNA-seq read mapper, with support for splice-junction and fusion read detection

The script used to build this module can be found here: https://github.com/northeastern-rc-software-modules/STAR-2.7.11b.git

To load the module, type:
module load star/2.7.11b

}
conflict        star
prepend-path    PATH /shared/EL9/explorer/star/2.7.11b/STAR-2.7.11b/bin
prepend-path    LIBRARY_PATH /shared/EL9/explorer/star/2.7.11b/STAR-2.7.11b/lib
prepend-path    LD_LIBRARY_PATH /shared/EL9/explorer/star/2.7.11b/STAR-2.7.11b/lib
prepend-path    CPATH /shared/EL9/explorer/star/2.7.11b/STAR-2.7.11b/include
-------------------------------------------------------------------

bcftools module
-------------------------------------------------------------------
/shared/EL9/explorer/modulefiles/bcftools/1.21:

module-whatis   {Loads bcftools/1.21 module.

This module was built on Fri Oct 25 01:26:54 PM EDT 2024

bcftools

The script used to build this module can be found here: https://github.com/northeastern-rc-software-modules/bcftools-1.21

To load the module, type:
module load bcftools/1.21

}
conflict        bcftools
prepend-path    PATH /shared/EL9/explorer/bcftools/1.21/bin
prepend-path    LIBRARY_PATH /shared/EL9/explorer/bcftools/1.21/lib
prepend-path    LD_LIBRARY_PATH /shared/EL9/explorer/bcftools/1.21/lib
prepend-path    CPATH /shared/EL9/explorer/bcftools/1.21/include
prepend-path    BCFTOOLS_PLUGINS /shared/EL9/explorer/bcftools/1.21/src/bcftools-1.21/plugins
-------------------------------------------------------------------
