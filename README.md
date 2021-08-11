# Factor-augmented-vector-autoregressive-(FAVAR)-WINRATS-code-package
### Introduction
- *__FAVAR_TWO_STEPS_LYX__* is the package for a *two-step estimation* method of the Factor augmented VAR (FAVAR) models, which is based on *__RATS 10.0__* . In the main code, I replicated the empirical results as in  *Bernanke et al. (2005)* ( *i.g. [Measuring the effects of monetary policy: a factor-augmented vector autoregressive (FAVAR) approach](https://academic.oup.com/qje/article-abstract/120/1/387/1931468?redirectedFrom=PDF&casa_token=ZkGknLUtMHwAAAAA:5EU8a8LgKVZAnpkuZ4F4zIIpy3EivyGD6ZuUKopeiPHjX9QmBabc_zysXUBBdpecMHXABLGc5IHB1A)* ).
- Although there has been a opensource *MATLAB* package for a Bayesian likelihood methods and Gibbs sampling estimation for FAVAR model, that is, the [*FAVAR*](https://drive.google.com/file/d/0BzOpR8T359fhOUY5bkh5dkM5bEU/view?resourcekey=0-MfpcA9LYIjBF3YsHYNiWRw) *MATLAB* package written by *Gary Koop*, it has the disadvantages of large time-consuming due to sampling estimation, inflexible result output process and even some bugs. In order to apply FAVAR in my own research, I have written this *RATS* code package.
- Compared with the *MATLAB* package, some <span style="border-bottom:2px;">superiorities</span> of *__FAVAR_TWO_STEPS_LYX__* are listed as below:
1. 
### Files loaded
#### Two __*'.xlsx'*__ files loaded by main code are listed as below:
File|# of series|Details
:-|:-:|:-
[*ydata.xlsx*](https://github.com/lyx66/Factor-augmented-vector-autoregressive-FAVAR-WINRATS-code-package-/blob/main/ydata.XLSX)|1|The proxy variable of monetary policy, that is, the only one observer factor in FAVAR model
[*xdata.xlsx*](https://github.com/lyx66/Factor-augmented-vector-autoregressive-FAVAR-WINRATS-code-package-/blob/main/xdata.XLSX)|119|Macroeconomic data sets, containing information on real-output, employment, interest rate, exchange rate, price level and financial asset price, etc.
###### *Data source: [Measuring the effects of monetary policy: a factor-augmented vector autoregressive (FAVAR) approach](https://academic.oup.com/qje/article-abstract/120/1/387/1931468?redirectedFrom=PDF&casa_token=ZkGknLUtMHwAAAAA:5EU8a8LgKVZAnpkuZ4F4zIIpy3EivyGD6ZuUKopeiPHjX9QmBabc_zysXUBBdpecMHXABLGc5IHB1A)*
### Copyright notice
- AUTHOR: __*Yingxin LIN*__
- Company: *Prof.[__Yi FAN__](http://sf.cufe.edu.cn/info/1112/10555.htm)'s workshop, School of Finance, Central University of Finance and Economics* (CUFE)
- Contact: lyxurthebest@163.com or lyxurthebest@outlook.com
- The copyright belongs to __*Yingxin LIN*__ , 2021/08/11.
#### *Enjoy*（。＾▽＾) *! (...and extend/modify)* 😊
