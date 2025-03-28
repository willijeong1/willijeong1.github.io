---
layout: post
title: Reaching out firsthand： Precise prevention of adolescent suicide in South Korea
date: 2022-12-14 12:00:00
description: A proposal to lower South Korean adolescent suicide rates by CBCL-brain/PRS interaction-based risk prediction and precise intervention
tags: suicide machine-learning Korea data-science-in-human-neuroimaging
categories: psychology psychiatry
thumbnail: assets/img/20221214_00.png
---

*** This project was for a term paper in the "Data Science in Human Neuroimaging" course in Fall 2022, led by Dr. Jiook Cha (Department of Psychology, Seoul National University). I worked with two other students majoring in Psychology to devise and analyze the prediction model.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_00.png" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
    </div>
</div>
<div class="caption">
    Reaching out firsthand.
</div>

*** An intriguing finding from this project was that behavioral assessment data showed a striking adeptness, compared to gene and brain imaging data, in generally predicting suicidal ideation. In retrospect, I believe this is an example describing the robust clinical efficacy of the current symptom-based diagnosis and treatment framework for psychiatric disorders. However, at the same time, it implies that the complex disparity between biological correlates and behavioral manifestations of mental illness, a major unsolved question in psychiatry research, would be nearly impossible to address without refining (or possibly revising) our current conceptualization of psychiatric disorders.

*** Revisiting this originally Korean post in 2024 to translate it for potential international visitors, I again feel heartbroken looking at the still rising adolescent suicide rates in my country. Even the mere thinking of the unfathomable struggles these young people would have went through before deciding to voluntarily end their own life makes me shudder. The most frightening and frustrating part about this is that I, currently living in a society that puts excessive burden on the people but remains to deem mental illness as strictly taboo, can too understand in part why these thousands of already lost souls might have thought of suicide as the last and only option left. Life should not be this way for young South Koreans, or any other person in Korea, or the world for that matter. We need to do something, anything. NOW.

-----

Adolescent suicide has long become a serious societal problem in South Korea. The country is now routinely scoring a disgraceful "first place" in age-adjusted suicide rates in OECD member countries. Suicide takes up the highest proportion in causes of South Korean adolescent death, and this number keeps increasing, leading to a paradoxical rise in suicide despite the decrease in total mortality. In 2021, an average 36.6 people per day committed suicide; that is one person per every 39 minutes. It is downright shocking that, if one lived in a hypothetical apartment complex housing about 4,000 residents, this number would be akin to one neighbor, friend, or family member per year. Moreover, as if this is not devastating enough, the recent lack of social relationship due to COVID-19 has only aggravated suicide rates.

<div class="row mt-3">
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_01_v2.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
</div>
<div class="row mt-3">
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_02_v2.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_03_v2.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
</div>
<div class="caption">
    Adolescent suicide has long become a serious societal problem in South Korea.
</div>

Various attempts have gone underway in South Korea to lower this devastating suicide rate, which does not even seem to budge. For instance, in the capital Seoul, signposts with supportive messages were attached to particular "suicide bridges" on the Hangang River,* and phone booths were installed to connect attempters with suicide helpline service. Another preventive strategy came in the form of educational programs such as the "Watch-Listen-Talk Strategy" and the "Lifesaving Gatekeeper Program," where teenagers and young adults are regularly coached to sense and provide assistance to high-risk peers around them. While these efforts are agreed upon to have valid social impacts in themselves, they are not sufficient in reversing the steep incline of adolescent suicide that continues on. To overthrow this tendency, it is necessary to devise a more direct and precise intervention strategy, considering the characteristics of adolescents that "fall through the safety net."

*Note: The Hangang River flows through the center of the Seoul metropolitan area with over 25 bridges across the 1km-wide (about 0.6 mi) waters. Although the riverbank is well-known for its refreshing scenery and is a perfect picnic spot for many Seoulites, a few bridges across the river are unfortunately recognized as popular "suicide spots" to some.

