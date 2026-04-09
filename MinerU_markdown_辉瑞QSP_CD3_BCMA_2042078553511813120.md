# Supplementary Materials for “Leveraging quantitative systems pharmacology modeling for elranatamab regimen optimization in relapsed or refractory multiple myeloma ”

![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/ffa4ddd320f82c9b9132e432d34a17cdbe5284d52e9fd64dcaa4625b2cd67e48.jpg)



Supplementary Figure 1 Local sensitivity analysis, top 20 parameters shown. Each parameter was decreased and increased by $2 5 \%$ and we measured its effect on serum M-spike at treatment day 364 with dose of $1 0 0 0 \mathrm { u g / k g }$ . The six parameters boxed in red were selected to vary based on LSA, and on prior knowledge of known heterogeneity or lack of knowledge on reference value used. Parameters not shown in top 20 that are perturbed are: ????????????, ??????, ????1, and they were selected due to their uncertainty. All parameters and their descriptions are listed in Supplementary Table 3.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/4964f6ca556c6ac7270998b1e648c4f44f88006e2ad7b1208fc1a40f6e950474.jpg)



Supplementary Figure 2 Parameter distributions of plausible patients (PP, $\mathrm { n } > 4 0 0 0 $ ) and virtual patients (VP, $\mathbf { n } = 1 2 0$ , VP is a subset of PP).



a


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/3fd2eae942dccbd2c3a34ec767e014675175aad31cbd14bcf7d78cb665c14a7e.jpg)



b


# Cost/Objective function

# Integrated biomarker (Serum M-spike or FLC)

# Best biochemical response

Only arms with highdoseused 

Withinarm,patients arerankedandgrouped 

Groupmediansare matched 

# Paraprotein dynamics

All dosesused, weighted byarm size 

Medians over time are matched 

# Biochemical response rates

All doses weighted by armsize 

Response %bydose and（high/low)sBCMA 

Supplementary Figure 3 Genetic algorithm. (a) Schema of genetic algorithm when selecting virtual patients from plausible patients. The collection of virtual patients is called a virtual population. (b) Optimization function uses 3 metrics that use an integrated biomarker as input. The 3 metrics are best biochemical response (percent change from baseline at best response), paraprotein dynamics (percent change from baseline), and biochemical response rates. We stratified patients’ biochemical response by sBCMA levels at baseline (low vs high) by finding the threshold that best separates objective biochemical responders from non-responders using a logistic regression with response as the outcome and high/low sBCMA as a dichotomous predictive variable. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/32f06c5215c8e6d6914324cb2df3433ee261884d46113f91507ebb9af9bba74d.jpg)



Supplementary Figure 4 Calculating response metrics based depends on selected integrated paraproteins. Each plausible patient will have simulated longitudinal serum M-protein and serum FLC value, but only one paraprotein will be used for response calculation and this paraprotein is referred to as an integrated paraprotein. We select the integrated paraprotein by observing the serum paraproteins at baseline, prioritize M-protein if it is measurable (greater or equal to 0.5 $\mathrm { g / d L ) }$ , otherwise use FLC as biomarker of response. This will result in responses based on two different biomarkers across the plausible patients. The dynamics of the selected integrated paraprotein is then used to calculate response metrics.



a



Ab_CD3dimer (DCD3)concentrationby Tcell concentration


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/e847eec7b26c851baefc8d5971e620b4c34e8068ab55f749862c018dd06920f9.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/37ef0da707456514bff97ab371c2b250be09ba90ef848643c36cb8f228a439e5.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/e37e3e9c91e798107616e8b11f479d2c8ad0d2ce26e9cf2ab540823e53d0bbdf.jpg)



Supplementary Figure 5 Dimers per cell ratios to analyze dose-reduction. (a) After a QW to Q2W switch, the ratio of drug-CD3 dimers standardized by T cells in each compartment decrease, compared to a constant QW regimen, shown in blue and red curves, respectively. The decrease of dimers relative to T cell concentrations suggests that availability of receptors will increase and be able to bind and create trimers. (b) Trimer production, relative to tumor burden, is increased after a QW to Q2W switch, suggesting greater antitumor activity. (c) Drug-BCMA dimers relative to tumor burden in the bone marrow remain roughly similar between the schedules. In all figures, the median ratio is shown in a solid curve and the $9 5 \%$ confidence interval is shown in shaded areas.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/f0011fd9084d2230d500dc05136739818de67dda8103280c9600e3f513a7f0a8.jpg)



Supplementary Figure 6 Calibration of best biochemical response (BBR) or waterfall plots to the MM-3 cohort A study. BBRs from clinical data are ranked in descending order, then they are grouped into 10 groups (shown vertical dashed red lines). For each group, the median BBR is estimated (shown in vertical solid red lines). Our optimization algorithm minimizes each group’s median BRR between the virtual patients and the clinical data. PCFP: Percent change from baseline.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/63f984e5ed482352b6ea06a9d411e347a4c05cb2ed2a978c28c1a085eae7a3f8.jpg)



Supplementary Figure 7 Timeseries of free sBCMA in central compartment. Median and $9 5 \%$ confidence interval of simulations are shown in solid lines and grey shaded areas, respectively. Median and $9 5 \%$ confidence interval of MM-3 cohort A study are shown in black dots and black error bars, respectively. In the data, these variables correspond to biomarkers measured from two distinct assays. The simulated regimen is $1 2 ~ \mathrm { m g }$ on C1D1, $3 2 ~ \mathrm { m g }$ on C1D4, 76 mg on C1D8 and QW thereafter until C6, then $7 6 \mathrm { m g } \mathrm { Q } 2 \mathrm { W }$ (if confirmed response) for 6 additional cycles, then 76 mg Q4W (if response is maintained).


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/42b262409bfbccdbb549544d34a62ba2b18e88dfff5eca45bfaa7854202fbad9.jpg)



Supplementary Figure 8 Cytokine dynamics in QSP model include attenuation of peaks and replicate observed median of IL-6 levels in MM-3 study. Visual check shows that fitted VPops accurately follow observed trends of IL-6 for MM3 study, which followed a priming regimen of $1 2 ~ \mathrm { m g }$ on C1D1, $3 2 { \mathrm { ~ m g ~ C l D 3 } }$ , and $7 6 ~ \mathrm { m g } ~ \mathrm { C l D 8 }$ and weekly thereafter. Median and $9 5 \%$ confidence intervals of observed IL6 levels in MM3 patients are shown in black dots and black error bars, respectively. Median and $9 5 \%$ prediction interval of projected IL-6 levels are shown in a blue solid line and filled area, respectively.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/8acc2455007751730c6a73b07dbd85fcbd06adb99241d93f177b46fa054bcf30.jpg)



Supplementary Figure 9 MM1 spider plots for one dose escalation arm. Shown VPop is the same as that shown in Figure 2c. This study arm was substantially smaller regarding study size, with 6 participants compared to MM3-Cohort A large study $\mathbf { N } = 1 2 0$ participants). VPop shows that observed variability was captured at most observed points. Median change from baseline and $9 5 \%$ prediction intervals of a VPop are shown in the red solid line and shaded area, respectively, compared to the observed median and $9 5 \%$ coverage of observed values shown in black dots and error bars, respectively.



a


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/0791621de72903ae2e14d6bfa513027e255f68cf4db57e3b1132194aa0e08243.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/02d57bf405fc5c276fd27887ed59e0354375c7fea88dcbe841146099007736a4.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/a69e67271caa4fa3dbae13172f42b2facb4dc1587db5715ad7b2230354473666.jpg)



Supplementary Figure 10 Individual simulated dose-response curves are used to stratify patients into 3 types: increasing (patients who will have higher trimer:BCMA ratio as drug increases), decreasing (patients who will have higher trimer:BCMA ratio as drug decreases), or bell-shape. A) Majority of virtual patients fall into the first category, whereas less than $10 \%$ will have decreasing dose-response curve. B) Additional dose-response curves in virtual patients, each dose is colored by simulated biochemical response (blue $=$ response, black $=$ no response) for the virtual patient in panel. Virtual


