---
title: "Brain Haemorrhage Detection"
excerpt: "Brain Haemorrhage Detection"
permalink: /portfolio/brain
search: true
gallery:
  - url: /assets/images/brain.jpg
    image_path: /assets/images/brain.jpg
    alt: "Results image 1"
toc: true
author_profile: true
---
Developed a brain hemorrhage detection and localization system to identify intracranial hemorrhages. Three models were analyzed, with their performance metrics evaluated, leading to the selection of ResNet150 for its superior effectiveness in identifying intracranial hemorrhages. Six windowing methods were implemented, and after thorough analysis, the sigmoid BSB method was determined to be the most effective. The system involved preprocessing data from a CSV file, matching it with the SOP Instance UID, and subsequently opening the corresponding DICOM images and labels for further analysis. This project was a collaborative effort between Rushrn Dianayake and me, where we contributed to model selection, performance evaluation, and data preprocessing to enhance the system’s accuracy and efficiency.

{% include gallery caption="Results" %}