<div class="row mt-3">
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_04_v2.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_05_v2.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
</div>
<div class="row mt-3">
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_06_v2.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_07_v2.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
</div>
<div class="caption">
    Examples of current attempts to lower adolescent suicide rates in South Korea.
</div>

A notable reason behind the insufficiency of suicide prevention policies in saving lives comes from South Korea's cultural norms regarding the perception of illness. Koreans habitually tend to hide their weaknesses and digress from their true feelings when they speak, which impedes opportunities for early intervention against many health problems. Espceially in terms of mood disorders - anxiety and depression problems are widespread amid the socioeconomic struggles the country faces - that seldom manifest explicitly, the Korean society often stigmatizes mental health problems and rather attributes them to incompetency or lack of integrity. Since mental illness is strictly considered as taboo in both personal and societal aspects, many patients acknowledge their condition too late and arrive at the clinic in much advanced crises, let alone benefit from early detection.

The steep incline of adolescent suicide in spite of clinically significant preventive measures seems to indicate that an unexpectedly high number of teens and young adults cover up their ideations of suicide and evade timely intervention. Considering the aforementioned cultural indifference to mental illness, preventive educational programs addressing the whole peer group might have proven otherwise for high-risk individuals in South Korea. To elaborate, if these teens and young adults thinking of suicide were led to think that it is "embarrassing" to admit their suffering, these anti-suicide sessions would only have heightened their self pressure in the effort to "fit in" with the others. Furthermore, even if the preventive programs were effective, it is questionnable whether high-risk adolescents had an understanding household environment where they would have had a chance to speak up about their problems. Concerning results from a nationwide survey indeed demonstrated that family members, with whom many teens spent most of their time with before ending their own lives, failed to recognize the warning signals these helpless youth repeatedly sent out.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_08.png" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
    </div>
</div>
<div class="row mt-3">
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_09_v2.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
</div>
<div class="caption">
    A number of teens and young adults may cover up suicidal ideations to "fit in," evading timely intervention.
</div>

An idealistic solution to the South Korean suicide crisis would be to promote social norm changes to allow individuals to acknowledge and seek help for their mental health problems, naturally resulting in adolescents with suicidal ideation receiving assistance as they need. Although this scenario does not seem impossible since younger generations in South Korea are becoming more vigilant towards mental health and well-being, the already devastating suicide rate that keeps rising rapidly by the minute calls for a more immediate approach. Taking into account the societal and cultural insensitivity towards suicidal ideation, the safety net against suicide could be widened by screening "silent" high-risk teens and young adults to intervene adequately. With this rationale, prediction models based on a combination of indirect variables, e.g. questionnaires and biological risk scores, could effectively detect the subtle nonverbal signals pointing to suicide. An investigation to compare and select such appropriate variables would thus provide valuable insights into early detection and prevention of adolescent suicide in South Korea.

-----

To evaluate suicide risk of suicide in adolescents, a good starting point is the differences between children with or without suicidal ideation. For this exemplary investigation, we included demographic information, polygenic risk scores (PRS), brain morphometry, functional magnetic resonance imaging (fMRI) and white matter diffusion MRI (dMRI) data, and child behavior checklist (CBCL) scores.

PRS represents genetic susceptibility to sucidal ideation that one is born with; this susceptibility, however, does not by itself lead directly to suicidal ideation. Inherited genotypes manifest as behavioral characteristics with influence from various environmental variables, and the brain acts as the mediator in the interactions between gene and environment. We employed brain morphometry (regional thickness and curvature) and dMRI data (connectivity in axon-rich white matter) to represent this mediator role. The fMRI data consists of regional activity levels during a "go-no-go" task, which represents the degree of impulse control in making a quick decision to or not to press a button following a given signal.

<div class="row mt-3">
    <div class="col-sm-3 mt-3 mt-md-0">
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_10.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
    </div>
