---
title: '6 STEPS TO CREATE AN AUTOMATED DATA PIPELINE FOR TABLEAU PUBLIC'
date: 2023-05-15 00:00:00
description: Now you can automatically refresh source data in Tableau Public for free using R, Google Sheets and GitHub Actions.
featured_image: '/images/blog/2023-05-15-tableau-pipeline/tableau-auto-dash.png'
---

![](/images/blog/2023-05-15-tableau-pipeline/tableau-auto-dash.png)

<a href="https://github.com/clarelgibson/tableau-public-autorefresh/wiki" class="button button--large">Go To Tutorial</a>

[Tableau Public](https://public.tableau.com) is a free platform for exploring, creating and publicly sharing data visualizations online. The free-to-use nature of Tableau Public comes with some limitations, one of which is the restriction on scheduled refreshing of the source data for your dashboards. If you have ever developed a Tableau Public dashboard that uses data that changes over time, you may have found yourself manually refreshing your data in the desktop application and then republishing to Tableau Public online.

In a new [tutorial](https://github.com/clarelgibson/tableau-public-autorefresh/wiki), I describe one method of automating the data pipeline, by taking advantage of several additional free-to-use tools:

* [R](https://www.r-project.org) for data extraction, transformation and loading (ETL);
* [Google Sheets](https://www.google.co.uk/sheets/about/) and [Google Drive](https://drive.google.com/drive/u/0/my-drive) for storing the clean data to be supplied to Tableau Public;
* [Github Actions](https://docs.github.com/en/actions) for automatic deployment.

## WHO IS THIS TUTORIAL FOR?

The tutorial uses dummy data generated in R to [illustrate the concepts](https://public.tableau.com/app/profile/clare.gibson/viz/TableauPublicAuto-Refresh/Dashboard) but the use cases are numerous. Any project that uses data that changes frequently (such as from an API) may find benefit from being able to tell Tableau to refresh automatically. I have used this method to build a [dashboard that tracks current inventory](https://public.tableau.com/app/profile/clare.gibson/viz/TeslaM3InventoryUK/Inventory) of used Tesla Model 3 cars in the UK by running a daily query against Tesla’s inventory API and pushing the outputs to a Google Sheet.

The main steps of the tutorial are summarised below, but if you want full details I recommend checking out the tutorial itself.

## STEP 1: SET YOURSELF UP FOR SUCCESS

<a href="https://github.com/clarelgibson/tableau-public-autorefresh/wiki/1.-Getting-started" class="button button--medium">Go To Step 1</a>

To get started you will need:

* a [GitHub](https://github.com) account and repo to store code and manage your workflow. You can choose whether to start from scratch or fork [this one](https://github.com/clarelgibson/tableau-public-autorefresh);
* An R coding environment including the [R language](https://www.r-project.org) and an IDE like [RStudio](https://posit.co);
* a [Google](https://google.com/) account;
* a [Tableau Public](https://public.tableau.com/) account.

## STEP 2: SET UP GOOGLE CLOUD PLATFORM SERVICES

<a href="https://github.com/clarelgibson/tableau-public-autorefresh/wiki/2.-Set-up-GCP-services" class="button button--medium">Go To Step 2</a>

Using [Google Drive](https://drive.google.com/) to store your project data and [Google Cloud Platform](https://cloud.google.com/) for automated authentication means that your scripts can run on a schedule without you being physically present. The tutorial shows you how to set up a GCP account, create a new project and enable to Google Drive API in order to automate your workflow.