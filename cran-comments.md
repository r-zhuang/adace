## Test environments
* local R installation, R 4.2.0
* Ubuntu Linux 20.04.1 LTS (on R-hub), R 4.2.0
* R-hub fedora-clang-devel (r-devel)
* Windows (devel and release)

## R CMD check results
The package was originally archived. This submission provides a second version
of the package and fixes any errors from the original package. There are no
ERRORs or WARNINGS during package checking, but 5 notes.

1. One related to the archival of this package:

On windows-x86_64-devel (r-devel), ubuntu-gcc-release (r-release)
  checking CRAN incoming feasibility ... NOTE
  Maintainer: 'Run Zhuang <capecod0321@gmail.com>'
  
  New submission
  
  Package was archived on CRAN
  
  Possibly misspelled words in DESCRIPTION:
    Adherer (2:25)
    Qu (40:5)
    Zhang (41:5)
    al (40:11, 41:15)
    et (40:8, 41:11)

2. One that is only found on Windows (Server 2023, R-devel 64-bit):

On windows-x86_64-devel (r-devel), ubuntu-gcc-release (r-release), 
fedora-clang-devel (r-devel)
  checking HTML version of manual ... NOTE
  Skipping checking math rendering: package 'V8' unavailable
  
3. As noted in R-hub issue #560, this seems to be an Rhub issue and so can 
likely be ignored.

❯ On windows-x86_64-devel (r-devel)
  checking for non-standard things in the check directory ... NOTE
  Found the following files/directories:
    ''NULL''
    
4. Another that is only found on Windows (Server 2023, R-devel 64-bit):

❯ On windows-x86_64-devel (r-devel)
  checking for detritus in the temp directory ... NOTE
  Found the following files/directories:
    'lastMiKTeXException'

5. No mispelled words.

❯ On fedora-clang-devel (r-devel)
  checking CRAN incoming feasibility ... [4s/13s] NOTE
  Maintainer: ‘Run Zhuang <capecod0321@gmail.com>’
  
  New submission
  
  Package was archived on CRAN
  
  Possibly misspelled words in DESCRIPTION:
    Adherer (2:25)
    Qu (40:5)
    Zhang (41:5)
    al (40:11, 41:15)
    et (40:8, 41:11)
    

