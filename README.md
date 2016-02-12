# RecoilCorrections

MET recoil corrections

----- How to set up the MET Recoil Correction Interface ------

> cd ${CMSSW_BASE}/src

> cmsenv

> git clone https://github.com/CMS-HTT/RecoilCorrections.git HTT-utilities/RecoilCorrections 

> scram b 

---- How to use the code ------------

// Add the header file to your source file

#include "HTT-utilities/RecoilCorrections/interface/RecoilCorrector.h"

// Create instances of class RecoilCorrection and

// load recoil resolution functions

RecoilCorrector recoilPFMetCorrector("HTT-utilities/RecoilCorrections/data/recoilPFMet.root");

RecoilCorrector recoilMvaMetCorrector("HTT-utilities/RecoilCorrections/data/recoilMvaMet.root");
  
RecoilCorrector recoilPuppiMetCorrector("HTT-utilities/RecoilCorrections/data/recoilPuppiMet.root");
 
// apply recoil corrections


