---
title: "Myproject"
author: "Sandeep Grover"
date: "23/09/2020"
output:
  html_document: 
    theme: cerulean
    highlight: kate
    css: myfirstcss.css
    #fig_height: 5
    #fig_width: 5
    toc: yes
    toc_float: true
    code_folding: hide
    keep_md: true
---




## R Markdown {#nextsteps .emphasized}

Here is a link to [SLACK] (https://ikeabworkspace.slack.com/archives/C01BC64V1FC)

The objective of my **project** is to __compare__ group A vs. group B.

This would enable us to *discover* new _treatments_.

THe name of current project is `ClinicalABC`.




```r
2+2
```

```
## [1] 4
```

```r
mean(c(1,2,3,4,5))
```

```
## [1] 3
```
#########################################
1. Introduction
    a. Disease
        i. Prevalence
        ii. Causes
        iii. Treatment
    b. Objective
        i. Markers
2. Methods
    a. Regression
3. Results
    a. Descriptive 
    b. Main results
    c. Secondary results
########################################
    
> Parkinson's disease is one of the most 
> common neurodegenerative diseases.
>
> 1. The disease is characterized by degeneration of
> 2. The disease has an delayed age of onset
>
> > above 60

#######################################



FID                           IID                            nstudy  study_recoded    age_study   age_onset   age_diag   pd_duration   atc_fam   ethnicity   GBA  GBA_mutation    LRKK2  LRKK2_mutation    atc_fam_mutation
----------------------------  ----------------------------  -------  --------------  ----------  ----------  ---------  ------------  --------  ----------  ----  -------------  ------  ---------------  -----------------
TRO_174580550_TRO_174580550   TRO_174580550_TRO_174580550         1  aasly                   77          59         NA            18        NA           1     0  NA                  0  NA                              NA
TRO_174581017_TRO_174581017   TRO_174581017_TRO_174581017         1  aasly                   NA          NA         NA            NA         0          NA     0  NA                  0  NA                               0
TRO_174581062_TRO_174581062   TRO_174581062_TRO_174581062         1  aasly                   NA          NA         NA            NA         0          NA     0  NA                  0  NA                               0
TRO_177274656_TRO_177274656   TRO_177274656_TRO_177274656         1  aasly                   NA          NA         NA            NA         0          NA     0  NA                  0  NA                               0
TRO_177274662_TRO_177274662   TRO_177274662_TRO_177274662         1  aasly                   NA          NA         NA            NA         0          NA     0  NA                  0  NA                               0
TRO_177274663_TRO_177274663   TRO_177274663_TRO_177274663         1  aasly                   NA          NA         NA            NA         0          NA     0  NA                  0  NA                               0

<!--html_preserve--><div class="Rtable1"><table class="Rtable1">
<thead>
<tr>
<th class='rowlabel firstrow lastrow'></th>
<th class='firstrow lastrow'><span class='stratlabel'>Overall<br><span class='stratn'>(N=24622)</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td class='rowlabel firstrow'><span class='varlabel'>Age at onset of PD</span></td>
<td class='firstrow'></td>
</tr>
<tr>
<td class='rowlabel'>Mean (SD)</td>
<td>58.5 (11.5)</td>
</tr>
<tr>
<td class='rowlabel'>Median [Min, Max]</td>
<td>59.0 [12.0, 93.0]</td>
</tr>
<tr>
<td class='rowlabel lastrow'>Missing</td>
<td class='lastrow'>11831 (48.1%)</td>
</tr>
<tr>
<td class='rowlabel firstrow'><span class='varlabel'>Duration of PD</span></td>
<td class='firstrow'></td>
</tr>
<tr>
<td class='rowlabel'>Mean (SD)</td>
<td>8.05 (6.42)</td>
</tr>
<tr>
<td class='rowlabel'>Median [Min, Max]</td>
<td>7.00 [0, 51.0]</td>
</tr>
<tr>
<td class='rowlabel lastrow'>Missing</td>
<td class='lastrow'>11831 (48.1%)</td>
</tr>
<tr>
<td class='rowlabel firstrow'><span class='varlabel'>Presence of GBA mutation</span></td>
<td class='firstrow'></td>
</tr>
<tr>
<td class='rowlabel'>D140H</td>
<td>1 (0.0%)</td>
</tr>
<tr>
<td class='rowlabel'>D409H</td>
<td>1 (0.0%)</td>
</tr>
<tr>
<td class='rowlabel'>deletion</td>
<td>1 (0.0%)</td>
</tr>
<tr>
<td class='rowlabel'>E326K</td>
<td>72 (0.3%)</td>
</tr>
<tr>
<td class='rowlabel'>Heterozygous</td>
<td>28 (0.1%)</td>
</tr>
<tr>
<td class='rowlabel'>Homozygous</td>
<td>4 (0.0%)</td>
</tr>
<tr>
<td class='rowlabel'>IVS2+1g>a</td>
<td>1 (0.0%)</td>
</tr>
<tr>
<td class='rowlabel'>L444P</td>
<td>51 (0.2%)</td>
</tr>
<tr>
<td class='rowlabel'>N370S</td>
<td>49 (0.2%)</td>
</tr>
<tr>
<td class='rowlabel'>N370S((hetero)</td>
<td>1 (0.0%)</td>
</tr>
<tr>
<td class='rowlabel'>R359X</td>
<td>1 (0.0%)</td>
</tr>
<tr>
<td class='rowlabel'>R398X</td>
<td>1 (0.0%)</td>
</tr>
<tr>
<td class='rowlabel'>S271G</td>
<td>1 (0.0%)</td>
</tr>
<tr>
<td class='rowlabel lastrow'>Missing</td>
<td class='lastrow'>24410 (99.1%)</td>
</tr>
<tr>
<td class='rowlabel firstrow'><span class='varlabel'>Presence of LRKK2 mutation</span></td>
<td class='firstrow'></td>
</tr>
<tr>
<td class='rowlabel'>G2019S</td>
<td>2 (0.0%)</td>
</tr>
<tr>
<td class='rowlabel lastrow'>Missing</td>
<td class='lastrow'>24620 (100.0%)</td>
</tr>
<tr>
<td class='rowlabel firstrow'><span class='varlabel'>Presence of ATC mutation</span></td>
<td class='firstrow'></td>
</tr>
<tr>
<td class='rowlabel'>Yes</td>
<td>2545 (10.3%)</td>
</tr>
<tr>
<td class='rowlabel'>No</td>
<td>12116 (49.2%)</td>
</tr>
<tr>
<td class='rowlabel lastrow'>Missing</td>
<td class='lastrow'>9961 (40.5%)</td>
</tr>
</tbody>
</table>
</div><!--/html_preserve-->




## Including Plots

$$ Y = \beta_0 + \beta_1*X $$




You can also embed plots, for example:

#```{r data cleaning, echo=FALSE}
head(rawdata)
rawdata %>%  slice(40:50) %>% 
  select(starts_with("age")) %>% 
  filter(age_study > 80) %>% 
  rename (age = age_study) %>% 
  mutate(age = age/10) %>% 
  group_by() %>% summarize() %>%
  merge()
  table1()
  write_csv()%>%
  #function() %>%
  to_lower() %>%
  arrange(desc()) %>%
  count()
  
  # Go ahead and save this data in your package, name it as cleandata.
  # cleandata()
  # 
```

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.