patients 6 and 7 are classified as bell-shaped, and they interestingly will reach a biochemical response with doses $4 4 - 7 6 \log \mathrm { Q W }$ but did not reach a response at $1 6 \mathrm { m g } \mathrm { Q W }$ or $1 5 2 ~ \mathrm { m g } \mathrm { Q W } . \mathrm { C }$ ) BRR across doses for each dose-response curve type shows that the increasing group has better BRR as dose increases, decreasing type has worse BRR, but bell-shaped curve type reaches maximum BRR at 76 mg QW. 


a


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/da96ab794d25c96fa67c25722ae77fe9eec66bbc1b3a260aa6331bbc48b153fb.jpg)



b


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/645cb51218ab08faf3362422ad22a9c54ae2a8243bacae79da2fde8607fe8d00.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/476f0ab52061ab343c3bc21858955ac846aa09e30cdd2a20e8061588bb31b25e.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/83b2b3ecd783d72c50febc233d4777320b01d2f2926ca92627d30bfa54a82856.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/7321698a20b96c542160007fee64311903721c8a0d1b80ef3d4a1232be3d4fea.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/9b5aed74eaa97a836e82e2ce80b80f8c61dc7e1ae59ad838bd4228761ad7202e.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/dc95c49fa577e6ce9db8a92c3d18cf50cc3c209a299e765f497400f6b0a05609.jpg)



Supplementary Figure 11 Factors that were identified as the most statistically significant simultaneously for predicting dose-response curve type are A) sBCMA at baseline, B) T cell concentration at baseline, and C) $\alpha _ { k i l l }$ , kill constant parameter that was perturbed across virtual patients. Further exploration of the relationship between sBCMA and T cells showed that, as expected, these variables were not correlated, suggesting that both these factors are important and independently


influence response. Higher levels of these factors seem to be associated with an increasing doseresponse type, but it is important to note that too much sBCMA resulted in no response despite having an increasing dose-response curve type. Small levels of T cell concentration resulted in a decreasing dose-response curve type, suggesting low to no efficacy as shown in Supplementary Figure 10b. Thus, if a theoretical patient has low BL sBCMA, our model suggests that T cell concentrations, which are measurable in clinic, can also affect response levels, with lower levels lowering the chance of efficacy despite patient to be considered “low risk” due to sBCMA levels. Unfortunately, parameters such as $\alpha _ { k i l l }$ are not measurable in clinic, suggesting additional unobserved tumor efficacy variables in clinic that one may not account for during dose selection. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/4261854e522faae08e08037e5b4adc4fe2c35d37c0b762c2e0050dbde73a30dc.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/ae413804974783f64996b77065ea285222a2a11d3363622a5647670a9fed66e8.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-04-09/41eb4e68-f616-444d-82c6-2dd410e39789/72916bc47d2f30111cb3ce92ada91dd58d95cba11aa89ac899d9ba3f34eb6c06.jpg)



Days of treatment



Supplementary Figure 12 Virtual patients (red) matched to observed patient’s trajectories (blue). Three participants from the MM-3 study with different paraprotein trajectories were identified and matched to three virtual patients from one of the 10 VPops. Panel #1 corresponds to an observed patient and a matched virtual patient who showed early response and maintained it after more than 2.5 years of treatment. Panel #2 shows that both observed and virtual patient had progressive disease after day 300 due to paraprotein elevations. Lastly, panel #3 shows an observed and a matched virtual patient that did not show a response and were removed from the trial due to progression after day 50 with a similar relative increase in paraprotein levels.



Supplementary Table 1 : Parameters Varied to generate PP


<table><tr><td>Parameter Name</td><td>Definition</td><td>Units</td><td>Default Value</td><td>VPop Range (LSA)</td><td>Reference</td></tr><tr><td>CD3density</td><td>Density of CD3 receptors on T cells</td><td>Receptor/cell</td><td>6 × 104</td><td>±25%</td><td>[5]</td></tr><tr><td>kresist</td><td>Rate of resistance maximal effect on trimer kill EC50 due to weakened T cell activation</td><td>1/hr</td><td>0.1</td><td>±2 fold</td><td>Calibrated</td></tr><tr><td>αresist</td><td>Maximal effect of resistance on trimer kill EC50 due to weakened T cell activation</td><td>hr</td><td>0.5</td><td>±2 fold</td><td>Calibrated</td></tr><tr><td>BCMAdensity</td><td>Density of BCMA receptors on tumor cell</td><td>Receptors/cell</td><td>1.259 × 104</td><td>±25%</td><td>[3]</td></tr><tr><td>kexp</td><td>Exponential-phase tumor growth rate</td><td>1/hr</td><td>3.32 × 10-4</td><td>±10 fold</td><td>[5, 7]</td></tr><tr><td>klin</td><td>Linear-phase tumor growth rate</td><td>Cells/hr</td><td>1500</td><td>±10 fold</td><td>[7]</td></tr><tr><td>τMM</td><td>Transit time between tumor cell death compartments</td><td>hr</td><td>27</td><td>24-30</td><td>[8]</td></tr><tr><td>αkill</td><td>Trimer tumor kill rate constant</td><td>1/hr</td><td>0.02</td><td>±10 fold</td><td>Calibrated</td></tr><tr><td>nkill</td><td>Trimer tumor kill rate Hill coefficient</td><td>unitless</td><td>0.8</td><td>0.5-1.5</td><td>Calibrated</td></tr></table>


Supplementary Table 1 : Parameters Varied to Generate PP. Each parameter was independently sampled from the biophysical ranges using uniform distributions . 



Supplementary Table 2 : Variables and Initial Conditions


<table><tr><td>Variable</td><td>Code Alias</td><td>Init. Value or [VPop Range]</td><td>Definition</td><td>Units</td></tr><tr><td>Ab_sc</td><td>Ab_sc</td><td>0</td><td>Free drug in sub-cutaneous compartment</td><td>pM</td></tr><tr><td>Ab_c</td><td>Ab_c</td><td>0</td><td>Free drug in central compartment</td><td>pM</td></tr><tr><td>Ab_BM</td><td>Ab_BM</td><td>0</td><td>Free drug in bone marrow compartment</td><td>pM</td></tr><tr><td>Tc_c</td><td>TC_c</td><td>[16 to 2,580]</td><td>T cells in central compartment</td><td>cells/uL</td></tr><tr><td>Tc_BM</td><td>TC_BM</td><td>[16 to 2,580]</td><td>T cells in bone marrow compartment</td><td>cells/uL</td></tr><tr><td>sBCMAc</td><td>sBCMA</td><td>[185 to 153,520]</td><td>Soluble BCMA in central compartment</td><td>pM</td></tr><tr><td>sBCMA_BM</td><td>sBCMA_BM</td><td>[185 to 153,520]</td><td>Soluble BCMA in bone marrow compartment</td><td>pM</td></tr><tr><td>Ab_sBCMAc</td><td>DsBCMA</td><td>0</td><td>Drug-sBCMA complex in central compartment</td><td>pM</td></tr><tr><td>Ab_CD3c</td><td>DCD3_c</td><td>0</td><td>Drug-T cell dimer in central compartment</td><td>pM</td></tr><tr><td>Ab_sBCMA_BM</td><td>DsBCMA_BM</td><td>0</td><td>Drug-sBCMA complex in tumor compartment</td><td>pM</td></tr><tr><td>Ab_BCMA_BM</td><td>DBCMA</td><td>0</td><td>Drug-MM cell dimer in tumor compartment</td><td>pM</td></tr><tr><td>Ab_CD3BM</td><td>DCD3_BM</td><td>0</td><td>Drug-T cell dimer in tumor compartment</td><td>pM</td></tr><tr><td>Trimer</td><td>Trimer_BM</td><td>0</td><td>Trimer between CD3, BCMA, and BsAB</td><td>pM</td></tr><tr><td>MM</td><td>TA</td><td>[0 to 450,000].</td><td>MM cells in BM</td><td>cells/uL</td></tr><tr><td>MMi</td><td>TAi</td><td>0</td><td>MM cells through (i=2-4) transit compartments</td><td>cells/uL</td></tr><tr><td>MP</td><td>MProtein</td><td>[0 to 70]</td><td>M-Protein in circulation</td><td>g/L</td></tr><tr><td>FLC</td><td>FLC</td><td>[0.92 to 174680]</td><td>FLC in circulation</td><td>mg/L</td></tr><tr><td>CBM</td><td>cytokine_BM</td><td>0</td><td>Cytokines shed by T cells after trimer</td><td>pg/mL</td></tr><tr><td>Ci</td><td>Cytokine_i</td><td>0</td><td>Cytokines through transit compartments (i = 1 - 5)</td><td>pg/mL</td></tr><tr><td>Cc</td><td>Cytokine_c</td><td>2.857</td><td>Cytokines in central compartment</td><td>pg/mL</td></tr></table>