</div>
<div class="caption">
    The brain as the mediator of gene-environmental interactions to determine behavioral characteristics.
</div>

Environmental factors have major influences in the connection from genetic susceptibility to actual intent and commitment of suicide. Unfortunately, a comprehensive index representing infinitely diverse and individual lifestyles is yet to be established, hence we included some basic demographic information such as education level, marital status, and household income. We assumed that scores on the CBCL questionnaire, an intimate behavioral assessment filled out by caregivers, would complement the limitations of demographic data by accounting for environmental influences as incorporated into the child's observable behavior.

Based on the above information, we performed automated machine learning (autoML) with the h2o package on R, a statistical computing software environment, to devise an effective screening model for children with high risk of suicide. Data for each variable was obtained from the ABCD (Adolescent Brain Cognitive Development) Study® on children 9–11 years of age in the United States.* The screening model was trained to predict whether a participant has suicidal ideation (dependent variable) from the indirect variables mentioned above (independent variables). We analyzed 1750 participants who reported suicidal ideation (experimental group) alongside participants without health problems (control group). Independent variables with excessive blank values or zero variance were removed to omit unintended bias in classification, and continuous variables were scaled to means of 0 and standard deviations of 1. For CBCL variables, raw scores (not T-scores) were scaled to allow for integrative analyses with variables from other modalities.

We randomly assigned data for 525 participants (30% of total) to test the efficacy of models; the prediction model was trained on the remaining 1225 participants. This separation of training and testing data ensures high reliability in autoML results. To address overfitting issues where the devised model's prediction criteria adheres specifically to the training dataset and would not be effective to other, real-life datasets, we also randomly organized the training data of 1225 participants into 5 different folds. The autoML process automatically selected and optimized a combination of machine learning algorithms, e.g. generalized linear model (GLM), gradient boosting machine (GBM), deep learning, distributed random forest (DRF), and ensemble learning, to best predict suicidal ideation.

The efficacy of prediction models were compared according to sensitivity and specificity as well as the area under the curve (AUC). To elaborate, sensitivity refers to the proportion of participants with suicidal ideation, which the model successfully predicts the presence of. Specificity refers to the proportion of participants without suicidal ideation, i.e. healthy participants, who are predicted not to have suicidal thoughts. The AUC is calculated from the receiver operating characteristic (ROC) curve, which depicts sensitivity against a given value of false positive rate (the proportion of healthy participants erroneously predicted of having thought of suicide) at each threshold setting.

*Note: Since there were no extensive datasets available for South Korean youth, we accessed the ABCD Study® for a general analysis including various ethnic and cultural backgrounds. By doing this, we also anticipated that the results could not only be applied to Korea, but also similar suicide intervention studies around the world. We strongly assert that establishing a South Korean youth database would immensely assist in national efforts against adolescent suicide.

<div class="row mt-3">
    <div class="col-sm-7 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_11.jpg" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_12_v2.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    (left) Demonstration of the ABCD Study® framework. (right) Outline of autoML for suicide prediction.
</div>

Before training the initial model including all independent variables, we evaluated the predictability of each variable using a univariate GLM. We proceeded on to autoML on selected variables which showed significant predictability in simple linear regression (p < .05). The trained prediction model predicted the dependent variable (suicidal ideation) in a satisfactory manner (AUC = 0.950, sensitivity = 0.816, specificity = 0.990). It was notable that almost all CBCL variables passed the variable selection by solitary predictability and also expressed highly dominant explainability in the initial prediction model. The below right figure depicts that the top 11 variables with highest explainability were all from CBCL.

