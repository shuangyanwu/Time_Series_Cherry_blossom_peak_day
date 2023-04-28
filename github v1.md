Show in New Window
New names:
• `` -> `...23`
• `` -> `...24`
R Console


Show in New Window

Show in New Window

Show in New Window

Show in New Window
 Error: 'MERGED2015_16_PP.csv' does not exist in current working directory ('/Users/wushuangyan/Desktop/STAT classes/Finished/STAT 6365E Programming/Working Directory').
                                   0.18198992 
relevel(factor(data9$year), ref = "1961")1982 
                                  -3.48467675 
relevel(factor(data9$year), ref = "1961")1983 
                                  -0.27255554 
relevel(factor(data9$year), ref = "1961")1984 
                                   9.94966668 
relevel(factor(data9$year), ref = "1961")1985 
                                   1.02037375 
relevel(factor(data9$year), ref = "1961")1986 
                                   1.76784850 
relevel(factor(data9$year), ref = "1961")1987 
                                  -0.69679796 
relevel(factor(data9$year), ref = "1961")1988 
                                   4.93042176 
relevel(factor(data9$year), ref = "1961")1989 
                                  -5.46447473 
relevel(factor(data9$year), ref = "1961")1990 
                                  -7.31295958 
relevel(factor(data9$year), ref = "1961")1991 
                                   0.04057577 
relevel(factor(data9$year), ref = "1961")1992 
                                  -1.35336362 
relevel(factor(data9$year), ref = "1961")1993 
                                   1.72116168 
relevel(factor(data9$year), ref = "1961")1994 
                                   0.45446944 
relevel(factor(data9$year), ref = "1961")1995 
                                   1.57809380 
relevel(factor(data9$year), ref = "1961")1996 
                                   3.60048681 
relevel(factor(data9$year), ref = "1961")1997 
                                  -3.20563564 
relevel(factor(data9$year), ref = "1961")1998 
                                  -4.93879642 
relevel(factor(data9$year), ref = "1961")1999 
                                  -1.76651323 
relevel(factor(data9$year), ref = "1961")2000 
                                   2.32337227 
relevel(factor(data9$year), ref = "1961")2001 
                                  -2.66868711 
relevel(factor(data9$year), ref = "1961")2002 
                                 -10.25407739 
relevel(factor(data9$year), ref = "1961")2003 
                                  -2.77056198 
relevel(factor(data9$year), ref = "1961")2004 
                                  -3.38346520 
relevel(factor(data9$year), ref = "1961")2005 
                                   3.03600689 
relevel(factor(data9$year), ref = "1961")2006 
                                  -1.30104259 
relevel(factor(data9$year), ref = "1961")2007 
                                  -1.01913593 
relevel(factor(data9$year), ref = "1961")2008 
                                  -3.34017577 
relevel(factor(data9$year), ref = "1961")2009 
                                  -3.71949421 
relevel(factor(data9$year), ref = "1961")2010 
                                  -1.55124800 
relevel(factor(data9$year), ref = "1961")2011 
                                   1.49835149 
relevel(factor(data9$year), ref = "1961")2012 
                                   1.51501816 
relevel(factor(data9$year), ref = "1961")2013 
                                  -5.13883554 
relevel(factor(data9$year), ref = "1961")2014 
                                  -5.12188638 
relevel(factor(data9$year), ref = "1961")2015 
                                  -6.27442876 
relevel(factor(data9$year), ref = "1961")2016 
                                  -2.29137791 
relevel(factor(data9$year), ref = "1961")2017 
                                   0.91201192 
relevel(factor(data9$year), ref = "1961")2018 
                                  -8.24053045 
relevel(factor(data9$year), ref = "1961")2019 
                                  -2.45561699 
relevel(factor(data9$year), ref = "1961")2020 
                                  -3.67552839 
relevel(factor(data9$year), ref = "1961")2021 
                                  -9.58667182 
> sum(a>=0)
[1] 49
> sum(a<=0)
[1] 49
> sum(b>=0)
[1] 34
> sum(b<=0)
[1] 34
> #### time series
> ## Japan/Kyoto
> library('astsa')
> data99<-data9[data9$Location=="Japan/Kyoto",]; data99 # data for Japan/Kyoto only
# A tibble: 69 × 6
# Groups:   Location [1]
   Location      lat  long   alt year  Fbloom_doy
   <chr>       <dbl> <dbl> <dbl> <chr>      <dbl>
 1 Japan/Kyoto  35.0  136.  40.8 1953         101
 2 Japan/Kyoto  35.0  136.  40.8 1954          95
 3 Japan/Kyoto  35.0  136.  40.8 1955          97
 4 Japan/Kyoto  35.0  136.  40.8 1956         101
 5 Japan/Kyoto  35.0  136.  40.8 1959          92
 6 Japan/Kyoto  35.0  136.  40.8 1966          96
 7 Japan/Kyoto  35.0  136.  40.8 1968          96
 8 Japan/Kyoto  35.0  136.  40.8 1969         103
 9 Japan/Kyoto  35.0  136.  40.8 1970         105
10 Japan/Kyoto  35.0  136.  40.8 1971          97
# … with 59 more rows
> kyoto <- ts(data99$Fbloom_doy,start=c(1953,1),frequency=1);kyoto_ts
Error: object 'kyoto_ts' not found
> plot(kyoto_Full_bloom_day)
Error in plot(kyoto_Full_bloom_day) : 
  object 'kyoto_Full_bloom_day' not found
> acf2(kyoto_Full_bloom_day)
Error in acf2(kyoto_Full_bloom_day) : 
  object 'kyoto_Full_bloom_day' not found
> kyoto1 = diff(kyoto_Full_bloom_day) #differenced
Error in diff(kyoto_Full_bloom_day) : 
  object 'kyoto_Full_bloom_day' not found
> plot(diff(kyoto_Full_bloom_day))
Error in diff(kyoto_Full_bloom_day) : 
  object 'kyoto_Full_bloom_day' not found