Supplementary Table 2 : Model variables in QSP model . Initial conditions of drug concentration , dimers and trimer are set to zero , unless they are sampled from the reported range for PP generation . The distributions for the varied initial st ates were fitted to Pfizer baseline clinical dat a or obt ained from literature as described in Q S P P MAR− 1 5 1 3 . Initial values of the varied st at es ( ${ T } c _ { c }$ , $T c _ { B M }$ , $s B C M A _ { c }$ , ${ } _ { s B C M A _ { B M } }$ , MM, $M _ { p }$ and $F L C$ ) were sampled from ranges shown in square brackets . 



Supplementary Table 3 : Full Table of Parameters


<table><tr><td>Section in QSP Model</td><td>Name [Code Alias]</td><td>Description</td><td>Units</td><td>Value</td><td>Source</td></tr><tr><td rowspan="15">Sect. 1.1: BsAB Reactions Central</td><td>kon1 [kon_BCMA]</td><td>Binding of BsAB to BCMA</td><td>pM-1hr-1</td><td>0.0054</td><td>Fixed internal nonclinical data</td></tr><tr><td>koff1 [koff_BCMA]</td><td>Unbinding rate</td><td>hr-1</td><td>0.162</td><td>Fixed internal nonclinical data</td></tr><tr><td>kon2 [kon_CD3]</td><td>Binding of BsAB to CD3</td><td>pM-1hr-1</td><td>0.00198</td><td>Fixed internal nonclinical data</td></tr><tr><td>koff2 [koff_CD3]</td><td>Unbinding rate</td><td>hr-1</td><td>82.17</td><td>Fixed internal nonclinical data</td></tr><tr><td>kdeg_sBCMA [kdeg_sBCMA]</td><td>Degradation of sBCMA</td><td>hr-1</td><td>0.01925</td><td>Fixed internal nonclinical data</td></tr><tr><td>ktrc_BM [k_Ab_c_BM]</td><td>BsAB transport rate from central to BM</td><td>hr-1</td><td>0.1</td><td>Estimated with clinical data</td></tr><tr><td>ktrBM_c [k_Ab_BM_c]</td><td>BsAB transport rate from BM to central</td><td>hr-1</td><td>0.3</td><td>Estimated with clinical data</td></tr><tr><td>ktrsBCMA_BM_c [k_SBCMA_BM_c]</td><td>Ab_sBCMA dimer transport rate from BM to central</td><td>hr-1</td><td>0.1</td><td>Assumed equal to ktrc_BM</td></tr><tr><td>kel [kel]</td><td>Elimination rate of BsAB and sBCMA dimer</td><td>hr-1</td><td>CL/Vc</td><td>Preliminary PopPK</td></tr><tr><td>ka [ka]</td><td>Drug absorption rate</td><td>hr-1</td><td>6.167E-3</td><td>Preliminary PopPK</td></tr><tr><td>F [F_SC]</td><td>Drug bioavailability</td><td></td><td>0.511</td><td>Preliminary PopPK</td></tr><tr><td>Vc [V1]</td><td>Volume in central</td><td>L</td><td>4.25</td><td>Preliminary PopPK</td></tr><tr><td>Vp [V2]</td><td>Volume of peripheral</td><td>L</td><td>7.8</td><td>Preliminary PopPK</td></tr><tr><td>Q [Q]</td><td>Inter-compartmental clearance</td><td>L/hr</td><td>0.008416</td><td>Preliminary PopPK</td></tr><tr><td>Cl [CL]</td><td>Clearance</td><td>mL/hr</td><td>13.9583</td><td>Preliminary PopPK</td></tr><tr><td rowspan="6">Sect. 1.2: T cell &amp; Cytokines Central</td><td>kTC_c_BM [k_TC_c_BM]</td><td>T cell transport from central to BM</td><td>hr-1</td><td>0.2</td><td>Estimated with clinical data and literature [14]</td></tr><tr><td>kTC_BM_c [k_TC_BM_c]</td><td>T cell transport from BM to central</td><td>hr-1</td><td>0.3893</td><td>Estimated with clinical data and literature [14]</td></tr><tr><td>kel_T [kel_TC_c]</td><td>T cell elimination rate in central</td><td>hr-1</td><td>0.1046</td><td>Fixed Literature [1]</td></tr><tr><td>βprod [basalproduction]</td><td>Basal cytokine production</td><td>pg/mL/hr</td><td>1</td><td>Estimated literature [14]</td></tr><tr><td>kdeg_cyt [cr_kdeg]</td><td>Degradation of cytokines</td><td>hr-1</td><td>0.5</td><td>Estimated with clinical data and literature [14]</td></tr><tr><td>ktrcyt [k_tr_cyt]</td><td>Cytokine transit rates from BM to central</td><td>hr-1</td><td>0.625</td><td>Estimated with clinical data and literature [14]</td></tr><tr><td rowspan="2">Sect. 1.3: Paraproteins Central</td><td>kdeg_Mp [MProtein_deg]</td><td>Degradation rate of M-protein</td><td>hr-1</td><td>0.0021</td><td>Fixed Literature [12]</td></tr><tr><td>kdeg_FLC [FLC_deg]</td><td>Degradation rate of FLC</td><td>hr-1</td><td>0.1733</td><td>Fixed Literature [13]</td></tr><tr><td>Sect. 2.2: Tumor Cells BM</td><td>VBM</td><td>Volume of bone marrow compartment</td><td>L</td><td>1.75</td><td>Fixed Literature [11, 10]</td></tr></table>