Meanwhile, contrary to common belief, brain imaging data failed to show meaningful predictability even from the variable selection process. Among brain morphometry, fMRI, and dMRI variables, only 2.57%, 0.29%, and 5.60% respectively were classified as significant. Though some dMRI variables could be distinguished for having moderate predictability, CBCL variables dominated all of these distinct variables by explainability. It is worth mentioning that distinguished dMRI variables pointed to the connectivity between left amygdala and left nucleus accumbens or left lateral orbitofrontal cortex, along with the connectivity between left insula and right middle temporal gyrus. These connections have been reported to constitute circuits related to anxiety, depression, or the reward system. Moreover, fMRI measurement of activity in the left nucleus accumbens also showed significant predictibility alone. Overall, we anticipated that predictability of these variables from brain imaging data would improve when their interactions with PRS - PRS variables had negligible explainability - were included.

<div class="row mt-3">
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_13.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
</div>
<div class="row mt-3">
    <div class="col-sm-3 mt-3 mt-md-0">
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_14_v2.png" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
    </div>
</div>
<div class="caption">
     (left) Explainability for top 20 independent variables in the initial autoML model including all variables. (right) Proportion of selected brain imaging data variables with significant predictability in the univariate GLM (p < .05). GM, WM connectivity, and Task fMRI respectively refer to brain morphometry, dMRI, and fMRI data.
</div>

The striking predictability of CBCL scores on suicidal ideation was robustly reproduced in a different prediction model that included demographic and CBCL variables only (AUC = 0.966, sensitivity = 0.801, specificity = 0.990). Among the CBCL variables, high explainability was attributed to the "broadband" Total Problems score, encompassing internalizing or externalizing problems, alongside the "narrowband" Anxious/Depressed scale. Indeed, incorporated in these assessments are factors reported to be significantly related to suicidal ideation, e.g. dysfunctional behavior, anxiety and depression, and impulsivity.

This led to a new research question: would requesting caregivers to fill out CBCL questionnaires be solely sufficient in precisely and effectively predicting and intervening with suicidal ideation?

-----

The prediction model for suicidal ideation centered on CBCL variables has one detrimental disadvantage: low sensitivity. This simple model has a specificity near 1, which means healthy participants without suicidal ideation are almost always appended the "safe" label. On the other hand, the model's low sensitivity (around 80%) indicates that among participants with suicidal ideation, 1 out of 5 are misunderstood as not having suicidal thoughts and are classified "safe." If this model is directly utilized in real life, it would not only fail to recognize 400 out of 2000 South Korean adolescents thinking of suicide (as of 2020), but would even misjudge them "safe."

Since the CBCL questionnaire obtained from the ABCD Study® requests caregivers' opinions on their children's behavior, it can be inferred that participants producing false negatives, i.e. high-risk individuals misunderstood as not having suicidal thoughts, appear healthy but have internal suffering poorly detected in behavioral traits. Another possibility is the caregiver's inaccurate assessment of their children's abnormal behavior, which lies along the lines of previously described survey results about family members being insensitive to pro-suicide signals in adolescents. With mental problems seldom being expressed in South Korean culture, implementing CBCL-centered prediction in South Korea would lead to even lower sensitivity than as shown with ABCD Study® data from the U.S.

To avoid the potential problems associated with low sensitivity, our next objective was to seek improvement in our prediction model by exploratively accounting for the interactions between CBCL scores and other variables.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_15_v2.png" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
    </div>
</div>
<div class="caption">
     Prediction results on testing data (525 participants) based on demographic and CBCL variables only. The rows indicate presence or absence of suicidal ideation (SI); the columns indicate prediction results. This model's sensitivity is approximately 80%, meaning that among participants with suicidal ideation, 1 out of 5 (in red) end up in false negatives (misunderstood as "safe").
</div>

-----

How, and with what data, could we find "silent" teens and young adults thinking about suicide? The poor efficacy of the CBCL scores in detecting suicidal ideation in these individuals stems from the fact that the "silent" high-risk group is not well distinguished from healthy adolescents in terms of behavior. We hypothesized that for these high-risk individuals, an interaction term for relationships between biological signs (represented by PRS or brain imaging data) and behavioral traits (represented by CBCL scores) would assist in further, more accurate classifcation. For instance, certain behavioral characteristics common between "silent" suicide thinkers and the control group might coincide with a particular biological state A in the former and another biological state B in the latter. We attempted to account for this interaction by exploratively appending to our model several product terms between the existing variables.