> #### time series
> ## Japan/Kyoto
> library('astsa')
> data99<-data9[data9$Location=="Japan/Kyoto",]; data99 # data for Japan/Kyoto only
# A tibble: 69 × 6
# Groups:   Location [1]
   Location      lat  long   alt year  Fbloom_doy
   <chr>       <dbl> <dbl> <dbl> <chr>      <dbl>
 1 Japan/Kyoto  35.0  136.  40.8 1953         101
 2 Japan/Kyoto  35.0  136.  40.8 1954          95
 3 Japan/Kyoto  35.0  136.  40.8 1955          97
 4 Japan/Kyoto  35.0  136.  40.8 1956         101
 5 Japan/Kyoto  35.0  136.  40.8 1959          92
 6 Japan/Kyoto  35.0  136.  40.8 1966          96
 7 Japan/Kyoto  35.0  136.  40.8 1968          96
 8 Japan/Kyoto  35.0  136.  40.8 1969         103
 9 Japan/Kyoto  35.0  136.  40.8 1970         105
10 Japan/Kyoto  35.0  136.  40.8 1971          97
# … with 59 more rows
> kyoto <- ts(data99$Fbloom_doy,start=c(1953,1),frequency=1);kyoto_ts
Error: object 'kyoto_ts' not found
> plot(kyoto_Full_bloom_day)
Error in plot(kyoto_Full_bloom_day) : 
  object 'kyoto_Full_bloom_day' not found
> acf2(kyoto_Full_bloom_day)
Error in acf2(kyoto_Full_bloom_day) : 
  object 'kyoto_Full_bloom_day' not found
> kyoto <- ts(data99$Fbloom_doy,start=c(1953,1),frequency=1);kyoto_ts
Error: object 'kyoto_ts' not found
> plot (mean$mean~mean$year,col="red",lwd=2, xlab="Year", 
+       ylab="Mean of full bloom date", main="Mean of Fbloom day vs Year",pch = 19,cex=0.6,
+       cex.axis = 1.1, cex.lab = 1.2,font.lab=2)
Error in mean$mean : object of type 'closure' is not subsettable
> #### time series
> ## Japan/Kyoto
> library('astsa')
> data99<-data9[data9$Location=="Japan/Kyoto",]; data99 # data for Japan/Kyoto only
# A tibble: 69 × 6
# Groups:   Location [1]
   Location      lat  long   alt year  Fbloom_doy
   <chr>       <dbl> <dbl> <dbl> <chr>      <dbl>
 1 Japan/Kyoto  35.0  136.  40.8 1953         101
 2 Japan/Kyoto  35.0  136.  40.8 1954          95
 3 Japan/Kyoto  35.0  136.  40.8 1955          97
 4 Japan/Kyoto  35.0  136.  40.8 1956         101
 5 Japan/Kyoto  35.0  136.  40.8 1959          92
 6 Japan/Kyoto  35.0  136.  40.8 1966          96
 7 Japan/Kyoto  35.0  136.  40.8 1968          96
 8 Japan/Kyoto  35.0  136.  40.8 1969         103
 9 Japan/Kyoto  35.0  136.  40.8 1970         105
10 Japan/Kyoto  35.0  136.  40.8 1971          97
# … with 59 more rows
> kyoto <- ts(data99$Fbloom_doy,start=c(1953,1),frequency=1);kyoto_ts
Error: object 'kyoto_ts' not found
> kyoto_ts
Error: object 'kyoto_ts' not found
> kyoto_ts <- ts(data99$Fbloom_doy,start=c(1953,1),frequency=1);kyoto_ts
Time Series:
Start = 1953 
End = 2021 
Frequency = 1 
 [1] 101  95  97 101  92  96  96 103 105  97  98  98  99 100 100  93 103  99  99  98  90  99 105  98
[25]  98  96 102  92  88  96  94  96  96  96 100  94  91  92 101  93  87  94  94  98  96  93  92  95
[49]  91  97 100  89  92  91  93  97  87  96  90  85 102  98  96  96  97  99  97 107  96
> plot(kyoto_Full_bloom_day)
Error in plot(kyoto_Full_bloom_day) : 
  object 'kyoto_Full_bloom_day' not found
> acf2(kyoto_Full_bloom_day)
Error in acf2(kyoto_Full_bloom_day) : 
  object 'kyoto_Full_bloom_day' not found
> data99<-data9[data9$Location=="Japan/Kyoto",]; data99 # data for Japan/Kyoto only
# A tibble: 69 × 6
# Groups:   Location [1]
   Location      lat  long   alt year  Fbloom_doy
   <chr>       <dbl> <dbl> <dbl> <chr>      <dbl>
 1 Japan/Kyoto  35.0  136.  40.8 1953         101
 2 Japan/Kyoto  35.0  136.  40.8 1954          95
 3 Japan/Kyoto  35.0  136.  40.8 1955          97
 4 Japan/Kyoto  35.0  136.  40.8 1956         101
 5 Japan/Kyoto  35.0  136.  40.8 1959          92
 6 Japan/Kyoto  35.0  136.  40.8 1966          96
 7 Japan/Kyoto  35.0  136.  40.8 1968          96
 8 Japan/Kyoto  35.0  136.  40.8 1969         103
 9 Japan/Kyoto  35.0  136.  40.8 1970         105
10 Japan/Kyoto  35.0  136.  40.8 1971          97
# … with 59 more rows
> kyoto_ts <- ts(data99$Fbloom_doy,start=c(1953,1),frequency=1);kyoto_ts
Time Series:
Start = 1953 
End = 2021 
Frequency = 1 
 [1] 101  95  97 101  92  96  96 103 105  97  98  98  99 100 100  93 103  99  99  98  90  99 105  98
[25]  98  96 102  92  88  96  94  96  96  96 100  94  91  92 101  93  87  94  94  98  96  93  92  95
[49]  91  97 100  89  92  91  93  97  87  96  90  85 102  98  96  96  97  99  97 107  96
> plot(kyoto_Full_bloom_day)
Error in plot(kyoto_Full_bloom_day) : 
  object 'kyoto_Full_bloom_day' not found