<table><tr><td>k0g0 [kg0]</td><td>Exponential tumor growth rate</td><td>hr-1</td><td>3.32 × 10-4</td><td>Calibrated with clinical data and literature [6, 4, 7]</td></tr><tr><td>k1g1 [kg1]</td><td>Linear tumor growth rate</td><td>cells/hr</td><td>1500</td><td>Calibrated with clinical data and literature [6, 7]</td></tr><tr><td>ψ [growth.switch]</td><td>Switch between exponential and linear growth phases</td><td></td><td>20</td><td>Fixed Literature [9]</td></tr><tr><td>αkill [alpha_kill]</td><td>Kill constant</td><td>hr-1</td><td>0.02</td><td>Calibrated with clinical data</td></tr><tr><td>km [km_kill]</td><td>Half saturation for tumor killing</td><td>pM/cells/uL</td><td>4.25E-4</td><td>Estimated with clinical data and literature [14]</td></tr><tr><td>nkill [n_kill]</td><td>Cooperativity coefficient kill constant</td><td></td><td>0.8</td><td>Calibrated with clinical data</td></tr><tr><td>τM [tau_TA]</td><td>Transit time to MM cell death</td><td>hr</td><td>24</td><td>Calibrated with clinical data and literature [8]</td></tr><tr><td>MMax</td><td>Maximum tumor burden</td><td>cells/uL</td><td>3 × 10^6</td><td>Estimated with clinical data</td></tr><tr><td>αresis [alpha_resis]</td><td>Maximum addition resistance</td><td></td><td>0.5</td><td>Calibrated with clinical data</td></tr><tr><td>βresis [beta_resis]</td><td>Rate of change of resistance</td><td>hr-1</td><td>0.1</td><td>Calibrated with clinical data</td></tr><tr><td>τresis [tau_resis]</td><td>Time to resistance</td><td>hr</td><td>600</td><td>Estimated with clinical data</td></tr><tr><td>BCMAdensity[BCMA_density]</td><td>Density of BCMA receptors per tumor cell</td><td>receptor/cell</td><td>12590</td><td>Calibrated with clinical data and literature [3]</td></tr><tr><td colspan="5">Sect. 2.3: T Cell &amp; Cytokines BM</td></tr><tr><td>CD3density[CD3_density]</td><td>Density of CD3 receptors per T cell</td><td>receptor/cell</td><td>6 × 10^4</td><td>Calibrated with clinical data and literature [5]</td></tr><tr><td>Imax [cr_Imax]</td><td>Maximum cytokine inhibition on cytokine release</td><td></td><td>1</td><td>Fixed Literature [2]</td></tr><tr><td>n1C [cr_n_IH]</td><td>Cooperativity coefficient for cytokine release inhibition</td><td></td><td>2.5</td><td>Fixed Literature [2]</td></tr><tr><td>IC50 [cr_IC50]</td><td>Cytokine concentration resulting in 50% release inhibition</td><td>pg/mL×hr</td><td>10000</td><td>[2]</td></tr><tr><td>K [cr_K]</td><td>Priming factor</td><td></td><td>2.83</td><td>[2]</td></tr><tr><td>N [n_dose_count]</td><td>Number of doses</td><td></td><td>1</td><td>[2]</td></tr><tr><td>Emax [cr_Emax]</td><td>Maximum cytokine release rate</td><td>pg/mL/hr</td><td>80590</td><td>[2]</td></tr><tr><td>EC50 [cr_EC50]</td><td>Exposure of active drug species to achieve 50% of Emax</td><td>pM</td><td>0.5</td><td>[2]</td></tr><tr><td>n2C [cr_n]</td><td>Hill coefficient for cytokine release</td><td></td><td>1</td><td>[2]</td></tr><tr><td>ImaxTC [Imax_TC]</td><td>Maximum T cell migration inhibition</td><td></td><td>1</td><td>Estimated</td></tr><tr><td>K1 [ksat_TC]</td><td>Cytokine concentration at 50% of ImaxTC</td><td>pg/mL</td><td>150</td><td>Estimated</td></tr><tr><td>K2 [ksat_Trimer_TC]</td><td>Trimer concentration at 50 % of ImaxTC</td><td>pM</td><td>0.02</td><td>Estimated</td></tr><tr><td>ncyt [n_cytokine_TC]</td><td>Hill coefficient T cell transport inhibition from cytokines</td><td></td><td>2</td><td>Estimated</td></tr><tr><td>ntri [n_Trimer_TC]</td><td>Hill coefficient T cell transport inhibition from trimers</td><td></td><td>1.5</td><td>Estimated</td></tr></table>


Supplementary Table 3 : Parameters in QSP model.



Supplementary Table 4: Study Data used for Model Calibration


<table><tr><td>Study (N)</td><td>Elranatamab Dosing Regimen</td><td>Day(s) of sampling (SPEP, serum FLC)</td><td>Day(s) of sBCMA and PK Sampling</td></tr><tr><td>C1071001 Part 1 (23)</td><td>IV: 0.1, 0.3, 1, 3, 10, 30, and 50 μg/kg QW</td><td>Screening: -14 to 1</td><td></td></tr><tr><td>Cycle 1: 1</td><td>Cycle 1: 1</td><td></td><td></td></tr><tr><td>C1071001 Part 1 (30)</td><td>SC: 80, 130, 215, 360, 600, and 1000 μg/kg QW</td><td>Screening: -14 to 1</td><td></td></tr><tr><td>Cycle 1 onwards: 1</td><td>Cycle 1: 1, 8, 15</td><td></td><td></td></tr><tr><td>Cycle 2: 1, 8, 15</td><td></td><td></td><td></td></tr><tr><td>Cycle 3 onwards: 1</td><td></td><td></td><td></td></tr><tr><td>C1071001 Part 1 C-D (13)</td><td>SC: combination</td><td>Screening: -14 to -1</td><td></td></tr><tr><td>Cycle 1: 1</td><td>Cycle 1: 1</td><td></td><td></td></tr><tr><td>C1071001 Part 1.1 QW (7)</td><td>SC: 600 μg/kg for the first week, then 1000 μg/kg QW</td><td>Screening: -14 to -1</td><td></td></tr><tr><td>Cycle 0: 0</td><td></td><td></td><td></td></tr><tr><td>Cycle 1 onwards: 1</td><td>Cycle 0: 0</td><td></td><td></td></tr><tr><td>Cycle 1: 1, 8, 15, 22</td><td></td><td></td><td></td></tr><tr><td>Cycle 2: 1, 8, 15, 22</td><td></td><td></td><td></td></tr><tr><td>Cycle 3 onwards: 1</td><td></td><td></td><td></td></tr><tr><td>C1071001 Part 1.1 Q2W (13)</td><td>SC: 600 μg/kg for the first week, then 1000 Q2W</td><td>Screening: -14 to -1</td><td></td></tr><tr><td>Cycle 0: 0</td><td>Cycle 0: 0</td><td></td><td></td></tr><tr><td>C1071001 Part 2Aa (15)</td><td>SC: 44 mg for the first week, then 76 mg QW</td><td>Screening: -14 to -1</td><td></td></tr><tr><td>Cycle 0: 0</td><td></td><td></td><td></td></tr><tr><td>Cycle 1 onwards: 1</td><td>Cycle 0: 0</td><td></td><td></td></tr><tr><td>Cycle 1: 1, 8, 15, 22</td><td></td><td></td><td></td></tr><tr><td>Cycle 2: 1, 8, 15, 22</td><td></td><td></td><td></td></tr><tr><td>Cycle 3 onwards: 2</td><td></td><td></td><td></td></tr><tr><td>C1071003a Part A (120)</td><td>SC: 12/32/76 mg</td><td>Screening: -28 to -1</td><td></td></tr><tr><td>Cycle 1 onwards: 1</td><td>C1D1/C1D4/C1D8 then 76 mg QWb</td><td></td><td></td></tr><tr><td>Cycle 2, 3, 4, 7, 10, etc.: 1</td><td>Cycle 1: 1, 4, 8, 15, 22</td><td></td><td></td></tr></table>

Supplementary Table 4: Source: Protocol for Study C1071001, Protocol for Study C1071003. 

$^ { a }$ Premedication with acetaminophen, diphenhydramine, and dexamethasone. 

$^ { b }$ 76 mg Q2W after C6 with persistent response, 76 mg Q4W after C13. 

Table abbreviations: N = number of participants; IV = intravenous; PK = pharmacokinetic; RRMM = relapsed/refractory multiple myeloma; PD = pharmacodynamic; QW = once a week; SC = subcutaneous. 

# Supplementary Note 1

# 1 QSP Model Description and Assumptions

# 1.1 Central compartment

