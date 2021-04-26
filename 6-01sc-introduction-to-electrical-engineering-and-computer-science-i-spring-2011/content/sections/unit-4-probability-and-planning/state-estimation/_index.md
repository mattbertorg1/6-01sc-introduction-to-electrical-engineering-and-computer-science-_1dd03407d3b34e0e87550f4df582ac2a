---
course_id: 6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011
layout: course_section
menu:
  leftnav:
    identifier: 78921a7ec8e9b114852dcaa46d83fd04
    name: State Estimation
    parent: f216c72df5191296c53119833fb7c73a
    weight: 410
parent_title: 'Unit 4: Probability and Planning'
title: State Estimation
type: course
uid: 78921a7ec8e9b114852dcaa46d83fd04

---

« [Previous]({{< baseurl >}}/sections/unit-4-probability-and-planning/discrete-probability) | [Next]({{< baseurl >}}/sections/unit-4-probability-and-planning/search-algorithms) »

Session Overview
----------------

| ![Diagram of robot estimating its distance from the wall.](/coursemedia/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/8e7d761e1fa51646ffba6ac411acfbde_11.jpg) |  {{< br >}}{{< br >}} In the last session, we introduced probability and the basic tools to interact with probability distributions. We use probability to model degrees of belief, so that we can build systems that are robust in the face of uncertainty. {{< br >}}{{< br >}} In this session, we focus on state estimation. We'll use state estimation to estimate the location of a robot in a hallway, and use it to localize a robot. Later we'll be able to localize and map at the same time. {{< br >}}{{< br >}} The overview handout provides a more detailed introduction, including the big ideas of the session, key vocabulary, what you should understand (theory) and be able to do (practice) after completing this session, and additional resources. {{< br >}}{{< br >}} *   [Session 11 Handout: State Estimation (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_ses11) {{< br >}}{{< br >}}  

Session Content
---------------

### Readings

Read sections 7.5-7.8 of the course notes.

*   [Chapter 7: Probabilistic State Estimation (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_chap07)

### Recitation Video

These videos have been developed for OCW Scholar, and are designed to supplement the lecture videos.

*   [Recitation 14: Probability: State Estimation]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/recitation-1-object-oriented-programming)

Session Activities
------------------

The problems in the tables below are taken from the 6.01 Online Tutor, an interactive environment that is not available on OCW. Do not try to answer these questions in the PDF files; answers will not be checked, and cannot be submitted.

This session contains a design lab from week 11 of the MIT course, and a software lab from week 12.

### Design Lab

*   [Design Lab 11: Robots in Hallways (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_designlab11)
*   [Code for Design Lab 11 (ZIP)](/coursemedia/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/ec06e4ded396a5bf2b6acb495ce96e2f_designLab11.zip) (This ZIP file contains: 1 .py file.)

| PROBLEM # | QUESTIONS |
| --- | --- |
| 11.1.1 | [Observation models (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_11_1_1) |
| 11.1.2 | [Transition models (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_11_1_2) |
| 11.1.4 | [Simulating hallways (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_11_1_4) |
| 11.1.5 | [Simulating hallways: the noisy-noisy case (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_11_1_5) |
| 11.1.6 | [Sonar hit (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_11_1_6) |
| 11.1.7 | [Ideal sonar readings (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_11_1_7) 

### Software Lab

*   [Software Lab 12: I think therefore where am I (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_swlab12)
*   [Code for Software Lab 12 (ZIP)](/coursemedia/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/5e5907831ddf22f02f65b682cc9ce418_swLab12.zip) (This ZIP file contains: 1 .py file.)

| PROBLEM # | QUESTIONS |
| --- | --- |
| 12.2.1 | [Stochastic state machines (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_12_2_1) |
| 12.2.2 | [Faster state estimation (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_12_2_2) |
| 12.2.3 | [Localization (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_12_2_3) 

Check Yourself
--------------

### Nano-Quiz

Nano-quiz problems and solutions are taken from a previous version of the 6.01 Online Tutor. Do not try to answer these questions in the PDF files; answers will not be checked, and cannot be submitted.

*   [Quiz Problem (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_quiz11)
*   [Quiz Solution (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_quiz11_sol)

### Homework

*   [Homework 4: Distributions (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_hw4)
*   [Code for Homework 4 (ZIP)](/coursemedia/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/2af533f161113a318664c482841194be_hw4.zip) (This ZIP file contains: 1 .py file.)

| PROBLEM # | QUESTIONS |
| --- | --- |
| 11.2.1 | [Basic distributions: square (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_11_2_1) |
| 11.2.2 | [Basic distributions: triangle (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_11_2_2) |
| 11.2.3 | [Mixture distribution (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/state-estimation/mit6_01scs11_11_2_3) 

« [Previous]({{< baseurl >}}/sections/unit-4-probability-and-planning/discrete-probability) | [Next]({{< baseurl >}}/sections/unit-4-probability-and-planning/search-algorithms) »