Another practical factor to put into consideration is the cost-effectiveness of the screening model. CBCL questionnaires are convenient to request caregivers to fill out, and they are relatively not time-consuming and inexpensive. On the other hand, genomic or brain imaging analyses would not be as convenient and take up more time and resources. Even if genomic or brain imaging analyses significantly increase suicidal ideation predictability when considered along with CBCL scores, these modalities should be administered only for detailed classification.

From the above rationale, the low sensitivity of the CBCL-centered model could be improved by employing PRS and brain imaging data to perform a secondary screening on individuals with no suicidal ideation, i.e. true and false negatives. This method is different from conventional complex screening algorithms that further classify the risk group according to degree of risk, but it is appropriate for suicide prevention where minimizing false negatives is crucial in "tightening the safety net."

<div class="row mt-3">
    <div class="col-sm-1 mt-3 mt-md-0">
    </div>
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_16_v2.png" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-1 mt-3 mt-md-0">
    </div>
</div>
<div class="caption">
     To address low sensitivity issues of the CBCL-centered autoML model, we devised a stepwise, two-phase screening protocol.
</div>

Consequently, we devised a two-phase suicide risk prediction protocol to find "silent" high-risk teens and young adults. In Phase 1, the CBCL-centered prediction model assesses demographic information and CBCL scores of the general adolescent population. Those who are positive for suicidal ideation can immediately arrange for intervention, and those who are negative go through secondary screening (Phase 2). Phase 2 selects "silent" high-risk adolescents with suicidal intent among those initially classified "safe," and these individuals can also benefit from intervention.

We exploratively added product terms between CBCL scores, PRS, and brain imaging data in the autoML model to determine an adequate predictor for Phase 2. The new prediction models were trained and tested as described previously, but we additionally tested the models for adeptness as a Phase 2 screening algorithm. The dataset for additional testing was derived from individuals classified "safe" by the Phase 1 model;* subsequent processing yielded a total 400 participants (26 with suicidal ideation and 374 without).

Below are the efficacy indices of prediction model candidates for Phase 2. When tested with general population data, appending product terms did not produce notable changes in efficacy, and some models were even slightly less effective than the CBCL-centered model. However, additional testing revealed that these models could screen a subgroup of high-risk participants that originally produced false negatives in the CBCL-centered model.

*Note: We used this subset only for testing Phase 2 model candidates because the sample size was too small to both train and test models as described previously without potential reliability and overfitting issues. In future studies, these models could be trained and tested in larger datasets to become more effective in screening "silent" suicide thinkers.

<div class="row mt-3">
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_17_v2.png" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
</div>
<div class="caption">
     Efficacy indices of Phase 2 prediction model candidates. "Brain" indicates all brain imaging data (brain morphometry, fMRI, dMRI). All variables were selected by significant solitary predictability in the univariate GLM (p < .01). Columns labeled "Phase 2" show efficacy indices for additional testing.
</div>

Examining the Phase 2 model candidates that were successful in the additional testing, we discovered that product terms between CBCL and brain imaging variables largely determined the dataset classification. In particular, dMRI data crossed with CBCL scores showed explainability similar to that of CBCL scores alone. This implies that information on white matter connectivity, when associated with behavioral characteristics, could reflect some changes in adolescents with suicidal ideation whose behavior closely resembles those without.

Meanwhile, explainability of CBCL and PRS data product terms was relatively nondominant. Does this mean that PRS itself is not effective in predicting suicidal thoughts? Including triple product terms for PRS, brain imaging, and CBCL data improved the specificity of Phase 2 model candidates; thus PRS data could influence the classifying criteria through interactions with other variables. In fact, interactions between PRS and brain imaging data may explain more of the differences in suicide thinkers than when appended separately. We investigated this effect more directly by generating autoML models including either demographic information, PRS, and brain imaging data or the former plus product terms between PRS and brain imaging data. Indeed, appending PRS-brain imaging interactions as independent variables drove major improvements in the AUC or accuracy (proportion of classified data that match their true designations) indices.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_18_v2.png" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
    </div>