> kyoto <- ts(data99$Fbloom_doy,start=c(1953,1),frequency=1);kyoto_ts
Time Series:
Start = 1953 
End = 2021 
Frequency = 1 
 [1] 101  95  97 101  92  96  96 103 105  97  98  98  99 100 100  93 103  99  99  98  90  99 105  98
[25]  98  96 102  92  88  96  94  96  96  96 100  94  91  92 101  93  87  94  94  98  96  93  92  95
[49]  91  97 100  89  92  91  93  97  87  96  90  85 102  98  96  96  97  99  97 107  96
> plot(kyoto_Full_bloom_day)
Error in plot(kyoto_Full_bloom_day) : 
  object 'kyoto_Full_bloom_day' not found
> plot(kyoto_ts)
> acf2(kyoto_Full_bloom_day)
Error in acf2(kyoto_Full_bloom_day) : 
  object 'kyoto_Full_bloom_day' not found
> kyoto_Full_bloom_day <- ts(data99$Fbloom_doy,start=c(1953,1),frequency=1);kyoto_ts
Time Series:
Start = 1953 
End = 2021 
Frequency = 1 
 [1] 101  95  97 101  92  96  96 103 105  97  98  98  99 100 100  93 103  99  99  98  90  99 105  98
[25]  98  96 102  92  88  96  94  96  96  96 100  94  91  92 101  93  87  94  94  98  96  93  92  95
[49]  91  97 100  89  92  91  93  97  87  96  90  85 102  98  96  96  97  99  97 107  96
> plot(kyoto_Full_bloom_day)
> acf2(kyoto_Full_bloom_day)
     [,1] [,2] [,3] [,4] [,5]  [,6] [,7]  [,8] [,9] [,10] [,11] [,12] [,13] [,14] [,15] [,16] [,17]
ACF  0.17 0.03 0.21 0.09 0.31  0.07 0.13  0.15 0.01  0.09  0.08  0.13  0.04 -0.04 -0.02  0.11  0.08
PACF 0.17 0.00 0.21 0.03 0.32 -0.07 0.16 -0.03 0.00 -0.06  0.06  0.05 -0.04 -0.05 -0.10  0.13 -0.02
     [,18] [,19]
ACF  -0.02  0.02
PACF  0.01 -0.01
> kyoto1 = diff(kyoto_Full_bloom_day) #differenced
> plot(diff(kyoto_Full_bloom_day))
> acf2(diff(kyoto_Full_bloom_day))
      [,1]  [,2]  [,3]  [,4] [,5]  [,6]  [,7]  [,8]  [,9] [,10] [,11] [,12] [,13] [,14] [,15] [,16]
ACF  -0.41 -0.19  0.17 -0.19 0.27 -0.18  0.00  0.09 -0.12  0.05 -0.04  0.08 -0.01 -0.06 -0.06  0.08
PACF -0.41 -0.43 -0.18 -0.39 0.03 -0.19 -0.02 -0.06 -0.03 -0.13 -0.11 -0.01  0.00  0.03 -0.16 -0.04
     [,17] [,18] [,19]
ACF   0.05 -0.09  0.11
PACF -0.06 -0.05  0.09
> (obj=sarima(kyoto, p=0, d=1, q=1, P = 0, D = 0, Q = 0, S = 0))
initial  value 1.743020 
iter   2 value 1.590336
iter   3 value 1.559790
iter   4 value 1.512694
iter   5 value 1.498316
iter   6 value 1.480461
iter   7 value 1.480072
iter   8 value 1.476885
iter   9 value 1.476560
iter  10 value 1.476280
iter  11 value 1.476271
iter  11 value 1.476271
final  value 1.476271 
converged
initial  value 1.475253 
iter   2 value 1.474680
iter   3 value 1.474676
iter   4 value 1.474672
iter   5 value 1.474672
iter   5 value 1.474672
iter   5 value 1.474672
final  value 1.474672 
converged
$fit

Call:
arima(x = xdata, order = c(p, d, q), seasonal = list(order = c(P, D, Q), period = S), 
    xreg = constant, transform.pars = trans, fixed = fixed, optim.control = list(trace = trc, 
        REPORT = 1, reltol = tol))

Coefficients:
          ma1  constant
      -0.8631   -0.0190
s.e.   0.0752    0.0833

sigma^2 estimated as 18.71:  log likelihood = -196.77,  aic = 399.53

$degrees_of_freedom
[1] 66

$ttable
         Estimate     SE  t.value p.value
ma1       -0.8631 0.0752 -11.4792  0.0000
constant  -0.0190 0.0833  -0.2276  0.8207

$AIC
[1] 5.875457

$AICc
[1] 5.878172

$BIC
[1] 5.973376

> (obj=sarima(kyoto, p=4, d=1, q=0, P = 0, D = 0, Q = 0, S = 0))
initial  value 1.741805 
iter   2 value 1.594998
iter   3 value 1.506595
iter   4 value 1.496358
iter   5 value 1.447610
iter   6 value 1.423254
iter   7 value 1.419038
iter   8 value 1.419005
iter   9 value 1.418438
iter  10 value 1.418436
iter  11 value 1.418434
iter  12 value 1.418434
iter  12 value 1.418434
final  value 1.418434 
converged
initial  value 1.425519 
iter   2 value 1.425401
iter   3 value 1.424776
iter   4 value 1.424701
iter   5 value 1.424673
iter   6 value 1.424660
iter   7 value 1.424659
iter   7 value 1.424659
iter   7 value 1.424659
final  value 1.424659 
converged
$fit

Call:
arima(x = xdata, order = c(p, d, q), seasonal = list(order = c(P, D, Q), period = S), 
    xreg = constant, transform.pars = trans, fixed = fixed, optim.control = list(trace = trc, 
        REPORT = 1, reltol = tol))

Coefficients:
          ar1      ar2      ar3      ar4  constant
      -0.7693  -0.8003  -0.4648  -0.4331    0.0243
s.e.   0.1107   0.1336   0.1319   0.1123    0.1472

