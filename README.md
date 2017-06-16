# NROps_Updated

Tools for calculating Dark Matter limits current and projected direct detection experiments in the framework of non-relativistic effective field theory (NREFT).

These `Mathematica` notebooks should allow you to calculate approximate limits on NREFT interactions using data from current and upcoming experiments. The limits are calculated according to the philosophy of [arXiv:1307.5955](https://arxiv.org/abs/1307.5955), using a test statistic and conversion factors to convert limits between different interactions. See [arXiv:1307.5955](https://arxiv.org/abs/1307.5955) for more explanation.

**Note that compared to [arXiv:1307.5955](https://arxiv.org/abs/1307.5955) there is one key difference.** Here, we use a different definition of the test statistic TS. For us, TS = Log_e[p], where p is the probability of obtaining fewer than the observed number of events (for a given mass and coupling of Dark Matter). **For a 90% CL, set TS = Log[0.1] and for a 95% CL, set TS = Log[0.05].**

### Version History

**Version 1.2 (16/09/2017):** New Xenon1T p-values (`TS`) and conversion factors (`Y`) added. Update to syntax, so that it looks more like the original syntax from arXiv:1307.5955.  
**Version 1.1 (09/06/2017):** In the process of adding XENON1T limits. Currently only XENON1T test statistic is available. More documentation added soon.  
**Version 1.0 (03/03/2017):** Initial release. The code should work, but it may not be completely stable (and may interact with other Mathematica packages). 

Please contact Bradley Kavanagh (bradkav@gmail.com) for any comments, questions or requests.

### Usage

To load the required functions, just run the notebooks:
 - `LUX/NRops-LUX.nb`
 - `XENON1T/NRops-Xe1T.nb`
 - `LZ/NRops-LZ.nb`.
 
 These then give you access to the following functions:
 
 `TS [exp] [Log10[mx], Log10[l]]`  
 
 `Y[interactiontype] [exp] [i, j] [N1, N2] [m]`

 where
 - interactiontype = Contact, Long-Range
 - exp = "LUX-2016", "Xe1T-2017", "LZ-projected"
 - (i, j) = Pairs of non-relativistic (NR) operactors, with i, j = 1 -> 11
 - (N1, N2) = Pairs of nucleons: ("p","p"),  ("n","n"),  ("p","n"),  ("n","p")
 - m = DM mass in GeV, in the range 5 GeV -> 10 TeV.

Examples of calculating limits are given in `Example.nb`.


### Citation

If you make use of this code, please cite the following papers:

&nbsp;&nbsp;&nbsp;&nbsp;*NROpsDD original paper*: [arXiv:1307.5955](https://arxiv.org/abs/1307.5955) [[BibTeX link](http://inspirehep.net/record/1244066/export/hx)]

**If you use the LUX WS2014-16 limits**:

&nbsp;&nbsp;&nbsp;&nbsp;*LUX WS2014-16 results paper*: [arXiv:1608.07648](https://arxiv.org/abs/1608.07648) [[BibTeX link](http://inspirehep.net/record/1484259/export/hx)]

&nbsp;&nbsp;&nbsp;&nbsp;*Procedure for calculating the LUX limits*: [arXiv:1611.05453 (Appendix B)](https://arxiv.org/abs/1611.05453) [[BibTeX link](http://inspirehep.net/record/1498519/export/hx)]

**If you use the LZ projected limits**:

&nbsp;&nbsp;&nbsp;&nbsp;*LZ Conceptual Design Report* [arXiv:1509.02910](https://arxiv.org/abs/1509.02910) [[BibTeX link](http://inspirehep.net/record/1392796/export/hx)]

&nbsp;&nbsp;&nbsp;&nbsp;*Procedure for calculating the LZ limits*: [arXiv:1605.04917 (Appendix D)](https://arxiv.org/abs/1605.04917) [[BibTeX link](http://inspirehep.net/record/1459229/export/hx)]

**Citations for Xenon1T limits to be updated soon...**



