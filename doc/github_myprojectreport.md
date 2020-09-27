R Markdown
----------

Here is a link to \[SLACK\]
(<a href="https://ikeabworkspace.slack.com/archives/C01BC64V1FC" class="uri">https://ikeabworkspace.slack.com/archives/C01BC64V1FC</a>)

The objective of my **project** is to **compare** group A vs. group B.

This would enable us to *discover* new *treatments*.

THe name of current project is `ClinicalABC`.

``` r
2+2
```

    ## [1] 4

``` r
mean(c(1,2,3,4,5))
```

    ## [1] 3

######################################### 

1.  Introduction
    1.  Disease
        1.  Prevalence
        2.  Causes
        3.  Treatment
    2.  Objective
        1.  Markers
2.  Methods
    1.  Regression
3.  Results
    1.  Descriptive
    2.  Main results
    3.  Secondary results
        \#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#

> Parkinson’s disease is one of the most common neurodegenerative
> diseases.
>
> 1.  The disease is characterized by degeneration of
> 2.  The disease has an delayed age of onset
>
> > above 60

####################################### 

| FID                            | IID                            |  nstudy| study\_recoded |  age\_study|  age\_onset|  age\_diag|  pd\_duration|  atc\_fam|  ethnicity|  GBA| GBA\_mutation |  LRKK2| LRKK2\_mutation |  atc\_fam\_mutation|
|:-------------------------------|:-------------------------------|-------:|:---------------|-----------:|-----------:|----------:|-------------:|---------:|----------:|----:|:--------------|------:|:----------------|-------------------:|
| TRO\_174580550\_TRO\_174580550 | TRO\_174580550\_TRO\_174580550 |       1| aasly          |          77|          59|         NA|            18|        NA|          1|    0| NA            |      0| NA              |                  NA|
| TRO\_174581017\_TRO\_174581017 | TRO\_174581017\_TRO\_174581017 |       1| aasly          |          NA|          NA|         NA|            NA|         0|         NA|    0| NA            |      0| NA              |                   0|
| TRO\_174581062\_TRO\_174581062 | TRO\_174581062\_TRO\_174581062 |       1| aasly          |          NA|          NA|         NA|            NA|         0|         NA|    0| NA            |      0| NA              |                   0|
| TRO\_177274656\_TRO\_177274656 | TRO\_177274656\_TRO\_177274656 |       1| aasly          |          NA|          NA|         NA|            NA|         0|         NA|    0| NA            |      0| NA              |                   0|
| TRO\_177274662\_TRO\_177274662 | TRO\_177274662\_TRO\_177274662 |       1| aasly          |          NA|          NA|         NA|            NA|         0|         NA|    0| NA            |      0| NA              |                   0|
| TRO\_177274663\_TRO\_177274663 | TRO\_177274663\_TRO\_177274663 |       1| aasly          |          NA|          NA|         NA|            NA|         0|         NA|    0| NA            |      0| NA              |                   0|

    ## [1] "<table class=\"Rtable1\">\n<thead>\n<tr>\n<th class='rowlabel firstrow lastrow'></th>\n<th class='firstrow lastrow'><span class='stratlabel'>Overall<br><span class='stratn'>(N=24622)</span></span></th>\n</tr>\n</thead>\n<tbody>\n<tr>\n<td class='rowlabel firstrow'><span class='varlabel'>Age at onset of PD</span></td>\n<td class='firstrow'></td>\n</tr>\n<tr>\n<td class='rowlabel'>Mean (SD)</td>\n<td>58.5 (11.5)</td>\n</tr>\n<tr>\n<td class='rowlabel'>Median [Min, Max]</td>\n<td>59.0 [12.0, 93.0]</td>\n</tr>\n<tr>\n<td class='rowlabel lastrow'>Missing</td>\n<td class='lastrow'>11831 (48.1%)</td>\n</tr>\n<tr>\n<td class='rowlabel firstrow'><span class='varlabel'>Duration of PD</span></td>\n<td class='firstrow'></td>\n</tr>\n<tr>\n<td class='rowlabel'>Mean (SD)</td>\n<td>8.05 (6.42)</td>\n</tr>\n<tr>\n<td class='rowlabel'>Median [Min, Max]</td>\n<td>7.00 [0, 51.0]</td>\n</tr>\n<tr>\n<td class='rowlabel lastrow'>Missing</td>\n<td class='lastrow'>11831 (48.1%)</td>\n</tr>\n<tr>\n<td class='rowlabel firstrow'><span class='varlabel'>Presence of GBA mutation</span></td>\n<td class='firstrow'></td>\n</tr>\n<tr>\n<td class='rowlabel'>D140H</td>\n<td>1 (0.0%)</td>\n</tr>\n<tr>\n<td class='rowlabel'>D409H</td>\n<td>1 (0.0%)</td>\n</tr>\n<tr>\n<td class='rowlabel'>deletion</td>\n<td>1 (0.0%)</td>\n</tr>\n<tr>\n<td class='rowlabel'>E326K</td>\n<td>72 (0.3%)</td>\n</tr>\n<tr>\n<td class='rowlabel'>Heterozygous</td>\n<td>28 (0.1%)</td>\n</tr>\n<tr>\n<td class='rowlabel'>Homozygous</td>\n<td>4 (0.0%)</td>\n</tr>\n<tr>\n<td class='rowlabel'>IVS2+1g>a</td>\n<td>1 (0.0%)</td>\n</tr>\n<tr>\n<td class='rowlabel'>L444P</td>\n<td>51 (0.2%)</td>\n</tr>\n<tr>\n<td class='rowlabel'>N370S</td>\n<td>49 (0.2%)</td>\n</tr>\n<tr>\n<td class='rowlabel'>N370S((hetero)</td>\n<td>1 (0.0%)</td>\n</tr>\n<tr>\n<td class='rowlabel'>R359X</td>\n<td>1 (0.0%)</td>\n</tr>\n<tr>\n<td class='rowlabel'>R398X</td>\n<td>1 (0.0%)</td>\n</tr>\n<tr>\n<td class='rowlabel'>S271G</td>\n<td>1 (0.0%)</td>\n</tr>\n<tr>\n<td class='rowlabel lastrow'>Missing</td>\n<td class='lastrow'>24410 (99.1%)</td>\n</tr>\n<tr>\n<td class='rowlabel firstrow'><span class='varlabel'>Presence of LRKK2 mutation</span></td>\n<td class='firstrow'></td>\n</tr>\n<tr>\n<td class='rowlabel'>G2019S</td>\n<td>2 (0.0%)</td>\n</tr>\n<tr>\n<td class='rowlabel lastrow'>Missing</td>\n<td class='lastrow'>24620 (100.0%)</td>\n</tr>\n<tr>\n<td class='rowlabel firstrow'><span class='varlabel'>Presence of ATC mutation</span></td>\n<td class='firstrow'></td>\n</tr>\n<tr>\n<td class='rowlabel'>Yes</td>\n<td>2545 (10.3%)</td>\n</tr>\n<tr>\n<td class='rowlabel'>No</td>\n<td>12116 (49.2%)</td>\n</tr>\n<tr>\n<td class='rowlabel lastrow'>Missing</td>\n<td class='lastrow'>9961 (40.5%)</td>\n</tr>\n</tbody>\n</table>\n"

Including Plots
---------------

*Y* = *β*<sub>0</sub> + *β*<sub>1</sub> \* *X*

You can also embed plots, for example:

\#\`\`\`{r data cleaning, echo=FALSE} head(rawdata) rawdata %\>%
slice(40:50) %\>% select(starts\_with(“age”)) %\>% filter(age\_study \>
80) %\>% rename (age = age\_study) %\>% mutate(age = age/10) %\>%
group\_by() %\>% summarize() %\>% merge() table1() write\_csv()%\>%
\#function() %\>% to\_lower() %\>% arrange(desc()) %\>% count()

\# Go ahead and save this data in your package, name it as cleandata. \#
cleandata() \# \`\`\`

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.
