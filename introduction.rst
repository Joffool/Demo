Introduction
============


Purpose
-------
    The purpose of this document is to present a detailed description of the differentially expressed genes analyzing system on which the web application is based. It will explain the purpose and features of the system, the interfaces of the system, what the system will do, the constraints under which it must operate and how the system will react to network outage. This document is intended for both the users and the developers of the system.


Scope of Project
----------------
    This software system will be a Genes Analyzing System for biologists, scientists and other researchers who are dealing with differentially expressed genes and in need of analyzing them via visual charts. This system will be designed to provide an automatically generated scatter plot after visualizing the raw data uploaded by users. By maximizing the users’ work efficiency and production the system will meet the users’ needs while remaining easy to understand and use.


Glossary
--------
================================  ==================================================================
  Term                                                       Definition
================================  ==================================================================
 Control sample                      A cell sample in its original condition.
 Treatment sample                    A cell sample treated by specific chemicals, or of which some genes are altered.
 Differentially expressed genes      The genes which have significantly different expression levels between two samples.
 Up-regulation                       A gene is said to be up-regulated if it has higher expression in treatment than in control.
 logFC                               log fold change of gene expression. Log2 (T/C), where T is the gene expression level from a treatment sample, and C is the gene expression level from a control sample0
================================  ==================================================================