sigma^2 estimated as 16.88:  log likelihood = -193.36,  aic = 398.73

$degrees_of_freedom
[1] 63

$ttable
         Estimate     SE t.value p.value
ar1       -0.7693 0.1107 -6.9506  0.0000
ar2       -0.8003 0.1336 -5.9921  0.0000
ar3       -0.4648 0.1319 -3.5249  0.0008
ar4       -0.4331 0.1123 -3.8548  0.0003
constant   0.0243 0.1472  0.1652  0.8693

$AIC
[1] 5.863666

$AICc
[1] 5.877897

$BIC
[1] 6.059505

> (obj=sarima(kyoto, p=1, d=1, q=2, P = 0, D = 0, Q = 0, S = 0))
initial  value 1.742456 
iter   2 value 1.503325
iter   3 value 1.489944
iter   4 value 1.475944
iter   5 value 1.465133
iter   6 value 1.464313
iter   7 value 1.463549
iter   8 value 1.462132
iter   9 value 1.461946
iter  10 value 1.460843
iter  11 value 1.460830
iter  12 value 1.455811
iter  13 value 1.455726
iter  14 value 1.453942
iter  15 value 1.449144
iter  16 value 1.447122
iter  17 value 1.445706
iter  18 value 1.444780
iter  19 value 1.444498
iter  20 value 1.442396
iter  21 value 1.422598
iter  22 value 1.422551
iter  23 value 1.413297
iter  24 value 1.407516
iter  25 value 1.400379
iter  25 value 1.400379
iter  26 value 1.393815
iter  27 value 1.393811
iter  28 value 1.392843
iter  29 value 1.392691
iter  30 value 1.392177
iter  31 value 1.392001
iter  32 value 1.391580
iter  33 value 1.391424
iter  34 value 1.390999
iter  35 value 1.390882
iter  36 value 1.390424
iter  37 value 1.390355
iter  38 value 1.389851
iter  39 value 1.389835
iter  40 value 1.389281
iter  41 value 1.389216
iter  42 value 1.389157
iter  43 value 1.389149
iter  44 value 1.388601
iter  45 value 1.388534
iter  46 value 1.388484
iter  47 value 1.388402
iter  48 value 1.388371
iter  49 value 1.388288
iter  50 value 1.388258
iter  51 value 1.388176
iter  52 value 1.388145
iter  53 value 1.388064
iter  54 value 1.388032
iter  55 value 1.387952
iter  56 value 1.387920
iter  57 value 1.387840
iter  58 value 1.387807
iter  59 value 1.387728
iter  60 value 1.387695
iter  61 value 1.387617
iter  62 value 1.387583
iter  63 value 1.387505
iter  64 value 1.387471
iter  65 value 1.387394
iter  66 value 1.387360
iter  67 value 1.387283
iter  68 value 1.387248
iter  69 value 1.387172
iter  70 value 1.387137
iter  71 value 1.387062
iter  72 value 1.387026
iter  73 value 1.386951
iter  74 value 1.386915
iter  75 value 1.386841
iter  76 value 1.386804
iter  77 value 1.386731
iter  78 value 1.386694
iter  79 value 1.386622
iter  80 value 1.386583
iter  81 value 1.386512
iter  82 value 1.386473
iter  83 value 1.386403
iter  84 value 1.386363
iter  85 value 1.386294
iter  86 value 1.386254
iter  87 value 1.386185
iter  88 value 1.386144
iter  89 value 1.386076
iter  90 value 1.386035
iter  91 value 1.385968
iter  92 value 1.385926
iter  93 value 1.385859
iter  94 value 1.385817
iter  95 value 1.385751
iter  96 value 1.385709
iter  97 value 1.385643
iter  98 value 1.385600
iter  99 value 1.385536
iter 100 value 1.385492
final  value 1.385492 
stopped after 100 iterations
initial  value 1.743020 
iter   2 value 1.506353
iter   3 value 1.497995
iter   4 value 1.494973
iter   5 value 1.469210
iter   6 value 1.468325
iter   7 value 1.467306
iter   8 value 1.464344
iter   9 value 1.461990
iter  10 value 1.461882
iter  11 value 1.459370
iter  12 value 1.444444
iter  13 value 1.442543
iter  14 value 1.438858
iter  15 value 1.438510
iter  16 value 1.438428
iter  17 value 1.438426
iter  18 value 1.438425
iter  18 value 1.438425
final  value 1.438425 
converged
$fit

Call:
arima(x = xdata, order = c(p, d, q), seasonal = list(order = c(P, D, Q), period = S), 
    xreg = constant, transform.pars = trans, fixed = fixed, optim.control = list(trace = trc, 
        REPORT = 1, reltol = tol))

Coefficients:
          ar1      ma1      ma2  constant
      -0.6752  -0.0113  -0.8061   -0.0363
s.e.   0.1548   0.1312   0.1028    0.0718

sigma^2 estimated as 17.29:  log likelihood = -194.3,  aic = 398.6

$degrees_of_freedom
[1] 64

$ttable
         Estimate     SE t.value p.value
ar1       -0.6752 0.1548 -4.3618  0.0000
ma1       -0.0113 0.1312 -0.0860  0.9318
ma2       -0.8061 0.1028 -7.8386  0.0000
constant  -0.0363 0.0718 -0.5060  0.6146

$AIC
[1] 5.861787

$AICc
[1] 5.871124

$BIC
[1] 6.024986

> (obj=sarima(kyoto, p=4, d=1, q=0, P = 0, D = 0, Q = 0, S = 0))
initial  value 1.741805 
iter   2 value 1.594998
iter   3 value 1.506595
iter   4 value 1.496358
iter   5 value 1.447610
iter   6 value 1.423254
iter   7 value 1.419038
iter   8 value 1.419005
iter   9 value 1.418438
iter  10 value 1.418436
iter  11 value 1.418434
iter  12 value 1.418434
iter  12 value 1.418434
final  value 1.418434 
converged
initial  value 1.425519 
iter   2 value 1.425401
iter   3 value 1.424776
iter   4 value 1.424701
iter   5 value 1.424673
iter   6 value 1.424660
iter   7 value 1.424659
iter   7 value 1.424659
iter   7 value 1.424659
final  value 1.424659 
converged
$fit

