# NROps_Updated

Tools for calculating current Dark Matter limits from the LUX experiment and projected limits from the LZ experiment in the framework of non-relativistic effective field theory (NREFT).

These `Mathematica` notebooks should allow you to calculate approximate limits on NREFT interactions using data from the LUX WS2014-16 and from the future LZ experiment. The limits are calculated according to the philosophy of [arXiv:1307.5955](https://arxiv.org/abs/1307.5955), using a test statistic and conversion factors to convert limits between different interactions. See [arXiv:1307.5955](https://arxiv.org/abs/1307.5955) for more explanation.

**Note that compared to [arXiv:1307.5955](https://arxiv.org/abs/1307.5955) there is one key difference.** Here, we use a different definition of the test statistic TS. For us, TS = Log_e[p], where p is the probability of obtaining fewer than the observed number of events (for a given mass and coupling of Dark Matter). **For a 90% CL, set TS = Log[0.1] and for a 95% CL, set TS = Log[0.05].**

**Version 1.1 (09/06/2017):** In the process of adding XENON1T limits. Currently only XENON1T test statistic is available. More documentation added soon.  
**Version 1.0 (03/03/2017):** Initial release. The code should work, but it may not be completely stable (and may interact with other Mathematica packages). 

Please contact Bradley Kavanagh (bradkav@gmail.com) for any comments, questions or requests.

### Usage

To load the required functions, just run the two notebooks `LUX/LUX-TS.nb` and `LZ/LZ-TS.nb`. 

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





