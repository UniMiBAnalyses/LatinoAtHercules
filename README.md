# LatinoAtHercules


Tutorials
====

Main latino twiki page:

    https://twiki.cern.ch/twiki/bin/view/CMS/LatinosTwiki
    
Check the tutorials:

    https://twiki.cern.ch/twiki/bin/view/CMS/LatinosFrameworkTutorials
    
In particular, details and main idea of how mkshape+mkplot and mkshape+mkdatacard work here (from the previous link):

    Plots: mkShape and mkPlot



Install at Hercules 
====




Location of the ntuples
====

In general the ntuples, as tranferred via webfts, end up being stored in:

    ls /gwteras/cms/store/group/OneLepton/

that corresponds to the grid-aware storage element:

    srm://storm.mib.infn.it:8444/cms/store/group/OneLepton/

    
Name of the folders:

From the name of the folder one can understand which modules have been run:

    e.g. /gwteras/cms/store/group/OneLepton/Apr2017_summer16/lepSel__MCWeights__bSFLpTEffMulti__cleanTauMC__l2loose__hadd__l2tightOR__LepTrgFix__dorochester__formulasMC__ssSel
    
Here we have:

    lepSel__MCWeights__bSFLpTEffMulti__cleanTauMC__l2loose__hadd__l2tightOR__LepTrgFix__dorochester__formulasMC__ssSel
    
And the different modules run are:

    lepSel
    MCWeights
    bSFLpTEffMulti
    
and so on, as defined in:

    https://github.com/latinos/LatinoAnalysis/blob/master/Gardener/python/Gardener_cfg.py#L3237-L3242
    
    
The ntuples can then be migrated to gwteray/other so that we can run further modules of the gardener, add more variables and do skims.
Location still to be defined.

    

PlotsConfigurations
====


If you want to develop a new configuration in parallel with respect to the master repository, download from the UniMiBAnalyses the PlotConfigurations:

    git clone git@github.com:UniMiBAnalyses/PlotsConfigurations.git

Remember at some point to merge with the main repository, to make things more useful:

    https://github.com/latinos/PlotsConfigurations/
    