Call:
arima(x = xdata, order = c(p, d, q), seasonal = list(order = c(P, D, Q), period = S), 
    xreg = constant, transform.pars = trans, fixed = fixed, optim.control = list(trace = trc, 
        REPORT = 1, reltol = tol))

Coefficients:
          ar1      ar2      ar3      ar4  constant
      -0.7693  -0.8003  -0.4648  -0.4331    0.0243
s.e.   0.1107   0.1336   0.1319   0.1123    0.1472

sigma^2 estimated as 16.88:  log likelihood = -193.36,  aic = 398.73

$degrees_of_freedom
[1] 63

$ttable
         Estimate     SE t.value p.value
ar1       -0.7693 0.1107 -6.9506  0.0000
ar2       -0.8003 0.1336 -5.9921  0.0000
ar3       -0.4648 0.1319 -3.5249  0.0008
ar4       -0.4331 0.1123 -3.8548  0.0003
constant   0.0243 0.1472  0.1652  0.8693

$AIC
[1] 5.863666

$AICc
[1] 5.877897

$BIC
[1] 6.059505

> plot(kyoto_Full_bloom_day)
> kyoto_Full_bloom_day<-kyoto
> sarima.for(kyoto_Full_bloom_day, n.ahead=1, p=0,d=1,q=1, P=0,D=0,Q=0,S=0)
$pred
Time Series:
Start = 2022 
End = 2022 
Frequency = 1 
[1] 96.85446

$se
Time Series:
Start = 2022 
End = 2022 
Frequency = 1 
[1] 4.325923

> sarima.for(kyoto, n.ahead=5, p=4,d=1,q=0, P=0,D=0,Q=0,S=0)
$pred
Time Series:
Start = 2022 
End = 2026 
Frequency = 1 
[1]  96.60651 101.24567  98.05813 101.36370  99.03715

$se
Time Series:
Start = 2022 
End = 2026 
Frequency = 1 
[1] 4.108344 4.216291 4.217276 4.434190 4.499137

> sarima.for(kyoto, n.ahead=5, p=1,d=1,q=2, P=0,D=0,Q=0,S=0)
$pred
Time Series:
Start = 2022 
End = 2026 
Frequency = 1 
[1] 93.84947 97.07338 94.83561 96.28577 95.24570

$se
Time Series:
Start = 2022 
End = 2026 
Frequency = 1 
[1] 4.158091 4.357615 4.359289 4.439658 4.443787

> sarima.for(kyoto, n.ahead=5, p=4,d=1,q=0, P=0,D=0,Q=0,S=0)
$pred
Time Series:
Start = 2022 
End = 2026 
Frequency = 1 
[1]  96.60651 101.24567  98.05813 101.36370  99.03715

$se
Time Series:
Start = 2022 
End = 2026 
Frequency = 1 
[1] 4.108344 4.216291 4.217276 4.434190 4.499137

> ## Historical data
> data13<-data9[data9$Location=="Japan/Kyoto",]; data99 # data for Japan/Kyoto only
# A tibble: 69 × 6
# Groups:   Location [1]
   Location      lat  long   alt year  Fbloom_doy
   <chr>       <dbl> <dbl> <dbl> <chr>      <dbl>
 1 Japan/Kyoto  35.0  136.  40.8 1953         101
 2 Japan/Kyoto  35.0  136.  40.8 1954          95
 3 Japan/Kyoto  35.0  136.  40.8 1955          97
 4 Japan/Kyoto  35.0  136.  40.8 1956         101
 5 Japan/Kyoto  35.0  136.  40.8 1959          92
 6 Japan/Kyoto  35.0  136.  40.8 1966          96
 7 Japan/Kyoto  35.0  136.  40.8 1968          96
 8 Japan/Kyoto  35.0  136.  40.8 1969         103
 9 Japan/Kyoto  35.0  136.  40.8 1970         105
10 Japan/Kyoto  35.0  136.  40.8 1971          97
# … with 59 more rows
> kyoto <- ts(data99$Fbloom_doy,start=c(1953,1),frequency=1);kyoto_ts
Time Series:
Start = 1953 
End = 2021 
Frequency = 1 
 [1] 101  95  97 101  92  96  96 103 105  97  98  98  99 100 100  93 103  99  99  98  90  99 105  98
[25]  98  96 102  92  88  96  94  96  96  96 100  94  91  92 101  93  87  94  94  98  96  93  92  95
[49]  91  97 100  89  92  91  93  97  87  96  90  85 102  98  96  96  97  99  97 107  96
> plot(kyoto)
> acf2(kyoto)
     [,1] [,2] [,3] [,4] [,5]  [,6] [,7]  [,8] [,9] [,10] [,11] [,12] [,13] [,14] [,15] [,16] [,17]
ACF  0.17 0.03 0.21 0.09 0.31  0.07 0.13  0.15 0.01  0.09  0.08  0.13  0.04 -0.04 -0.02  0.11  0.08
PACF 0.17 0.00 0.21 0.03 0.32 -0.07 0.16 -0.03 0.00 -0.06  0.06  0.05 -0.04 -0.05 -0.10  0.13 -0.02
     [,18] [,19]
ACF  -0.02  0.02
PACF  0.01 -0.01
> ?ifelse
> kyoto1 = diff(kyoto) #differenced
> plot(diff(kyoto))
> acf2(kyoto1)
      [,1]  [,2]  [,3]  [,4] [,5]  [,6]  [,7]  [,8]  [,9] [,10] [,11] [,12] [,13] [,14] [,15] [,16]
ACF  -0.41 -0.19  0.17 -0.19 0.27 -0.18  0.00  0.09 -0.12  0.05 -0.04  0.08 -0.01 -0.06 -0.06  0.08
PACF -0.41 -0.43 -0.18 -0.39 0.03 -0.19 -0.02 -0.06 -0.03 -0.13 -0.11 -0.01  0.00  0.03 -0.16 -0.04
     [,17] [,18] [,19]