In the central compartment, the key interactions captured by the model are binding of BsAB to shed sBCMA receptors in circulation, as well as to circulatory T cell CD3 receptors. In addition, circulatory paraproteins (M-protein, FLC) and generic cytokine reactions are also included in this compartment. Serum FLC and M-protein dynamics are given by a balance of synthesis rates, proportional to total tumor burden, and degradation rates. 

# 1.1.1 BsAB binding kinetics in central compartment

The free drug, corresponding to unbound BsAB, denoted by $[ A b _ { c } ]$ can flow in from a subcutaneous compartment in the case of SC modality and also exchange with a peripheral compartment $[ A b _ { p } ]$ . Free drug can bind either to unbound soluble BCMA receptors $\left( \left[ s B C M A _ { c } \right] \right)$ ) or to free circulating CD3+T cell receptors $[ C D 3 _ { c } ] )$ ). 

We outline a few assumptions made to reduce the number of parameters: 

 The free drug, corresponding to unbound BsAB, denoted by $[ A b _ { c } ]$ can flow in from a subcutaneous compartment in the case of SC modality and also exchange with a peripheral compartment $[ A b _ { p } ]$ . 

 Free drug can bind either to unbound soluble BCMA receptors $( \left\lfloor s B C M A _ { c } \right\rfloor )$ ) or to free circulating CD3+T cell receptors $\left( [ C D 3 _ { c } ] \right)$ ). 

 The elimination rate for the unbound bispecific, $[ A b _ { c } ]$ and bispecific sBCMA dimers are assumed to be the same $k _ { e l }$ . 

 Similar to work of [1], a trimer between sBCMA and T cells in circulation is omitted from the model equations since this species is not pharmacologically active. 

 Synthesis of sBCMA in the central compartment is assumed to be proportional to the amount of sBCMA that enters the central compartment from the bone marrow and the system was in steady state at baseline ( $t = 0$ ). 

Thus the equations in their final form read: 

$$
\frac {d \left[ A b _ {c} \right]}{d t} = \frac {\text {I n p u t} _ {i v}}{V _ {c}} + \frac {F k _ {a} \left[ A b _ {s c} \right]}{V _ {c}} - k _ {1 2} \left[ A b _ {c} \right] + k _ {2 1} \frac {V _ {p}}{V _ {c}} \left[ A b _ {p} \right] \tag {1}
$$

$$
- k _ {o n 1} \left[ A b _ {c} \right] \left[ s B C M A _ {c} \right] + k _ {\text {o f f 1}} \left[ A b _ {-} s B C M A _ {c} \right] - k _ {o n 2} \left[ A b _ {c} \right] \left[ C D 3 _ {c} \right] + k _ {\text {o f f 2}} \left[ A b _ {-} C D 3 _ {c} \right]
$$

$$
- k t r _ {c. B M} [ A b _ {c} ] + k t r _ {B M. c} \frac {V _ {B M}}{V _ {c}} [ A b _ {B M} ] - k _ {e l} [ A b _ {c} ]
$$

$$
\begin{array}{l} \frac {d [ s B C M A _ {c} ]}{d t} = k _ {\text {d e g .} s B C M A} \left(\frac {[ s B C M A _ {c} ^ {0} ]}{[ s B C M A _ {B M} ^ {0} ]} [ s B C M A _ {B M} ] - [ s B C M A _ {c} ]\right) (2) \\ - k _ {o n 1} \left[ A b _ {c} \right] \left[ s B C M A _ {c} \right] + k _ {\text {o f f 1}} \left[ A b _ {-} s B C M A _ {c} \right] (3) \\ \end{array}
$$

$$
\begin{array}{l} \frac {d [ A b _ {-} s B C M A _ {c} ]}{d t} = k _ {\text {o n 1}} [ A b _ {c} ] [ s B C M A _ {c} ] - k _ {\text {o f f 1}} [ A b _ {-} s B C M A _ {c} ] \tag {4} \\ + k t r _ {s B C M A _ {-} B M _ {-} c} \frac {V _ {B M}}{V _ {c}} [ A b _ {-} s B C M A _ {B M} ] - k _ {e l} [ A b _ {-} s B C M A _ {c} ] \\ \end{array}
$$

$$
\frac {d [ A b _ {-} C D 3 _ {c} ]}{d t} = k _ {o n 2} [ A b _ {c} ] [ C D 3 _ {c} ] - k _ {\text {o f f 2}} [ A b _ {-} C D 3 _ {c} ] \tag {5}
$$

In the next section we outline how the CD3 receptor counts are obtained for BsAB-T cell dimer formation. 

# 1.1.2 CD3+T cell and cytokine dynamics in the central compartment

We make the following assumptions: 

 CD3+T cells in the central compartment, denoted by $[ T c _ { c } ]$ can either flow out of the central compartment into tissues (peripheral) and tumor site (BM), be eliminated, or generate at a balanced rate proportional to initial circulating T cell counts $( T c _ { c } ^ { 0 } )$ . 

 Pro-inflammatory cytokines ( $\lfloor C _ { c } \rfloor$ ), e.g. IL-6, flow into the central compartment from the BM, when trimers are activated. 

 The individual T cell level receptor production is constant and set at literature obtained CD3 receptor values, similar to [1]. 

Accordingly, we write the following ODE for T cells and cytokines in circulation: 

$$
\frac {d [ T c _ {c} ]}{d t} = k _ {e l \_ T} [ T c _ {c} ^ {0} ] - (k _ {e l \_ T} + k _ {T C \_ c \_ B M}) [ T c _ {c} ] + k _ {T C \_ B M \_ c} [ T _ {B M} ] \frac {V _ {B M}}{V _ {c}} (1 - T _ {i n h}) \tag {6}
$$

$$
\frac {d \left[ C _ {c} \right]}{d t} = \beta_ {p r o d} + k _ {t r - c y t} \left[ C _ {5} \right] \frac {V _ {B M}}{V _ {c}} - k _ {d e g - c y t} \left[ C _ {c} \right]. \tag {7}
$$

We define $T _ { i n h }$ term which controls T cell outflow from site of action in section 1.2.3. 

To obtain the number CD3 receptors in the central compartment: 

$$
C D 3 _ {t o t - c} = \left[ T c _ {c} \right] \times C D 3 _ {d e n s i t y} \frac {L _ {-} t o _ {-} u L}{a v _ {-} n u m} 1 e 1 2 \tag {8}
$$

$$
C D 3 _ {c} = C D 3 _ {t o t \_ c} - A b \_ C D 3 _ {c} \tag {9}
$$

The initial conditions for these additional equations are: 

$$
[ T c _ {c} (0) ] = T c _ {c} ^ {0}, \quad [ C D 3 _ {c} (0) ] = [ T c _ {c} ^ {0} ] \times C D 3 _ {d e n s i t y} \frac {L _ {-} t o _ {-} u L}{a v _ {-} n u m} 1 e 1 2, \tag {10}
$$

which supports the dimer initial condition mentioned in the prior section, namely: 

$$
[ A b \_ C D 3 _ {c} (0) ] = 0.
$$

# 1.1.3 Paraproteins in the central compartment

Similar to the assumptions made for sBCMA, we make these assumptiosn for the paraprotein dynamics: 

 Basal M-spike and FLC synthesis in circulation is set to zero. 

 Paraprotein production is driven by tumor burden since the synthesis rate is proportional to total tumor burden in BM, $[ M M _ { t o t } ]$ . 

 Amount of paraprotein entering the central compartment from the bone marrow was in steady state at $t = 0$ . 

Thus, the model equations for paraproteins in the central compartment are: 

$$
\frac {d [ M _ {P} ]}{d t} = k _ {\text {d e g} - M p} \frac {[ M _ {P} ^ {0} ]}{[ M M _ {\text {t o t}} ^ {0} ]} [ M M _ {\text {t o t}} ] - k _ {\text {d e g} - M p} [ M _ {P} ] \tag {11}
$$

