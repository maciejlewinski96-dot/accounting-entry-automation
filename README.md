# SAP Journal Posting Automation

## Overview

This repository presents a process improvement initiative focused on automating repetitive month-end journal postings into SAP.

The initiative originated from an operational issue observed during the month-end close process, where accounting teams received multiple recurring journal entries from internal teams that required manual posting.

Because many of these entries followed a similar structure each month, an opportunity for automation was identified.

The project documentation includes:

1. Process diagram
2. Process analysis
3. Business requirements
4. Automation logic
5. Exception handling

## Business Context

During month-end close, the finance team received approximately 30 recurring journal entry requests over a period of several days.

These entries were typically provided as CSV files and required manual posting into SAP.

Although the structure of these entries was similar each month, they still required repetitive manual input in SAP.

## Problem

The manual process created several operational challenges:

- repetitive manual SAP postings,
- high operational workload during month-end close,
- frequent interruptions caused by incoming posting requests,
- risk of manual input errors,
- inefficient use of analyst time.

## Objective

The objective of the initiative was to automate recurring journal postings using a bot capable of reading structured input files and posting entries into SAP.

The goal was to reduce manual workload, improve process efficiency, and allow analysts to focus on higher-value tasks.

## My Role

My contribution to the initiative included:

- identifying recurring journal postings suitable for automation,
- analyzing the existing month-end posting workflow,
- defining the automation logic for processing CSV input files,
- collaborating with developers on solution design,
- supporting testing of the automation and identifying inconsistencies during test runs.

## AS-IS Process

1. Internal teams send recurring journal entries as CSV files.
2. Finance analyst reviews the input file.
3. Analyst logs into SAP manually.
4. Journal entries are entered manually into SAP.
5. Posting parameters are verified.
6. Entry is posted.
7. Process is repeated for each request received.

Over several days during month-end close, analysts could receive around 30 such requests.

## TO-BE Process

1. Internal teams provide journal entry data in CSV format.
2. Automation bot reads the CSV input file.
3. Bot validates required posting fields.
4. Bot logs into SAP.
5. Bot posts recurring journal entries automatically.
6. If validation errors occur, an error notification is sent by email.
7. Analyst reviews the error and either corrects the file or performs manual posting.

## Exception Handling

If the bot detects inconsistencies or missing data, it sends an automated email notification describing the issue.

The analyst can then either:
- correct the input file and rerun the process, or
- perform manual posting if required.

## Expected Benefits

The automation initiative aimed to achieve:

- reduction of repetitive manual work,
- smoother month-end workflow,
- fewer interruptions during close activities,
- reduced risk of manual posting errors,
- better use of analyst capacity.

## Skills Demonstrated

- business process analysis
- automation opportunity identification
- requirements definition
- collaboration with development teams
- finance process improvement
- exception handling design

## Note

This repository is a portfolio example prepared for professional presentation purposes and does not contain any confidential company information.