</div>
<div class="caption">
     Appending product terms representing PRS-brain imaging interactions improves model performance.
</div>

In summary of the performances of Phase 2 screening model candidates on additional testing, dMRI data led to discovery of around half of "silent" suicide thinkers, although there was a decline in specificity. However, we could seek improvement in this lowered specificity by including interaction terms regarding PRS, brain morphometry, or fMRI data. PRS and brain imaging data, though with minuscule influences on data classification individually, might have potential in enhancing the accuracy of Phase 2 screening. We selected the best fit Phase 2 models as shown below.

<div class="row mt-3">
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_19_v2.png" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
</div>
<div class="caption">
     Selected models for Phase 2 screening. "Brain" indicates all brain imaging data (brain morphometry, fMRI, dMRI). All variables were selected by significant solitary predictability in the univariate GLM (p < .01). Table below depicts prediction results for each model on additional testing data (400 participants). The rows indicate presence or absence of suicidal ideation (SI); the columns indicate prediction results.
</div>

-----

Given the devastating South Korean adolescent suicide crisis, an effective screening model that predicts suicidal ideation could constitute a more immediate approach to overthrow the steep incline of suicide rates. Here, we propose a two-phase suicide risk prediction model that could serve as a prototype in this approach. An ideal nationwide screening protocol would start with requesting caregivers, guardians, and school teachers to complete CBCL assessments. Then, Phase 1 screening would evaluate suicide risk for the general adolescent population based on that CBCL data as well as demographic information. Subsequently, teens and young adults initially classified not to have suicidal ideation would go through Phase 2 screening, where we would obtain PRS or brain imaging data according to the selected Phase 2 model and include them to discover "silent" suicide thinkers.

One of the advantages this tedious but potentially effective approach has is that we can identify and "reach out firsthand" to teens and young adults suffering in silence. In a culture that tends to be indifferent to mental illness, South Korean adolescents required much time and courage even to make that decision to talk to their caregiver, teacher, or the school counselor, or to walk into the clinic and seek help. Our proposed model aids in reducing that burden of extensive, indecisive rumination by discovering high-risk youth by a census and actively "reaching out." In fact, professionals could possibly engage in visiting sessions in environments more friendly to these individuals, prompting a smooth transition into forming healthy social relationships and learning problem-solving and coping skills along with appropriate pharmacotherapy if needed. This multidimensional therapeutic approach is important because it exceeds beyond the simplistic model of curing, or eliminating, suicidal ideation, which could mislead teens and young adults to view their problems as something embarrassing or something they did wrong. Precise intervention based on a thorough prediction model would minimize this stigma effect especially in South Korea, providing safe grounds for these suffering youth to speak up about their deepest troubles such as anxiety or depression.

On a further note, with the consent of providers, the valuable information obtained from these South Korean adolescents may open windows for future research to shed light on the contributing factors and pathophysiology of suicidal ideation. Developing a Korean version of the ABCD Study® would give rise to studies based on this ethnically and culturally unique population, adding to the existing literature on adolescent suicide as well as various dysfunctional behavior including mood disorders, attention deficit, aggression, and many others.

Even at this hour, there are thousands of beautiful but fragile young South Koreans, and more adolescents around the world, who all are desperately reaching out, looking for someone to really listen to their voices and help them climb out of their suffering. "Reaching out firsthand" means engaging with them hand in hand, resonating with their troubles, and ultimately making a difference in the world for them, and for all of us, to enjoy our lives that we deserve to live to the fullest.

<div class="row mt-3">
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/20221214_20_v2.png" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
</div>
<div class="caption">
    Making a difference.
</div>