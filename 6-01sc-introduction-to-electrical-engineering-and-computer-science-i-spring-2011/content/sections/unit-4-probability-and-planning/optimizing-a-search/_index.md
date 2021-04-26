---
course_id: 6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011
layout: course_section
menu:
  leftnav:
    identifier: da41172cd83b25719eaecaa5c1bcde32
    name: Optimizing a Search
    parent: f216c72df5191296c53119833fb7c73a
    weight: 430
parent_title: 'Unit 4: Probability and Planning'
title: Optimizing a Search
type: course
uid: da41172cd83b25719eaecaa5c1bcde32

---

« [Previous]({{< baseurl >}}/sections/unit-4-probability-and-planning/search-algorithms) | [Next]({{< baseurl >}}/sections/final-exam) »

Session Overview
----------------

| ![Illustration of the Manhattan distance.](/coursemedia/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/fda65a5c1968cceb16198e8186c90464_13.jpg) |  {{< br >}}{{< br >}} In the last session, we introduced the concept of search. We looked at the 6.01 implementation of a general search algorithm, addressed issues of common sense and dynamic programming, and localized a robot. {{< br >}}{{< br >}} In this session, we focus on improving search. We can systematically use information we have about the state space we're searching, in order to save us time and space. {{< br >}}{{< br >}} The overview handout provides a more detailed introduction, including the big ideas of the session, key vocabulary, what you should understand (theory) and be able to do (practice) after completing this session, and additional resources. {{< br >}}{{< br >}} *   [Session 13 Handout: Optimizing a Search (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/optimizing-a-search/mit6_01scs11_ses13) {{< br >}}{{< br >}}  

Session Content
---------------

### Readings

Read sections 8.5-8.6 of the course notes.

*   [Chapter 8: Long-Term Decision-Making and Search (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/optimizing-a-search/mit6_01scs11_chap08)

### Lecture Video

Watch the lecture video. The handout and slides present the same material, but the slides include answers to the in-class questions.

*   [Lecture 13: Optimizing a Search]({{< baseurl >}}/sections/unit-4-probability-and-planning/optimizing-a-search/lecture-1-object-oriented-programming)

> ### About this Video
> 
> Uniform cost search takes into account the cost associated with an action, and can be implemented with a priority queue. Heuristics estimate the cost of the remaining path to the goal; the Manhattan distance is an example of an admissible heuristic.

*   [Lecture handout (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/optimizing-a-search/mit6_01scs11_lec13_handout)
*   [Lecture slides (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/optimizing-a-search/mit6_01scs11_lec13)

### Recitation Video

These videos have been developed for OCW Scholar, and are designed to supplement the lecture videos.

*   [Recitation 16: Search: Dynamic Programming, Costs and Heuristics]({{< baseurl >}}/sections/unit-4-probability-and-planning/optimizing-a-search/recitation-1-object-oriented-programming)

Session Activities
------------------

The problems in the tables below are taken from the 6.01 Online Tutor, an interactive environment that is not available on OCW. Do not try to answer these questions in the PDF files; answers will not be checked, and cannot be submitted.

### Software Lab

*   [Software Lab 14: Plan from Outer Space (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/optimizing-a-search/mit6_01scs11_swlab14)
*   [Code for Software Lab 14 (ZIP)](/coursemedia/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/01f0f94f591f7020ef718a2dafbc2aaa_swLab14.zip) (This ZIP file contains: 3 .py files.)

| PROBLEM # | QUESTIONS |
| --- | --- |
| 14.1.1 | [Modeling the world (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/optimizing-a-search/mit6_01scs11_14_1_1) |
| 14.1.2 | [Robot on a grid map (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/optimizing-a-search/mit6_01scs11_14_1_2) 

### Design Lab

*   [Design Lab 14: I'm the Map! (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/optimizing-a-search/mit6_01scs11_designlab14)
*   [Code for Design Lab 14 (ZIP)](/coursemedia/6-01sc-introduction-to-electrical-engineering-and-computer-science-i-spring-2011/ac67003a96de8ae44ba6da23e5c9c665_designLab14.zip) (This ZIP file contains: 13 .py files.)

| PROBLEM # | QUESTIONS |
| --- | --- |
| 14.2.3 | [Aliasing instances (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/optimizing-a-search/mit6_01scs11_14_2_3) |
| 14.2.6 | [Robot race results \[optional\] (PDF)]({{< baseurl >}}/sections/unit-4-probability-and-planning/optimizing-a-search/mit6_01scs11_14_2_6) 

« [Previous]({{< baseurl >}}/sections/unit-4-probability-and-planning/search-algorithms) | [Next]({{< baseurl >}}/sections/final-exam) »