ACF   0.05 -0.09  0.11
PACF -0.06 -0.05  0.09
> datanm<-data6 [misspercent==0,]; datanm
# A tibble: 41 × 73
# Groups:   Location [41]
   Location       lat  long   alt `1953` `1954` `1955` `1956` `1959` `1966` `1968` `1969` `1970` `1971`
   <chr>        <dbl> <dbl> <dbl>  <dbl>  <dbl>  <dbl>  <dbl>  <dbl>  <dbl>  <dbl>  <dbl>  <dbl>  <dbl>
 1 Japan/Akita   39.7  140.   6.3    119    112    113    117    107    115    115    119    121    119
 2 Japan/Asahi…  43.8  142. 120.     136    138    134    134    133    138    126    129    130    135
 3 Japan/Choshi  35.7  141.  20.1     95     95     94    102     92     95     95    101    107     98
 4 Japan/Fukui   36.1  136.   8.8    102     96     99    105     94     99    102    103    109    103
 5 Japan/Fukus…  37.8  140.  67.4    101     99    101    107     98    104    102    104    111    104
 6 Japan/Gifu    35.4  137.  12.7     99     95     91     98     93     96    100    101    105     97
 7 Japan/Hakod…  41.8  141.  35      129    127    134    129    122    131    128    128    131    134
 8 Japan/Hikone  35.3  136.  87.3    102     97     98    103     95    103    104    104    108    100
 9 Japan/Hiros…  34.4  132.   3.6    101     96     96    102     93     97     98    103    104     97
10 Japan/Kagos…  31.6  131.   3.9     98     98     93     93     89     86     95     97     97     93
# … with 31 more rows, and 59 more variables: `1972` <dbl>, `1973` <dbl>, `1974` <dbl>, `1975` <dbl>,
#   `1976` <dbl>, `1977` <dbl>, `1978` <dbl>, `1979` <dbl>, `1980` <dbl>, `1981` <dbl>, `1982` <dbl>,
#   `1983` <dbl>, `1984` <dbl>, `1985` <dbl>, `1986` <dbl>, `1987` <dbl>, `1988` <dbl>, `1989` <dbl>,
#   `1990` <dbl>, `1991` <dbl>, `1992` <dbl>, `1993` <dbl>, `1994` <dbl>, `1995` <dbl>, `1996` <dbl>,
#   `1997` <dbl>, `1998` <dbl>, `1999` <dbl>, `2000` <dbl>, `2001` <dbl>, `2002` <dbl>, `2003` <dbl>,
#   `2004` <dbl>, `2005` <dbl>, `2006` <dbl>, `2007` <dbl>, `2008` <dbl>, `2009` <dbl>, `2010` <dbl>,
#   `2011` <dbl>, `2012` <dbl>, `2013` <dbl>, `2014` <dbl>, `2015` <dbl>, `2016` <dbl>, …
> datanm2<-datanm %>% pivot_longer(5:73, names_to = "year", values_to = "Fbloom_doy"); 
> print(datanm2,n=50)
# A tibble: 2,829 × 6
# Groups:   Location [41]
   Location      lat  long   alt year  Fbloom_doy
   <chr>       <dbl> <dbl> <dbl> <chr>      <dbl>
 1 Japan/Akita  39.7  140.   6.3 1953         119
 2 Japan/Akita  39.7  140.   6.3 1954         112
 3 Japan/Akita  39.7  140.   6.3 1955         113
 4 Japan/Akita  39.7  140.   6.3 1956         117
 5 Japan/Akita  39.7  140.   6.3 1959         107
 6 Japan/Akita  39.7  140.   6.3 1966         115
 7 Japan/Akita  39.7  140.   6.3 1968         115
 8 Japan/Akita  39.7  140.   6.3 1969         119
 9 Japan/Akita  39.7  140.   6.3 1970         121
10 Japan/Akita  39.7  140.   6.3 1971         119
11 Japan/Akita  39.7  140.   6.3 1972         113
12 Japan/Akita  39.7  140.   6.3 1973         113
13 Japan/Akita  39.7  140.   6.3 1974         120
14 Japan/Akita  39.7  140.   6.3 1975         115
15 Japan/Akita  39.7  140.   6.3 1976         119
16 Japan/Akita  39.7  140.   6.3 1977         117
17 Japan/Akita  39.7  140.   6.3 1978         120
18 Japan/Akita  39.7  140.   6.3 1979         115
19 Japan/Akita  39.7  140.   6.3 1980         119
20 Japan/Akita  39.7  140.   6.3 1981         117
21 Japan/Akita  39.7  140.   6.3 1982         114
22 Japan/Akita  39.7  140.   6.3 1983         109
23 Japan/Akita  39.7  140.   6.3 1984         126
24 Japan/Akita  39.7  140.   6.3 1985         113
25 Japan/Akita  39.7  140.   6.3 1986         115
26 Japan/Akita  39.7  140.   6.3 1987         111
27 Japan/Akita  39.7  140.   6.3 1988         119
28 Japan/Akita  39.7  140.   6.3 1989         105
29 Japan/Akita  39.7  140.   6.3 1990         103
30 Japan/Akita  39.7  140.   6.3 1991         112
31 Japan/Akita  39.7  140.   6.3 1992         113
32 Japan/Akita  39.7  140.   6.3 1993         114
33 Japan/Akita  39.7  140.   6.3 1994         114
34 Japan/Akita  39.7  140.   6.3 1995         113
35 Japan/Akita  39.7  140.   6.3 1996         121
36 Japan/Akita  39.7  140.   6.3 1997         112
37 Japan/Akita  39.7  140.   6.3 1998         106
38 Japan/Akita  39.7  140.   6.3 1999         110
39 Japan/Akita  39.7  140.   6.3 2000         116
40 Japan/Akita  39.7  140.   6.3 2001         108
41 Japan/Akita  39.7  140.   6.3 2002         102
42 Japan/Akita  39.7  140.   6.3 2003         111
43 Japan/Akita  39.7  140.   6.3 2004         107
44 Japan/Akita  39.7  140.   6.3 2005         118
45 Japan/Akita  39.7  140.   6.3 2006         116
46 Japan/Akita  39.7  140.   6.3 2007         113
47 Japan/Akita  39.7  140.   6.3 2008         106
48 Japan/Akita  39.7  140.   6.3 2009         109
49 Japan/Akita  39.7  140.   6.3 2010         118
50 Japan/Akita  39.7  140.   6.3 2011         117
# … with 2,779 more rows
> mean<-group_by(datanm2,year)%>% summarise(mean = mean(Fbloom_doy));mean
# A tibble: 69 × 2
   year   mean
   <chr> <dbl>
 1 1953  105. 
 2 1954  101. 
 3 1955  101. 
 4 1956  105. 
 5 1957  107. 
 6 1958  103. 
 7 1959   97.4
 8 1960  103. 
 9 1961  102. 
