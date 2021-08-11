# Factor-augmented-vector-autoregressive-(FAVAR)-WINRATS-code-package
### Introduction
- [*__FAVAR_TWO_STEPS_LYX__*](https://github.com/lyx66/Factor-augmented-vector-autoregressive-FAVAR-WINRATS-code-package-/blob/main/FAVAR_TWO_STEPS_LYX.zip) is the package for a *two-step estimation* method of the Factor augmented VAR (FAVAR) models, which is based on *__RATS 10.0__* . In the main code, I replicated the empirical results as in  *Bernanke et al. (2005)* ( *i.g. [Measuring the effects of monetary policy: a factor-augmented vector autoregressive (FAVAR) approach](https://academic.oup.com/qje/article-abstract/120/1/387/1931468?redirectedFrom=PDF&casa_token=ZkGknLUtMHwAAAAA:5EU8a8LgKVZAnpkuZ4F4zIIpy3EivyGD6ZuUKopeiPHjX9QmBabc_zysXUBBdpecMHXABLGc5IHB1A)* ), some of them are showed as below:
##### *Fig.1 IRF comparation: baseline (5 Factors+FFR) vs 3 Factors+FFR*
![IRF results comparation-baseline(5 factors) vs 3 factors](https://github.com/lyx66/Factor-augmented-vector-autoregressive-FAVAR-WINRATS-code-package-/blob/main/IRF%20results%20comparation-baseline(5%20factors)%20vs%203%20factors.png?raw=false)
###### *Note:* FFR (Federal funds rate) is the proxy variable of Monetary Policy and the only one observable factor in FAVAR model.
##### *Fig.2 Impluse response  to MP schock of FFR and other 19 Macroeconomic variables in Xdata (7 lags)*
![Impluse response of FRR and other 19 Macroeconomic variables in Xdata to MP schock](https://github.com/lyx66/Factor-augmented-vector-autoregressive-FAVAR-WINRATS-code-package-/blob/main/Impluse%20response%20of%20FFR%20and%20other%2019%20Macroeconomic%20variables%20in%20Xdata%20to%20MP%20schock.png?raw=false)
- __*Why I write this package?*__
</br>&emsp;&emsp;Although there has been a opensource *MATLAB* package for a Bayesian likelihood methods and Gibbs sampling estimation for FAVAR model yet, that is, the [*FAVAR*](https://drive.google.com/file/d/0BzOpR8T359fhOUY5bkh5dkM5bEU/view?resourcekey=0-MfpcA9LYIjBF3YsHYNiWRw) *MATLAB* package written by *Gary Koop*, it has the disadvantages of large time-consuming due to sampling estimation, inflexible result output process and even some bugs. In order to apply FAVAR in my own research, I have written this *RATS* code package.
- Compared with the *MATLAB* package, some superiorities of [*__FAVAR_TWO_STEPS_LYX__*](https://github.com/lyx66/Factor-augmented-vector-autoregressive-FAVAR-WINRATS-code-package-/blob/main/FAVAR_TWO_STEPS_LYX.zip) are listed as below:
</br>&emsp;1.&emsp;Less running time-comsumption.
</br>&emsp;2.&emsp;The program only needs to run once to output the impulse response with error band and variance decomposition results of all series in both [*xdata.xlsx*](https://github.com/lyx66/Factor-augmented-vector-autoregressive-FAVAR-WINRATS-code-package-/blob/main/xdata.XLSX) and [*ydata.xlsx*](https://github.com/lyx66/Factor-augmented-vector-autoregressive-FAVAR-WINRATS-code-package-/blob/main/ydata.XLSX).
</br>&emsp;3.&emsp;The result of *generalized variance decomposition* is available.
</br>&emsp;4.&emsp;Almost no bugs.
- I also provided a Python code ( *i.g.* [__*Draw IRF.ipynb*__](https://github.com/lyx66/Factor-augmented-vector-autoregressive-FAVAR-WINRATS-code-package-/blob/main/Draw%20IRF.ipynb) ) to show the IRF results in this package.
### Files in package [*__FAVAR_TWO_STEPS_LYX__*](https://github.com/lyx66/Factor-augmented-vector-autoregressive-FAVAR-WINRATS-code-package-/blob/main/FAVAR_TWO_STEPS_LYX.zip)
- Main code.rpf
- verd_lyx.src&emsp;&emsp;&emsp;&ensp;- get variance matrix of forecast error
- mcgraphirf_lyx.src&ensp;- get median value and error band of IRF
- kilianbootsetup.src - *two-stages boostrap* for IRF error band ( [*Kilian, 1998*](https://direct.mit.edu/rest/article-abstract/80/2/218/57059) )
### Enviroment
- FAVAR model: *Windows RATS 10.0*
- Graph for IRF: *Python 3.8*
### Files loaded
#### Two __*'.xlsx'*__ files loaded by main code are listed as below:
File|# of series|Details
:-|:-:|:-
[*ydata.xlsx*](https://github.com/lyx66/Factor-augmented-vector-autoregressive-FAVAR-WINRATS-code-package-/blob/main/ydata.XLSX)|1|The proxy variable of monetary policy, that is, the only one observable factor in FAVAR model
[*xdata.xlsx*](https://github.com/lyx66/Factor-augmented-vector-autoregressive-FAVAR-WINRATS-code-package-/blob/main/xdata.XLSX)|119|Macroeconomic data sets, containing information on real-output, employment, interest rate, exchange rate, price level and financial asset price, etc.
###### *Data source: [Measuring the effects of monetary policy: a factor-augmented vector autoregressive (FAVAR) approach](https://academic.oup.com/qje/article-abstract/120/1/387/1931468?redirectedFrom=PDF&casa_token=ZkGknLUtMHwAAAAA:5EU8a8LgKVZAnpkuZ4F4zIIpy3EivyGD6ZuUKopeiPHjX9QmBabc_zysXUBBdpecMHXABLGc5IHB1A)*
### Outputs
- The result of IRF with error bands   :  [*IRF_FAVAR.xlsx*](https://github.com/lyx66/Factor-augmented-vector-autoregressive-FAVAR-WINRATS-code-package-/blob/main/IRF_FAVAR.xlsx)
- The result of variance decomposition :  [*VD_FAVAR.xlsx*](https://github.com/lyx66/Factor-augmented-vector-autoregressive-FAVAR-WINRATS-code-package-/blob/main/DV_FAVAR.xlsx)
### Copyright notice
- AUTHOR: __*Yingxin LIN*__
- Company: *Prof.[__Yi FAN__](http://sf.cufe.edu.cn/info/1112/10555.htm)'s workshop, School of Finance, Central University of Finance and Economics* (CUFE)
- Contact: lyxurthebest@163.com or lyxurthebest@outlook.com
- The copyright belongs to __*Yingxin LIN*__ , 2021/08/12.
#### *Enjoy*（。＾▽＾) *! (...and extend/modify)* 😊
