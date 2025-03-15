java c
Assignment   3 
STAT   321   Winter   2025 
Due:   Friday   March   14,   5:00PM1.    (8    points)    Suppose we have a dataset with continuous   response    Y ∈ Rn   ,    and   two
continuous   predictors x   ∈ Rn      and z   ∈   Rn.   Suppose   the   predictors   are   both   centered:
Define   (βˆ0   ,βˆx   ,βˆz   ), the estimate of the unknown regression coefficients in the   (multiple)
linear   regression   model
Yi      = β0   +   βxxi   +   βz   zi   + ϵi.
Define   (β0, βx   )   and   (β0, βz   ),   the   estimates   of the   unkown   regression   coefficients   in   the   (simple)   linear   regression   models
Yi      = β0   +   βxxi   + ϵi   ,               Yi      = β0   +   βz   zi   + ϵi
respectively.
Show   that   if the   sample   correlation   between x and z is 0, βˆx = β˜x, βˆz = β˜z, and
{s.e.(β(ˆ)x   +   β(ˆ)z   )}2      = {s.e.(β(ˆ)x   )}2   + {s.e.(β(ˆ)z   )}2   .
2.    (15   points)   In   the   next   two   problems,   you   will   work   with   data   in   321divorce   . csv,   located on Learn under Assignments/Datasets.   The data contains information about   annual   divorce   rates   among   American   women.    More   information   about   the   data   can   be   found   by   installing   the   faraway   package   and   running   the   following   line   of code:
?faraway::   divusa
Fit   an   MLR   model   with   divorce   as   the   reponse   and   all   other   variates   as   the   predictors.
(a)   Report   the   variance   inflation   factors    (VIFs)   for   this   model.       Is    there   any   evi-   dence   of   extreme   multicollinearity?    Draw   and   interpret   a   scatter   plot   of   the   two predictors   with   the   greatest   sample   correlation.
(b)    Plot the fitted values against the residuals,   and plot each   predictor variate   against   the residuals. Describe   at   least two patterns   in the plots   which   do   not   agree   with   the   MLR   modelling   assumptions.
(c)    Use   at   least   one   plot   to   check   the   normality   assumption   for   the   errors.
(d)    Use   at   least   one   plot   to   check   for   high   leverage   and   high   influence   years.   For   the   three   highest   leverage   years,   report   their   predictors   and   explain   why   these   are   high   leverage   points.
(e)    Use   at   least   one   plot   to   check   for   autocorrelation   in   the   errors.
3.    (10 points) Using   the   321divorce   . csv   dataset   from   Problem   2,   implement   the   follow-   ing   variable   selection   methods   to   determine   the   best   model,   with   response   divorce   and   all   other   variates   as   possible   continuous   predictors.
(a)   Backwards   elimination   (with   level   α   = 0.05)
(b)   Adjusted   R2
(c)   AIC
4.    (10 points)   In this problem,   similar   to   Assignment   2   Problem   5,   you   will   simulate   new   random response vecto代 写STAT 321 Winter 2025 Assignment 3Matlab
代做程序编程语言rs to inspect properties of our MLR confidence intervals.   Use the   predictor matrix X    ∈ R30 ×3 from Assignment 2, Problem 5   (the data can also be loaded   directly   from   321galapagos   . csv,   located   on   Learn   under   Assignments/Datasets),   and   set   the   model   parameters   to

(a)    Simulate   a   new   random   response   vector   Y    =   Xβ    + ϵ where   the   entries   of ϵ   are   mutually   independent   and   satisfy
ϵi    = 50   · Ti   ,             Ti      ~ t(3),               i   =   1,   .   .   .   , 30.
Fit   a   linear   regression   model   with   response   Y      and   predictor   matrix   X      and   create a   QQ-plot   of the   residuals.   Describe   the   pattern   in   the   QQ-plot.(b)    Repeat   the   procedure   in   part   (a)   1000   times,   and   for   each   replication   store   the
estimated   regression   coefficients,  Report   the   sample   means   of

Compare   these   to   the   theoretical   mean   we    derived   in   class   for   the   regression   coefficient   estimator.
(c)    Repeat   the   procedure   in   part    (a)    1000    times,    and   for   each   replication   store   a   99%   confidence   interval   for   β1   .      Report   the   proportion   of   replications   in   which   the   confidence   interval   contains   the   true   expected   response.      Do   these   intervals   actually   cover   the   true   parameter   in   99%   of replications?
Additional instructions: 
– If you are unsure how to use an R function, its documentation can be viewed by typing a question mark and then the function name (i.e. ?function) into the RStudio console.
– Unless otherwise specified, you may use results from lecture without additional justification. Results from the reference textbooks can be used, but you should show all steps for full marks.
– This assignment will be graded out of 43 points. Per the course outline, in normal circumstances it will count for 5% of your final grade.
– Assignment solutions, including code, should be submitted on Crowdmark. Make sure that the uploaded solutions correspond to the correct problem. If the assignment is submitted with written solutions but no supporting code, it will be graded as normal, but the point total will be multiplied by 0.75.
– If you experience technical difficulties using Crowdmark,
1. Consult Crowdmark Help
2. Watch this short video about submitting an assignment on Crowdmark
3. As a last resort, if you cannot upload your assignment to Crowdmark before the deadline, email it to [email   protected], so I have proof that you completed your assignment on time.
– If you choose to submit typed solutions, please also email me the .tex or RMarkdown files used to compile your solutions.
– Rules regarding extensions for (formally documented) absences and grades for late submissions are provided in the course outline on Learn.



         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