10 1962  105. 
# … with 59 more rows
> plot (mean$mean~mean$year,col="red", type='l',lwd=2, xlab="Year", 
+       ylab="Mean of full bloom date", main="Mean of Fbloom day vs Year",
+       cex.axis = 1.1, cex.lab = 1.2,font.lab=2)
> plot (mean$mean~mean$year,col="red",lwd=2, xlab="Year", 
+       ylab="Mean of full bloom date", main="Mean of Fbloom day vs Year",pch = 19,cex=0.6,
+       cex.axis = 1.1, cex.lab = 1.2,font.lab=2)
> plot (mean$mean~mean$year,col="red", type='l',lwd=2, xlab="Year", 
+       ylab="Mean of full bloom date", main="Mean of Fbloom day vs Year",
+       cex.axis = 1.1, cex.lab = 1.2,font.lab=2)
> plot (mean$mean~mean$year,col="red",lwd=2, xlab="Year", 
+       ylab="Mean of full bloom date", main="Mean of Fbloom day vs Year",pch = 19,cex=0.6,
+       cex.axis = 1.1, cex.lab = 1.2,font.lab=2)
> ## by alt
> mean2<-group_by(datanm2,lat)%>% summarise(mean = mean(Fbloom_doy));mean2
# A tibble: 41 × 2
     lat  mean
   <dbl> <dbl>
 1  31.6  94  
 2  31.9  92.5
 3  32.7  92.9
 4  32.8  92.0
 5  33.2  94.7
 6  33.8  94.8
 7  33.9  96  
 8  34.1  95.4
 9  34.3  96.0
10  34.4  95.6
# … with 31 more rows
> plot (mean2$mean~mean2$lat,col="red", type='l',lwd=2, xlab="Latitude", 
+       ylab="Mean of full bloom date", main="Mean of Fbloom day vs Latitude",
+       cex.axis = 1.1, cex.lab = 1.2,font.lab=2)
> plot (mean2$mean~mean2$lat,col="red",lwd=2, xlab="Latitude", 
+       ylab="Mean of full bloom date", main="Mean of Fbloom day vs Latitude",pch = 19,cex=0.6,
+       cex.axis = 1.1, cex.lab = 1.2,font.lab=2)
> plot (mean2$mean~mean2$lat,col="red", type='l',lwd=2, xlab="Latitude", 
+       ylab="Mean of full bloom date", main="Mean of Fbloom day vs Latitude",
+       cex.axis = 1.1, cex.lab = 1.2,font.lab=2)
> plot (mean2$mean~mean2$lat,col="red",lwd=2, xlab="Latitude", 
+       ylab="Mean of full bloom date", main="Mean of Fbloom day vs Latitude",pch = 19,cex=0.6,
+       cex.axis = 1.1, cex.lab = 1.2,font.lab=2)
> 
> 
> 
> plot (mean2$mean~mean2$lat,col="red",lwd=2, xlab="Latitude", 
+       ylab="Mean of full bloom date", main="Mean of Fbloom day vs Latitude",pch = 19,cex=0.6,
+       cex.axis = 1.1, cex.lab = 1.2,font.lab=2)
> plot (mean$mean~mean$year,col="red",lwd=2, xlab="Year", 
+       ylab="Mean of full bloom date", main="Mean of Fbloom day vs Year",pch = 19,cex=0.6,
+       cex.axis = 1.1, cex.lab = 1.2,font.lab=2)
> library(tidyverse)
> library(readxl)
> library (ISLR)
> library (splines )
> 
> #1
> data1 <- read_excel("FullFlower.xls", col_names = TRUE,na=c("","NA"))
> data1
> dim(data1)  #1221    6
[1] 1221    6
> missDOY<-sum(is.na(data1$`Full-flowering date (DOY)`));missDOY #388 row
[1] 388
> missAD<-sum(is.na(data1$AD));missAD;  #=0;
[1] 0
> 
> plot(data1$`Full-flowering date (DOY)`~ data1$AD)
> g1<-lm(data1$`Full-flowering date (DOY)`~ data1$AD)
> summary(g1) # very bad fitting

Call:
lm(formula = data1$`Full-flowering date (DOY)` ~ data1$AD)

Residuals:
     Min       1Q   Median       3Q      Max 
-18.7443  -4.6554   0.0242   4.5787  19.1993 

Coefficients:
              Estimate Std. Error t value Pr(>|t|)    
(Intercept)  1.068e+02  1.160e+00  92.086   <2e-16 ***
data1$AD    -1.514e-03  7.331e-04  -2.065   0.0393 *  
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

Residual standard error: 6.463 on 831 degrees of freedom
  (388 observations deleted due to missingness)
Multiple R-squared:  0.005103,	Adjusted R-squared:  0.003906 
F-statistic: 4.262 on 1 and 831 DF,  p-value: 0.03928

> anova(g1)
Analysis of Variance Table

Response: data1$`Full-flowering date (DOY)`
           Df Sum Sq Mean Sq F value  Pr(>F)  
