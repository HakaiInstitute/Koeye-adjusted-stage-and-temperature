Koeye gauge data calibration methods 

Overview - 
The Koeye River stream elevation gauge was first installed in September 2013. This original gauge was a Hobo U20 water level logger, and was installed upstream of the smolt-trap site on the lower Koeye River in a still built from perforated PVC pipe with a cement block as it’s base. This gauge operated more or less continuously until May 27, 2019, when the battery finally died. Throughout this 6-year period the original stream gauge in Koeye provided vital insights into the flow conditions encountered by juvenile and adult salmon in the Koeye River, and stream elevation data from the site were used as a covariate in a number of analyses, including relating adult sockeye survival and smolt capture probability during the spring smolt trapping season to river flow. 

A second stream elevation gauge (also a Hobo U20) was installed by Hakai in late August of 2017. This gauge was installed using a much more robust and permanent anchoring and still system. This gauge continues to operate, providing ongoing monitoring of flow conditions in the lower Koeye River, however in order to use these data in existing analyses there was a need to calibrate the Hakai gauge with the original gauge dataset. 

Analysis – 
To calibrate the two gauge datasets we used a generalized additive model (gam) written in the statistical program R. This model assumed that residual errors followed a gaussian distribution and related the original Koeye gauge values (response variable) to the new Hakai gauge values (predictor variable). Goodness of fit was evaluated visually using residual plots. We then extrapolated the estimated relationship between the two gauge datasets to generate predictions of the old gauge height for dates after May 27, 2019 using the predict() function in R. 

