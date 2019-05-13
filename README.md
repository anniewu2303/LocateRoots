# LocateRoots
Locate roots of an equation using Bisection, Newton-Raphson, Secant, False-Position, and Modified Secant methods. <br />
```
Function #1 
    f(x) = 2x3 – 11.7x2 + 17.7x – 5 has 3 roots in range [0, 4]
    actual roots: 0.365, 1.922, 3.563
```
```
Function #2 
    f(x) = x + 10 – xcosh(50/x) has 1 root in range [120, 130]
    actual root: 126.632
```
### To run file on command line / terminal
```
java -jar "filepath/../LocateRoots.jar"
```
### Sample Output
```
 Program 2: Locating Roots of a Function - Annie Wu

   n    |     a         |     b         |     c         |    f(a)       |    f(b)       |    f(c)       |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   0.000       |   1.000       |   0.500       |   -5.000      |   3.000       |   1.175       |   1.000
   1    |   0.000       |   0.500       |   0.250       |   -5.000      |   1.175       |   -1.275      |   1.000
   2    |   0.250       |   0.500       |   0.375       |   -1.275      |   1.175       |   0.098       |   0.333
   3    |   0.250       |   0.375       |   0.313       |   -1.275      |   0.098       |   -0.550      |   0.200
   4    |   0.313       |   0.375       |   0.344       |   -0.550      |   0.098       |   -0.217      |   0.091
   5    |   0.344       |   0.375       |   0.359       |   -0.217      |   0.098       |   -0.057      |   0.043
   6    |   0.359       |   0.375       |   0.367       |   -0.057      |   0.098       |   0.021       |   0.021
   7    |   0.359       |   0.367       |   0.363       |   -0.057      |   0.021       |   -0.018      |   0.011
   8    |   0.363       |   0.367       |   0.365       |   -0.018      |   0.021       |   0.001       |   0.005
BISECTION - The root 0.365 has been found in between 0 and 1 for function #1 in 9 iterations.

   n    |     a         |     b         |     c         |    f(a)       |    f(b)       |    f(c)       |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   1.000       |   2.000       |   1.500       |   3.000       |   -0.400      |   1.975       |   1.000
   1    |   1.500       |   2.000       |   1.750       |   1.975       |   -0.400      |   0.863       |   0.143
   2    |   1.750       |   2.000       |   1.875       |   0.863       |   -0.400      |   0.238       |   0.067
   3    |   1.875       |   2.000       |   1.938       |   0.238       |   -0.400      |   -0.081      |   0.032
   4    |   1.875       |   1.938       |   1.906       |   0.238       |   -0.081      |   0.079       |   0.016
   5    |   1.906       |   1.938       |   1.922       |   0.079       |   -0.081      |   -0.001      |   0.008
BISECTION - The root 1.922 has been found in between 1 and 2 for function #1 in 6 iterations.

   n    |     a         |     b         |     c         |    f(a)       |    f(b)       |    f(c)       |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   2.000       |   3.000       |   2.500       |   -0.400      |   -3.200      |   -2.625      |   1.000
   1    |   2.500       |   3.000       |   2.750       |   -2.625      |   -3.200      |   -3.212      |   0.091
   2    |   2.750       |   3.000       |   2.875       |   -3.212      |   -3.200      |   -3.293      |   0.043
   3    |   2.875       |   3.000       |   2.938       |   -3.293      |   -3.200      |   -3.270      |   0.021
   4    |   2.938       |   3.000       |   2.969       |   -3.270      |   -3.200      |   -3.241      |   0.011
   5    |   2.969       |   3.000       |   2.984       |   -3.241      |   -3.200      |   -3.222      |   0.005
BISECTION - There are no roots in between 2 and 3 for function #1.

   n    |     a         |     b         |     c         |    f(a)       |    f(b)       |    f(c)       |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   3.000       |   4.000       |   3.500       |   -3.200      |   6.600       |   -0.625      |   1.000
   1    |   3.500       |   4.000       |   3.750       |   -0.625      |   6.600       |   2.313       |   0.067
   2    |   3.500       |   3.750       |   3.625       |   -0.625      |   2.313       |   0.687       |   0.034
   3    |   3.500       |   3.625       |   3.563       |   -0.625      |   0.687       |   -0.007      |   0.018
   4    |   3.563       |   3.625       |   3.594       |   -0.007      |   0.687       |   0.330       |   0.009
BISECTION - The root 3.594 has been found in between 3 and 4 for function #1 in 5 iterations.

   n    |     xn        |   f(xn)       |   f'(xn)      |   Error
------------------------------------------------------------------
   0    |   1.000       |   3.000       |   0.300       |   1.000
   1    |   -9.000      |   -2570.000   |   714.300     |   1.111
   2    |   -5.402      |   -757.341    |   319.203     |   0.666
   3    |   -3.029      |   -221.608    |   143.656     |   0.783
   4    |   -1.487      |   -63.756     |   65.756      |   1.038
   5    |   -0.517      |   -17.563     |   31.409      |   1.874
   6    |   0.042       |   -4.279      |   16.730      |   13.345
   7    |   0.298       |   -0.715      |   11.267      |   0.859
   8    |   0.361       |   -0.039      |   10.032      |   0.176
   9    |   0.365       |   -0.000      |   9.957       |   0.011
   10   |   0.365       |   -0.000      |   9.956       |   0.000
NEWTON - The root 0.365 has been found for function #1 starting at x = 1 in 11 iterations.

   n    |     xn        |   f(xn)       |   f'(xn)      |   Error
------------------------------------------------------------------
   0    |   2.000       |   -0.400      |   -5.100      |   1.000
   1    |   1.922       |   0.001       |   -5.110      |   0.041
   2    |   1.922       |   -0.000      |   -5.110      |   0.000
NEWTON - The root 1.922 has been found for function #1 starting at x = 2 in 3 iterations.

   n    |     xn        |   f(xn)       |   f'(xn)      |   Error
------------------------------------------------------------------
   0    |   3.000       |   -3.200      |   1.500       |   1.000
   1    |   5.133       |   48.090      |   55.687      |   0.416
   2    |   4.270       |   12.956      |   27.172      |   0.202
   3    |   3.793       |   2.948       |   15.263      |   0.126
   4    |   3.600       |   0.398       |   11.216      |   0.054
   5    |   3.564       |   0.012       |   10.522      |   0.010
NEWTON - The root 3.564 has been found for function #1 starting at x = 3 in 6 iterations.

   n    |     xn        |   f(xn)       |   f'(xn)      |   Error
------------------------------------------------------------------
   0    |   4.000       |   6.600       |   20.100      |   1.000
   1    |   3.672       |   1.255       |   12.669      |   0.089
   2    |   3.573       |   0.099       |   10.681      |   0.028
   3    |   3.563       |   0.001       |   10.500      |   0.003
NEWTON - The root 3.563 has been found for function #1 starting at x = 4 in 4 iterations.

   n    |    xn-1       |     xn        |   f(xn-1)     |   f(xn)       |   f'(xn)      |   Error
----------------------------------------------------------------------------------------------------
   0    |   0.000       |   1.000       |   -5.000      |   3.000       |   0.300       |   1.000
   1    |   1.000       |   0.625       |   3.000       |   1.980       |   5.419       |   0.600
   2    |   0.625       |   -0.103      |   1.980       |   -6.958      |   20.185      |   7.042
   3    |   -0.103      |   0.464       |   -6.958      |   0.890       |   8.141       |   1.223
   4    |   0.464       |   0.399       |   0.890       |   0.329       |   9.313       |   0.161
   5    |   0.399       |   0.362       |   0.329       |   -0.036      |   10.024      |   0.104
   6    |   0.362       |   0.365       |   -0.036      |   0.001       |   9.954       |   0.010
   7    |   0.365       |   0.365       |   0.001       |   0.000       |   9.956       |   0.000
SECANT - The root 0.365 has been found for function #1 starting at x = 1 in 8 iterations.

   n    |    xn-1       |     xn        |   f(xn-1)     |   f(xn)       |   f'(xn)      |   Error
----------------------------------------------------------------------------------------------------
   0    |   1.000       |   2.000       |   3.000       |   -0.400      |   -5.100      |   0.500
   1    |   2.000       |   1.882       |   -0.400      |   0.201       |   -5.088      |   0.062
   2    |   1.882       |   1.922       |   0.201       |   0.000       |   -5.110      |   0.020
   3    |   1.922       |   1.922       |   0.000       |   -0.000      |   -5.110      |   0.000
SECANT - The root 1.922 has been found for function #1 starting at x = 2 in 4 iterations.

   n    |    xn-1       |     xn        |   f(xn-1)     |   f(xn)       |   f'(xn)      |   Error
----------------------------------------------------------------------------------------------------
   0    |   2.000       |   3.000       |   -0.400      |   -3.200      |   1.500       |   0.333
   1    |   3.000       |   1.857       |   -3.200      |   0.329       |   -5.063      |   0.615
   2    |   1.857       |   1.964       |   0.329       |   -0.214      |   -5.114      |   0.054
   3    |   1.964       |   1.922       |   -0.214      |   0.001       |   -5.110      |   0.022
   4    |   1.922       |   1.922       |   0.001       |   0.000       |   -5.110      |   0.000
SECANT - The root 1.922 has been found for function #1 starting at x = 3 in 5 iterations.

   n    |    xn-1       |     xn        |   f(xn-1)     |   f(xn)       |   f'(xn)      |   Error
----------------------------------------------------------------------------------------------------
   0    |   3.000       |   4.000       |   -3.200      |   6.600       |   20.100      |   0.250
   1    |   4.000       |   3.327       |   6.600       |   -1.969      |   6.254       |   0.202
   2    |   3.327       |   3.481       |   -1.969      |   -0.796      |   8.954       |   0.044
   3    |   3.481       |   3.586       |   -0.796      |   0.248       |   10.949      |   0.029
   4    |   3.586       |   3.561       |   0.248       |   -0.019      |   10.464      |   0.007
SECANT - The root 3.561 has been found for function #1 starting at x = 4 in 5 iterations.

   n    |     a         |     b         |     c         |    f(a)       |    f(b)       |    f(c)       |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   0.000       |   1.000       |   0.625       |   -5.000      |   3.000       |   1.980       |   1.000
   1    |   0.000       |   0.625       |   0.448       |   -5.000      |   1.980       |   0.758       |   0.396
   2    |   0.000       |   0.448       |   0.389       |   -5.000      |   0.758       |   0.230       |   0.152
   3    |   0.000       |   0.389       |   0.372       |   -5.000      |   0.230       |   0.065       |   0.046
   4    |   0.000       |   0.372       |   0.367       |   -5.000      |   0.065       |   0.018       |   0.013
   5    |   0.000       |   0.367       |   0.366       |   -5.000      |   0.018       |   0.005       |   0.004
FALSE-POSITION - The root 0.366 has been found in between 0 and 1 for function #1 in 6 iterations.

   n    |     a         |     b         |     c         |    f(a)       |    f(b)       |    f(c)       |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   1.000       |   2.000       |   1.882       |   3.000       |   -0.400      |   0.201       |   1.000
   1    |   1.882       |   2.000       |   1.922       |   0.201       |   -0.400      |   0.000       |   0.020
   2    |   1.922       |   2.000       |   1.922       |   0.000       |   -0.400      |   0.000       |   0.000
FALSE-POSITION - The root 1.922 has been found in between 1 and 2 for function #1 in 3 iterations.

   n    |     a         |     b         |     c         |    f(a)       |    f(b)       |    f(c)       |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   2.000       |   3.000       |   1.857       |   -0.400      |   -3.200      |   0.329       |   1.000
   1    |   2.000       |   1.857       |   1.922       |   -0.400      |   0.329       |   0.001       |   0.034
   2    |   2.000       |   1.922       |   1.922       |   -0.400      |   0.001       |   0.000       |   0.000
FALSE-POSITION - The root 1.922 has been found in between 2 and 3 for function #1 in 3 iterations.

   n    |     a         |     b         |     c         |    f(a)       |    f(b)       |    f(c)       |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   3.000       |   4.000       |   3.327       |   -3.200      |   6.600       |   -1.969      |   1.000
   1    |   3.327       |   4.000       |   3.481       |   -1.969      |   6.600       |   -0.796      |   0.044
   2    |   3.481       |   4.000       |   3.537       |   -0.796      |   6.600       |   -0.267      |   0.016
   3    |   3.537       |   4.000       |   3.555       |   -0.267      |   6.600       |   -0.084      |   0.005
FALSE-POSITION - The root 3.555 has been found in between 3 and 4 for function #1 in 4 iterations.

   n    |    xn         |  delta*xn     |   f(xn)       |  f(x+delta*x) |   f'(xn)      |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   1.000       |   0.010       |   3.000       |   3.002       |   0.300       |   1.000
   1    |   -11.336     |   -0.113      |   -4622.118   |   -4742.612   |   1053.916    |   1.088
   2    |   -6.987      |   -0.070      |   -1382.148   |   -1415.539   |   474.132     |   0.622
   3    |   -4.095      |   -0.041      |   -411.030    |   -419.860    |   214.141     |   0.706
   4    |   -2.189      |   -0.022      |   -120.774    |   -122.924    |   97.667      |   0.871
   5    |   -0.959      |   -0.010      |   -34.505     |   -34.944     |   45.663      |   1.282
   6    |   -0.206      |   -0.002      |   -9.166      |   -9.213      |   22.782      |   3.650
   7    |   0.196       |   0.002       |   -1.970      |   -1.944      |   13.352      |   2.054
   8    |   0.343       |   0.003       |   -0.220      |   -0.185      |   10.372      |   0.430
   9    |   0.365       |   0.004       |   -0.004      |   0.033       |   9.963       |   0.058
   10   |   0.365       |   0.004       |   0.000       |   0.036       |   9.956       |   0.001
MODIFIED SECANT - The root 0.365 has been found for function #1 starting at x = 1 in 11 iterations.

   n    |    xn         |  delta*xn     |   f(xn)       |  f(x+delta*x) |   f'(xn)      |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   2.000       |   0.020       |   -0.400      |   -0.502      |   -5.100      |   0.500
   1    |   1.921       |   0.019       |   0.001       |   -0.097      |   -5.110      |   0.041
   2    |   1.922       |   0.019       |   0.000       |   -0.098      |   -5.110      |   0.000
MODIFIED SECANT - The root 1.922 has been found for function #1 starting at x = 2 in 3 iterations.

   n    |    xn         |  delta*xn     |   f(xn)       |  f(x+delta*x) |   f'(xn)      |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   3.000       |   0.030       |   -3.200      |   -3.149      |   1.500       |   0.333
   1    |   4.893       |   0.049       |   35.763      |   38.097      |   46.838      |   0.387
   2    |   4.143       |   0.041       |   9.730       |   10.737      |   23.739      |   0.181
   3    |   3.742       |   0.037       |   2.203       |   2.748       |   14.159      |   0.107
   4    |   3.591       |   0.036       |   0.300       |   0.710       |   11.043      |   0.042
   5    |   3.565       |   0.036       |   0.016       |   0.404       |   10.529      |   0.007
MODIFIED SECANT - The root 3.565 has been found for function #1 starting at x = 3 in 6 iterations.

   n    |    xn         |  delta*xn     |   f(xn)       |  f(x+delta*x) |   f'(xn)      |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   4.000       |   0.040       |   6.600       |   7.424       |   20.100      |   0.250
   1    |   3.680       |   0.037       |   1.356       |   1.842       |   12.833      |   0.087
   2    |   3.577       |   0.036       |   0.147       |   0.544       |   10.767      |   0.029
   3    |   3.564       |   0.036       |   0.006       |   0.393       |   10.510      |   0.004
MODIFIED SECANT - The root 3.564 has been found for function #1 starting at x = 4 in 4 iterations.

   n    |     a         |     b         |     c         |    f(a)       |    f(b)       |    f(c)       |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   120.000     |   130.000     |   125.000     |   -0.568      |   0.265       |   -0.134      |   1.000
   1    |   125.000     |   130.000     |   127.500     |   -0.134      |   0.265       |   0.070       |   0.020
   2    |   125.000     |   127.500     |   126.250     |   -0.134      |   0.070       |   -0.031      |   0.010
BISECTION - The root 126.250 has been found in between 120 and 130 for function #2 in 3 iterations.

   n    |     xn        |   f(xn)       |   f'(xn)      |   Error
------------------------------------------------------------------
   0    |   130.000     |   0.265       |   0.077       |   1.000
   1    |   126.540     |   -0.008      |   0.081       |   0.027
   2    |   126.632     |   -0.000      |   0.081       |   0.001
NEWTON - The root 126.632 has been found for function #2 starting at x = 130 in 3 iterations.

   n    |    xn-1       |     xn        |   f(xn-1)     |   f(xn)       |   f'(xn)      |   Error
----------------------------------------------------------------------------------------------------
   0    |   120.000     |   130.000     |   -0.568      |   0.265       |   0.077       |   0.077
   1    |   130.000     |   126.816     |   0.265       |   0.015       |   0.081       |   0.025
   2    |   126.816     |   126.627     |   0.015       |   -0.000      |   0.081       |   0.001
SECANT - The root 126.627 has been found for function #2 starting at x = 130 in 3 iterations.

   n    |     a         |     b         |     c         |    f(a)       |    f(b)       |    f(c)       |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   120.000     |   130.000     |   126.816     |   -0.568      |   0.265       |   0.015       |   1.000
   1    |   120.000     |   126.816     |   126.642     |   -0.568      |   0.015       |   0.001       |   0.001
FALSE-POSITION - The root 126.642 has been found in between 120 and 130 for function #2 in 2 iterations.

   n    |    xn         |  delta*xn     |   f(xn)       |  f(x+delta*x) |   f'(xn)      |   Error
-------------------------------------------------------------------------------------------------------------------
   0    |   130.000     |   1.300       |   0.265       |   0.364       |   0.077       |   0.077
   1    |   126.504     |   1.265       |   -0.010      |   0.091       |   0.081       |   0.028
   2    |   126.634     |   1.266       |   0.000       |   0.102       |   0.081       |   0.001
MODIFIED SECANT - The root 126.634 has been found for function #2 starting at x = 130 in 3 iterations.

End of Program
```