data1$AD    1    178 178.059  4.2622 0.03928 *
Residuals 831  34716  41.777                  
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1
> 
> library(tidyverse)
> library(readxl)
> library (ISLR)
> library (splines )
> 
> #1
> data1 <- read_excel("FullFlower.xls", col_names = TRUE,na=c("","NA"))
Error: `path` does not exist: ‘FullFlower.xls’
> setwd("~/Desktop/STAT classes/Finished/STAT 8000")
> library(tidyverse)
> library(readxl)
> library (ISLR)
> library (splines )
> 
> #1
> data1 <- read_excel("FullFlower.xls", col_names = TRUE,na=c("","NA"))
Error: `path` does not exist: ‘FullFlower.xls’
> setwd("~/Desktop/STAT classes/Finished/STAT 8000")
> library(tidyverse)
> library(readxl)
> library (ISLR)
> library (splines )
> 
> #1
> data1 <- read_excel("FullFlower.xls", col_names = TRUE,na=c("","NA"))
Error: `path` does not exist: ‘FullFlower.xls’
> #1
> data1 <- read_excel("FullFlower.xls", col_names = TRUE,na=c("","NA"))
                                                                                                     
> library(tidyverse)
> library(readxl)
> library (ISLR)
> library (splines )
> 
> #1
> data1 <- read_excel("FullFlower.xls", col_names = TRUE,na=c("","NA"))
> data1                                                                                              
# A tibble: 1,221 × 6
      AD `Full-flowering date (DOY)` `Full-flowering …` `Source code` `Data type code` `Reference Name`
   <dbl>                       <dbl>              <dbl>         <dbl>            <dbl> <chr>           
 1   801                          NA                 NA            NA               NA -               
 2   802                          NA                 NA            NA               NA -               
 3   803                          NA                 NA            NA               NA -               
 4   804                          NA                 NA            NA               NA -               
 5   805                          NA                 NA            NA               NA -               
 6   806                          NA                 NA            NA               NA -               
 7   807                          NA                 NA            NA               NA -               
 8   808                          NA                 NA            NA               NA -               
 9   809                          NA                 NA            NA               NA -               
10   810                          NA                 NA            NA               NA -               
# … with 1,211 more rows
> library(tidyverse)
> library(readxl)
> library (ISLR)
> library (splines )
> 
> #1
> data1 <- read_excel("FullFlower.xls", col_names = TRUE,na=c("","NA"))
Error: `path` does not exist: ‘FullFlower.xls’
> library(tidyverse)
> library(readxl)
> data1<-read_excel("table-1.xls", skip=3,col_names = TRUE,na="")
Error: `path` does not exist: ‘table-1.xls’
> setwd("~/Desktop/STAT classes/Finished/STAT 6365E Programming/Working Directory")
> library(tidyverse)
> library(readxl)
> data1<-read_excel("table-1.xls", skip=3,col_names = TRUE,na="")
New names:
• `` -> `...23`
• `` -> `...24`
> crime<-data1[1:(31-3-7-1),1:22]
> crime$Year[crime$Year==20015]<-2001
> crime$Year[crime$Year==20166]<-2016
> colnames(crime) <- c("Year","Population","VC","VCR","MNM","MNMR" , "RP_RD" ,"RR_RD",
+                      "RP_LD","RR_LD", 
+   "RB","RBR","AA", "AAR","PC","PCR", "BG","BGR","LT","LTR","MVT","MVTR")
> ggplot(data=crime) +
+   geom_line(mapping = aes(x=Year, y=VCR, group=1), color="black")+
+   geom_point(mapping = aes(x=Year, y=VCR, group=1))+
+   ggtitle("Violent Crime Rate vs Year")+
+   ylab("Violent Crime Rate")
> options(warn = - 1)    
> ggplot(data=crime,aes(x = Year)) +
+   geom_line(aes(y=MNMR,group=1,colour="Murder and NM"),size = 1)+
+   geom_line(aes(y=RR_RD,group=1,colour="Rape_RD"),size = 1)+
+   geom_line(aes(y=RR_LD,group=1,colour="Rape_LD"),size = 1)+
+   geom_line(aes(y=RBR,group=1,colour="Robbery"),size = 1)+
+   geom_line(aes(y=AAR,group=1,colour="Aggravated assault"),size = 1)+
+   geom_line(aes(y=VCR,group=1,colour="Violent crime"),size = 1)+
+   scale_colour_manual("", breaks = c("Murder and NM", "Rape_RD", "Rape_LD","Robbery",
+   "Aggravated assault", "Violent crime"), 
+   values = c("black", "blue",
+ "yellow","brown","green","red"))+ 
+   theme(legend.position="bottom")+
+   ggtitle("Violent Crime Rates vs Year")+ ylab("Rate")
> ggplot(data=crime) +
+   geom_line(mapping = aes(x=Year, y=PCR, group=1), color="red")+
+   geom_point(mapping = aes(x=Year, y=PCR, group=1))+
+   ggtitle("Property Crime Rate vs Year")+
+   ylab("Rate")
> ggplot(data=crime,aes(x = Year)) +
+   geom_line(aes(y=BGR,group=1,colour="Burglary"),size = 1)+
+   geom_line(aes(y=LTR,group=1,colour="Larceny-theft"),size = 1)+
+   geom_line(aes(y=MVTR,group=1,colour="Moter vehicle theft"),size = 1)+
+   geom_line(aes(y=PCR,group=1,colour="Property crime rate"),size = 1)+
+   scale_colour_manual("", breaks = c("Burglary", "Larceny-theft", 
+ "Moter vehicle theft","Property crime rate"),
+ values = c("black", "blue", "yellow","red"))+
+   theme(legend.position="bottom")+
+   ggtitle("Property Crime Rates vs Year")+ylab("Rate")
> score<-read_csv("MERGED2015_16_PP.csv",na=c(" ","NA","NULL","Privacy_Suppressed"),
+                 show_col_types = FALSE)
Error: 'MERGED2015_16_PP.csv' does not exist in current working directory ('/Users/wushuangyan/Desktop/STAT classes/Finished/STAT 6365E Programming/Working Directory').
> 