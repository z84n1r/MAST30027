java cMAST30027: Modern Applied Statistics
Assignment 2, 2024.
Due: 11:59pm Monday September 2nd
 This assignment is worth 8% of your total mark.
 To get full marks, show your working including 1) R commands and outputs you use, 2)
mathematics derivation, and 3) rigorous explanation why you reach conclusions or answers.
If you just provide final answers, you will get zero mark.
 The assignment you hand in must be typed (except for math formulas), and be submitted
using LMS as a single PDF document only (no other formats allowed). For math formulas,
you can take a picture of them. Your answers must be clearly numbered and in the same
order as the assignment questions.
 The LMS will not accept late submissions. It is your responsibility to ensure that your
assignments are submitted correctly and on time, and problems with online submissions are
not a valid excuse for submitting a late or incorrect version of an assignment.
 We will mark a selected set of problems. We will select problems worth ≥ 50% of the full
marks listed.
 If you need an extension, please contact the lecturer before the due date with appropriate
justification and supporting documents. Late assignments will only be accepted if you have
obtained an extension from the lecturer before the due date. To ensure that the lecturer
responds to your extension request email before the due date, please contact 24h before the
due date. Under no circumstances an assignment will be marked if solutions for it have been
released.
 Also, please read the “Assessments” section in “Subject Overview” page of the LMS.
1. The inverse Gaussian distribution has p.d.f.
f(x;μ, λ) =
(
λ
2pix3
)1/2
exp
(?λ(x? μ)2
2μ2x
)
for x > 0, where μ > 0 and λ > 0.
(a) (5 marks) Show that the inverse Gaussian distribution is an exponential family.
(b) (5 marks) Obtain the canonical link and the variance function.
[hint: you could consider θ = ?1/μ2.]
2. (30 marks)
Note: There is no unique answer for this problem. The report for this prob-
lem should be typed. Hand-written report or report including screen-captured
R codes or figures won’t be marked. An example report written by a student
previous year has been post代 写MAST30027、Java/C++
代做程序编程语言ed on LMS.
1
Data: The dataset comes from the Fiji Fertility Survey and shows data on the number of
children ever born to married women of the Indian race classified by duration since their
first marriage (grouped in six categories), type of place of residence (Suva, urban, and rural),
and educational level (classified in four categories: none, lower primary, upper primary, and
secondary or higher). The data can be found in the file assignment2 prob2.txt. The
dataset has 70 rows representing 70 groups of families. Each row has entries for:
 duration: marriage duration of mothers in each group (years),
 residence: residence of families in each group (Suva, urban, rural),
 education: education of mothers in each group (none, lower primary, upper primary,
secondary+),
 nChildren: number of children ever born in each group (e.g. 4), and
 nMother: number of mothers in each group (e.g. 8).
We can summarise data as a table as follows.
> data  data$duration  , ordered=TRUE)
> data$residence  data$education  ftable(xtabs(cbind(nChildren,nMother) ~ duration + residence + education, data))
Problem: We want to determine which factors (duration, residence, education) and two-
way interactions are related to the number of children per woman (fertility rate). The
observed number of children ever born in each group (nChildren) depends on the number of
mothers (nMother) in each group. We must take account of the difference in the number of
mothers (hint: one of the lab problems shows how to handle this issue). Write a report on
the analysis that should summarise the substantive conclusions and include the highlights
of your analysis: for example, data visualisation, choice of model (e.g., Poisson, binomial,
gamma, etc), model fitting and model selection (e.g., using AIC), diagnostic, check for
overdispersion if necessary, and summary/interpretation of your final model.
At each step of your analysis, you should write why you do that and your interpreta-
tion/conclusion. For example, “I make an interaction plot to see whether there are in-
teractions between X and Y”, show a plot, and “It seems that there are some interaction
between X and Y”.

         
加QQ：99515681  WX：codinghelp