$$
\frac {d [ F L C ]}{d t} = k _ {d e g \_ F L C} \frac {[ F L C ^ {0} ]}{[ M M _ {t o t} ^ {0} ]} [ M M _ {t o t} ] - k _ {d e g \_ F L C} [ F L C ]. \tag {12}
$$

where $M M _ { t o t } = [ M M ] + [ M M _ { 2 } ] + [ M M _ { 3 } ] + [ M M _ { 4 } ]$ is the total tumor burden. Initial conditions are $M _ { P } ( 0 ) = M _ { P } ^ { 0 } , F L C ( 0 ) = F L C ^ { 0 }$ . 

# 1.2 Bone marrow (BM) compartment

In the bone marrow (BM) compartment, the key interactions captured by the model are binding of BsAb to shed sBCMA receptors in BM, membrane-bound BCMA receptors, and T cell CD3 receptors. A functional trimer is formed when BsAb is simultaneously bound to the BCMA and CD3 receptors, and this complex drives tumor-killing in the BM and cytokine release. 

# 1.2.1 Drug kinetics in Bone Marrow

We start with the following assumptions in the BM: 

 The rate of BCMA shedding is assumed to be proportional to tumor burden. 

 As assumed with other model states, the system is at steady state at $t = 0$ . 

 Central and BM binding rates are assumed to the the same 

 Complex formation rates for sBCMA and BCMA are assumed to be the same (i.e., BsAb binds to sBCMA and BCMA at same rate). 

The dynamics of free drug (BsAB) and sBCMA in the BM compartment are given by 

$$
\begin{array}{l} \frac {d \left[ A b _ {B M} \right]}{d t} = k _ {\text {o f f 1}} \left[ A b _ {-} s B C M A _ {B M} \right] - k _ {\text {o n 1}} \left[ A b _ {B M} \right] \left[ s B C M A _ {B M} \right] \tag {13} \\ + k _ {\text {o f f 2}} \left[ A b _ {-} C D 3 _ {B M} \right] - k _ {\text {o n 2}} \left[ A b _ {B M} \right] \left[ C D 3 _ {-} B M \right] + k _ {\text {o f f 1}} \left[ A b _ {-} B C M A _ {B M} \right] \\ - k _ {o n 1} [ A b _ {B M} ] [ B C M A _ {B M} ] - k t r _ {B M \_ c} [ A b _ {B M} ] + k t r _ {c \_ B M} \frac {V _ {c}}{V _ {B M}} [ A b _ {c} ] \\ \end{array}
$$

$$
\begin{array}{l} \frac {d [ s B C M A _ {B M} ]}{d t} = k _ {\text {d e g .} s B C M A} \frac {V _ {c}}{V _ {B M}} \frac {[ s B C M A _ {c} ^ {0} ]}{[ M M _ {\text {t o t}} ^ {0} ]} [ M M _ {\text {t o t}} ] - k t r _ {s B C M A} [ s B C M A _ {B M} ] \tag {14} \\ - k _ {o n 1} [ A b _ {B M} ] [ s B C M A _ {B M} ] + k _ {\mathrm {o f f 1}} [ A b _ {s} B C M A _ {B M} ] \\ \end{array}
$$

The rest of the dimerization and trimer formation equations are: 

$$
\begin{array}{l} \frac {d [ A b \_ B C M A _ {B M} ]}{d t} = k _ {\text {o n 1}} [ A b _ {B M} ] [ B C M A _ {B M} ] - k _ {\text {o f f 1}} [ A b \_ B C M A _ {B M} ] \tag {15} \\ - k _ {o n 2} \left[ A b _ {-} B C M A _ {B M} \right] \left[ C D 3 _ {B M} \right] + k _ {\text {o f f 2}} \left[ T r i m e r \right] \\ \end{array}
$$

$$
\begin{array}{l} \frac {d [ A b _ {-} s B C M A _ {B M} ]}{d t} = k _ {o n 1} [ A b _ {B M} ] [ s B C M A _ {B M} ] - k _ {\text {o f f 1}} [ A b _ {-} s B C M A _ {B M} ] (16) \\ - k t r _ {s B C M A _ {-} B M _ {-} c} \frac {V _ {B M}}{V _ {c}} [ A b _ {-} s B C M A _ {B M} ] (17) \\ \end{array}
$$

$$
\begin{array}{l} \frac {d [ A b \_ C D 3 _ {B M} ]}{d t} = k _ {\text {o n 2}} [ A b _ {B M} ] [ C D 3 _ {B M} ] - k _ {\text {o f f 2}} [ A b \_ C D 3 _ {B M} ] \tag {18} \\ - k _ {o n 1} \left[ A b _ {-} C D 3 _ {B M} \right] \left[ B C M A _ {B M} \right] + k _ {\text {o f f 1}} \left[ T r i m e r \right] \\ \end{array}
$$

$$
\begin{array}{l} \frac {d [ \text {T r i m e r} ]}{d t} = k _ {\text {o n 1}} [ A b _ {-} C D 3 _ {B M} ] [ B C M A _ {B M} ] - k _ {\text {o f f 1}} [ \text {T r i m e r} ] \tag {19} \\ + k _ {o n 2} \left[ A b _ {-} B C M A _ {B M} \right] \left[ C D 3 _ {B M} \right] - k _ {\text {o f f 2}} \left[ T r i m e r \right] \\ \end{array}
$$

The total receptor counts in the bone marrow are given by 

$$
C D 3 _ {t o t B M} = T c _ {B M} \times C D 3 _ {d e n s i t y} \frac {L _ {-} t o _ {-} u L}{a v _ {-} n u m} 1 e 1 2 \tag {20}
$$

$$
B C M A _ {t o t B M} = M M _ {t o t} \times B M C A _ {\text {d e n s i t y}} \frac {L _ {t o u L}}{a v _ {n u m}} 1 e 1 2 \tag {21}
$$

and the free receptors in the bone marrow are calculated: 

$$
B C M A _ {B M} = B C M A _ {t o t B M} - A b _ {-} B C M A _ {B M} - T r i m e r \tag {22}
$$

$$
C D 3 _ {B M} = C D 3 _ {t o t B M} - A b \_ C D 3 _ {B M} - T r i m e r. \tag {23}
$$

# 1.2.2 Tumor cell dynamics in BM

The equations for tumor plasma cell dynamics follow the standard Simeoni [9] tumor growth dynamics with a kill term driven by trimer concentration as follows: 

$$
\frac {d [ M M ]}{d t} = k _ {g _ {0}} \frac {1 - \frac {[ M M _ {t o t} ]}{M M _ {m a x}}}{\left(1 + \left(\frac {k _ {g _ {0}}}{k _ {g _ {1}}} M M _ {t o t}\right) ^ {\psi}\right) ^ {1 / \psi} [ M M ] - K _ {\mathrm {M k i l l}} [ M M ]} \tag {24}
$$

$$
\frac {d [ M M _ {2} ]}{d t} = K _ {\mathrm {M k i l l}} [ M M ] - \frac {4}{\tau_ {M}} [ M M _ {2} ] \tag {25}
$$

$$
\frac {d [ M M _ {3} ]}{d t} = \frac {4}{\tau_ {M}} [ M M _ {2} ] - \frac {4}{\tau_ {M}} [ M M _ {3} ] \tag {26}
$$

$$
\frac {d [ M M _ {4} ]}{d t} = \frac {4}{\tau_ {M}} [ M M _ {3} ] - \frac {4}{\tau_ {M}} [ M M _ {4} ] \tag {27}
$$

where $^ { \tau _ { M } }$ is a total delay transit compartment rate. The rate of tumor killing and the overall efficacy is dependent on the trimer to tumor ratio as follows: 

