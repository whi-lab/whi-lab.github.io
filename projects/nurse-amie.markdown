---
title: "Nurse AMIE: Using Smart Speakers to Provide Supportive Care Intervention for Women with Metastatic Breast Cancer" # TODO: review project title
layout: page
---

<div class="row">
    <div class="col-md-12">
        <div class="col-xs-offset-1 col-md-10">
            <!-- TODO: find header image (at least 1000 x 527)
                Note: Please be mindful of licensing permissions. The Noun Project (https://thenounproject.com/),
                FreePik (https://www.freepik.com/) and Adobe Stock (https://stock.adobe.com/) are great places to start!
                Google Image results licensed under Creative Commons are also acceptable.
            -->
        </div>
    </div>
</div>

<!-- TODO: review description of project & add external links as needed -->

According to the estimation of American Cancer Society, there are more than 168,000 women living with metastatic breast cancer in the U.S. Metastatic breast cancer (also called stage IV or advanced breast cancer) is the most advanced stage of breast cancer. Although metastatic breast cancer can’t be cured today, it can be treated. Treatment focuses on extending life and maintaining quality of life. A study showed that patients prefer to routinely visit their health care providers in seek of the treatments, which is reasonable considering that the level of patients' symptoms are different, dynamic, and temporal. On the other hand, it generates a significant amount of pressure on hospitals and other health services.

Smart speakers, such as Amazon Alexa and Google Home, have become a quite popular household electronics in the past few years. Although most of the current smart speakers are designed to provide primitive household services and functionalities, such as buying groceries, setting alarms, etc, the embracing of smart speaker based health intervention scheme have become more feasible, accessible and promising than ever before. Comparing to other intervention platforms such as mobile phones, CA is able to produce active information flow in both ways rather than just passive delivery of information. By listening to patients and giving them voice feedback, CAs are expected to be capable of forming a therapeutic alliance with patients.

In this project, our key goal is to develop an Alexa skill, Nurse AMIE, for women with metastatic breast cancer,and produce practical design implications based on the comprehensive analysis of user experience. The latest version of Nurse AMIE has three main features. First of all, Nurse AMIE provides daily educational nutrition tips based on patients’ individual progress. Nurse AMIE keeps track of patients’ daily health status, which are extracted from the dialogue between the two parties. Based on patients’ health status and other factors(e.g. for safety reasons, the exercise treatments from Nurse AMIE vary based on patients’ location of metastasis.), Nurse AMIE offers daily intervention activities, ranging from mental health educational videos to exercise treatments.

Technical Overview: The backend of the Alexa skill is written in Python and is deployed on AWS Lambda. The frontend (interactive visual experience) of the skill is written in Alexa Presentation Language (APL). User data, including health status, skill status and user activity log are stored in Amazon DynamoDB.

## Demo ##
<iframe width="640" height="480" src="https://www.youtube.com/embed/4pKBvTatb9M" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen=""></iframe>

## Papers ##
<!-- TODO: review list of publications -->

* Brett Gordon, **Saeed Abdullah**, Shawna, Doerksen, Abigail Lorenzo, Bethany Kanski, **Ling Qiu**, Kathryn Schmitz. (2022).
[Comparing Two Delivery Modes Of A Supportive Care Platform For Metastatic Breast Cancer Patients][msse-2022].
Journal of Medicine & Science in Sports & Exercise.
* **Ling Qiu**, Bethany Kanski, Shawna Doerksen, Renate Winkels, Kathryn H. Schmitz, **Saeed Abdullah**. (2021).
[Nurse AMIE: Using Smart Speakers to Provide Supportive Care Intervention for Women with Metastatic Breast Cancer][chi-lbw-2021]. CHI LBW.

## Support ##
<!-- TODO: list funding sources (if applicable) -->

Support for this research is provided by [insert grant info here] grant.

## People ##

[Ling Qiu](https://lingqiu3.github.io)  
<!-- TODO: list project team members w/ links to personal websites -->
[Collaborator #1](/404.markdown)  
[Collaborator #2](/404.markdown)  
[Saeed Abdullah](https://saeedabdullah.com)

[msse=2022]: /404.markdown
[chi-lbw-2021]: /files/pubs/ling-nurse-amie-lbw-2021.pdf