$$
K _ {\mathrm {M k i l l}} = \alpha_ {k i l l} \frac {(\frac {[ T r i m e r ]}{\varepsilon + [ M M ]}) ^ {n _ {k i l l}}}{k _ {m k i l l} ^ {n _ {k i l l}} + (\frac {[ T r i m e r ]}{\varepsilon + [ M M ]}) ^ {n _ {k i l l}}}.
$$

The term $\varepsilon$ is a small value introduced for numerical stability. With this formulation, tumor killing would be achieved if trimer levels are high while tumor levels are either low or high, or when trimer and tumor levels are both low. 

Finally, the tumor killing half-max effect term, $k _ { m k i l l }$ was designed to be time-dependent in order to capture the patients who showed initial FLC/M-protein lowering but then ultimately relapsed with an increase in paraproteins. This weakening of trimer kill efficacy over time can correspond to eventual attenuation of T cell activity due to variety of known mechanisms, such as PD-1 expression. We implement this effect using the following equation: 

$$
k _ {m k i l l} = k _ {m} \left(1 + \alpha_ {r e s i s} (1 - e ^ {- \beta_ {r e s i s} (t - \tau_ {r e s i s})}\right)
$$

where $\alpha _ { r e s i s }$ is the maximum addition resistance that increases the trimer/drug needed to induce efficacy, $\tau _ { r e s i s }$ is the time it takes for the resistance to occur, and $\beta _ { r e s i s }$ is the rate at which the resistance reaches maximum effect. 

# 1.2.3 CD3+T cell and cytokine dynamics in BM

For BM T cell and cytokine dynamics, we partially adapt the model of [2] with key focus on production of a pro-inflammatory cytokine (e.g., IL-6) in response to T cell activation due to binding in a trimer complex with MM cells in the BM. Additional assumptions or deviations from Chen et al. include: 

 Significant T cell activation in the BM results in inhibition of T cell back-flow from the BM back into circulation. 

 Cumulative cytokine exposure is reduced with each new dosing interval, instead of being set to 0. 

As in the central compartment, we have an equivalent BM equation for T cells: 

$$
\frac {d [ T c _ {B M} ]}{d t} = k _ {T C \_ c \_ B M} \frac {V _ {c}}{V _ {B M}} [ T c e l l s _ {c} ] - k _ {T C \_ B M \_ c} [ T c _ {B M} ] (1 - T _ {i n h}) \tag {28}
$$

with a T cell transport inhibition term, 

$$
T _ {i n h} = I _ {m a x T C} \left(\frac {\bar {C} _ {B M} ^ {n _ {c y t}}}{K _ {1} ^ {n _ {c y t}} + \bar {C} _ {B M} ^ {n _ {c y t}}}\right) \left(\frac {\text {T r i m e r} ^ {n _ {t r i}}}{K _ {2} ^ {n _ {t r i}} + \text {T r i m e r} ^ {n _ {t r i}}}\right). \tag {29}
$$

The quantity $C _ { B M } = ( C _ { B M } + C _ { 1 } + C _ { 2 } + C _ { 3 } + C _ { 4 } + C _ { 5 } ) / 6$ gives the average cytokine levels in the BM. Thus, T cells transport out of the BM decreases as BM trimer and cytokine levels increase. 

The cytokine equations read as follows: 

$$
\frac {d \left[ C _ {B M} \right]}{d t} = R _ {\text {s y n}} (1 - I H) - \left(k _ {\text {t r} _ {-} c y t} + k _ {\text {d e g} _ {-} c y t}\right) \left[ C _ {B M} \right] \tag {30}
$$

$$
\frac {d [ C 1 ]}{d t} = k _ {t r \_ c y t} [ C _ {B M} ] - (k _ {t r \_ c y t} + k _ {d e g \_ c y t}) [ C 1 ] \tag {31}
$$

$$
\frac {d [ C 2 ]}{d t} = k _ {t r \_ c y t} [ C 1 ] - \left(k _ {t r \_ c y t} + k _ {d e g \_ c y t}\right) [ C 2 ] \tag {32}
$$

$$
\frac {d [ C 3 ]}{d t} = k _ {t r \_ c y t} [ C 2 ] - \left(k _ {t r \_ c y t} + k _ {d e g \_ c y t}\right) [ C 3 ] \tag {33}
$$

$$
\frac {d [ C 4 ]}{d t} = k _ {t r \_ c y t} [ C 3 ] - \left(k _ {t r \_ c y t} + k _ {d e g \_ c y t}\right) [ C 4 ] \tag {34}
$$

$$
\frac {d [ C 5 ]}{d t} = k _ {t r \_ c y t} [ C 4 ] - \left(k _ {t r \_ c y t} + k _ {d e g \_ c y t}\right) [ C 5 ] \tag {35}
$$

$$
\frac {d \left[ C _ {\text {a u c}} \right]}{d t} = \left[ C _ {B M} \right] - \beta_ {\text {p r o d}} \tag {36}
$$

The terms $[ C _ { B M } ]$ to $\left[ C _ { 5 } \right]$ represent cytokine concentrations in various compartments (i.e. $[ C _ { B M } ]$ : release compartment, $\left[ C _ { 1 } \right]$ to $\left[ C _ { 5 } \right]$ : five transit compartments, $\left[ C _ { c } \right]$ : circulation compartment described in the central compartment section). 

Similar to [2] a negative feedback loop, $I H$ was incorporated by assuming inhibition on cytokine release is a function of cumulative cytokine exposure during individual dosing intervals, $C _ { a u c }$ , whereas cytokine release rate, $R _ { s y n }$ is trimer dependent. The cumulative cytokine exposure in this model is reduced (by division) at each dosing interval using a Hill equation dependent on a dose counter: 

$$
C _ {a u c, N} (0) = \frac {C _ {a u c , N - 1} (\tau)}{5 \left(1 - \frac {(N + 1) ^ {2}}{1 . 3 ^ {2} + (N + 1) ^ {2}}\right)} \tag {37}
$$

where $N$ is the number of doses and $\tau$ is the length of the dosing interval. 

Thus, the equations for cytokine release inhibition and cytokine release are given by 

$$
I H = I _ {m a x} \frac {C _ {a u c} ^ {n _ {1 C}}}{I C _ {5 0} ^ {n _ {1 C}} + C _ {a u c} ^ {n _ {1 C}}} \quad R _ {s y n} = E _ {m a x} \frac {\text {T r i m e r} ^ {n _ {2 C}}}{E C _ {5 0} ^ {n _ {2 C}} + \text {T r i m e r} ^ {n _ {2 C}}}. \tag {38}
$$

# 1.3 Description of objective function for virtual population calibration

From the plausible population, we select 120 virtual patients by using an objective function that uses the 3 metrics described below. All endpoints described are used simultaneously for model calibration and applied via a genetic algorithm (see Figure S3a for genetic algorithm flowchart). 

# 1.3.1 Best biochemical objective response

Best biochemical objective respose (BOR) is defined as the greatest decrease of percent change from baseline of integrated paraproteins (serum M-protein or FLC). We use BOR from the MM3 Cohort A trial ( $n = 1 2 0$ patients) to calibrate the BOR of the virtual populations. Let $b _ { ( i ) }$ be the ranked BOR of patients $i = 1 , \ldots , 1 2 0$ , we separatate the ranked BOR into 10 distinct groups and estimate the median BOR for each group, $b _ { g }$ for $g = 1 , \ldots , 1 0$ , as shown in Figure S6. We repeat the process with a virtual population of 120 virtual patients, $B _ { ( j ) }$ where $j = 1 , \ldots , 1 2 0$ , and the median BORs for each group is $B _ { g }$ for $g = 1 , \ldots , 1 0$ . We minimize the function: 

$$
\sum_ {g = 1} ^ {1 0} (b _ {g} - B _ {g}) ^ {2}
$$

and select the proposed virtual population (VP) such that the function above yields a value below an acceptable threshold. 

# 1.3.2 Paraprotein dynamics

We define the paraprotein dynamics for patients $i$ as the percent change from baseline in the integrated paraprotein (see Figure S4 for guideline of biomarker selection) in the form: 

$$
D _ {i, t} = \frac {x _ {i , t} - x _ {i , 0}}{x _ {i , 0}}
$$

where $x _ { i , t }$ is the value of the paraprotein at scheduled assessment $t$ , and $x _ { 0 }$ is the baseline value. We use the paraprotein dynamics from all monotherapy arms with QW dosing in both studies (MM1 and MM3 Cohort A) which results in 7 different arms. For each arm, $a = 1 , \dots , 7$ , we obtain the median percent change at each tumor assessment point, $t$ (every 3 weeks) and minimize the least squares, weighing by number of patients of each arm, $n _ { a }$ . Thus, our objective function is: 

$$
\sum_ {a = 1} ^ {7} n _ {a} \sum_ {t _ {a}} (d _ {m e d i a n, t _ {a}} - D _ {m e d i a n, t _ {a}}) ^ {2}
$$

where $d _ { m e d i a n , t _ { a } }$ is the median percent change for a proposed virtual population (simulated under similar conditions as the arm it is being compared to) at tumor assessment time $t _ { a }$ in arm $a$ . 

# 1.3.3 Biochemical response rates

Biochemical response rates (BRR) are defined as the percent of patients in each arm that had a decrease of 50% of greater from baseline and response is observed for at least two consecutive tumor assessments. This metric is similar to the objective response rates, but relies on only 

serum paraprotein responses. We used the same arms used for the paraprotein dynamics response for calibration but stratified patients by sBCMA levels at baseline (high vs low). Thus, we have up to 14 possible arms to calibrate BRR. Let $R _ { a , h }$ be the BRR for patients in arm $a = 1 , \ldots , 7$ and sBLCA group $h = 0 ( { l o w s B C M A } ) , 1 ( { h i g h s B C M A } )$ . We propose a virtual population, stratify by high/low levels of sBCMA, simulate all 7 arm schedules, and calculate BRR, $r _ { a , h }$ . We add the following term to the objective function: 

$$
\sum_ {a = 1} ^ {7} \sum_ {h = 0} ^ {1} n _ {a, h} (r _ {a, h} - R _ {a, h}) ^ {2}.
$$

# 1.4 Miscellaneous

# 1.4.1 Calculation of standardized proportion of trimers from Figure 4

We take the simulated dynamics of drug, trimer and dimer (drug-BCMA) concentration of all virtual patients accross the five simulated schedules (16 mg, 28 mg, 44 mg, 76 mg, and 152 mg QW). For each dose and each patient, we calculate the mean drug concentration. Let $T _ { i }$ and $M _ { i }$ be the average trimer and drug-BCMA dimer concentration for patient $i$ , respectively. For each dose, we calculate the ratio of trimers to BCMA bound complexes, $R _ { t r i m e r , i , d o s e }$ : 

$$
R _ {t r i m e r, i, d o s e} = \frac {\bar {T} _ {i , d o s e}}{\bar {T} _ {i , d o s e} + \bar {M} _ {i , d o s e}}
$$

We standardize the ratio accross the 5 simulated for each patient: 

$$
R _ {t r i m e r, i, d o s e} ^ {*} = \frac {R _ {t r i m e r , i , d o s e} - \operatorname* {m i n} _ {d o s e = 1 , \dots , 5} \left(R _ {t r i m e r , i , d o s e}\right)}{\operatorname* {m a x} _ {d o s e = 1 , \dots , 5} \left(R _ {t r i m e r , i , d o s e}\right)} \tag {39}
$$

Figure 4 shows the mean drug concentration plotted against $R _ { t r i m e r , i , d o s e } ^ { * }$ for 4 virtual patients. 

# Supplementary References



[1] Betts, A., Haddish-Berhane, N., Shah, D.K. et al. A Translational Quantitative Systems Pharmacology Model for CD3 Bispecific Molecules: Application to Quantify T Cell-Mediated Tumor Cell Killing by P-Cadherin LP DART. AAPS J 21, 66 (2019). 





[2] Chen, X., Kamperschroer, C., Wong, G. and Xuan, D. (2019), A Modeling Framework to Characterize Cytokine Release upon T-Cell–Engaging Bispecific Antibody Treatment: Methodology and Opportunities. Clin Transl Sci, 12: 600-608 (2019). 





[3] Friedman, K. M., Garrett, T. E., Evans, J. W., Horton, H. M., Latimer, H. J., Seidel, S. L., Horvath, C. J., & Morgan, R. A. (2018). Effective Targeting of Multiple B-Cell Maturation Antigen-Expressing Hematological Malignances by Anti-B-Cell Maturation Antigen Chimeric Antigen Receptor T Cells. Human gene therapy, 29(5), 585–601. https://doi.org/10.1089/hum.2018.001 





[4] Hokanson, J A et al. Tumor growth patterns in multiple myeloma. Cancer vol. 39,3 (1977): 1077-84. 





[5] Nicolas, L et al. Human gammadelta T cells express a higher TCR/CD3 complex density than alphabeta T cells. Clinical immunology (Orlando, Fla.) vol. 98,3 (2001): 358-63. doi:10.1006/clim.2000.4978 





[6] Oivanen T. M. Plateau phase in multiple myeloma: an analysis of long-term follow-up of 432 patients. Finnish Leukaemia Group. Br J Haematol, 1996. 92(4): p. 834-9. 





[7] Oivanen, T.M. Prognostic value of serum M-protein doubling time at escape from plateau of multiple myeloma. The Finnish Leukaemia Group. Eur J Haematol, 1996. 57(3): p. 247-53. 





[8] Ramakrishnan, V. and D.E. Mager. Pharmacodynamic Models of Differential Bortezomib Signaling Across Several Cell Lines of Multiple Myeloma. CPT: Pharmacometrics & Systems Pharmacology, 2019. 8(3): p. 146-157. 





[9] Simeoni M. et al. Predictive Pharmacokinetic-Pharmacodynamic Modeling of Tumor Growth Kinetics in Xenograft Models after Administration of Anticancer Agents. Cancer Res, 2004. 64 (3) p. 1094–1101 





[10] Nombela-Arrieta C., Manz G. M, Quantification and three-dimensional microanatomical organization of the bone marrow. Blood Adv 2017; 1 (6): 407–416. 





[11] Hassan HT, El-Sheemy M. Adult bone-marrow stem cells and their potential in medicine. J R Soc Med. 2004 Oct;97(10):465-71. 





[12] Mills, JR et al. High sensitivity blood-based M-protein detection in sCR patients with multiple myeloma. Blood Cancer J. 2017 Aug; 7(8):e590. doi: 10.1038/bcj.2017.75. PMID: 28841203; PMCID: PMC5596386 





[13] Tosi P, et al. Serum free light-chain assay for the detection and monitoring of multiple myeloma and related conditions. Ther Adv Hematol. 2013 Feb;4(1):37-41. doi: 10.1177/2040620712466863. PMID: 23610612; PMCID: PMC3629763. 





[14] Topp M., Duell J. et al, Anti–B-Cell Maturation Antigen BiTE Molecule AMG 420 Induces Responses in Multiple Myeloma. Journal of Clinical Oncology 2020 38:8, 775-783. PMID: 31895611. 





[15] Schropp, J., Khot, A., Shah, D. K., Koch, G. Target-Mediated Drug Disposition Model for Bispecific Antibodies: Properties, Approximation, and Optimal Dosing Strategy. CPT: Pharmacometrics & Systems Pharmacology, Vol. 8 No. 3, (2019). 





[16] Mager, D. Krzyzanski, W. Quasi-Equilibrium Pharmacokinetic Model for Drugs Exhibiting Target-Mediated Drug Disposition. Pharmaceutical Research, Vol. 22, No. 10, (2005) 

