---
nav_title: Heap
article_title: Heap
page_order: 1

description: "This article details the integration between Braze and Heap"
alias: /partners/heap/

page_type: partner
search_tag: Partner
hidden: true

---

# Heap

> [Heap](https://heap.io/) In this first section, include a brief description of your company. Also, include a link to your main site. TODO - is this something Heap should provide?

The Braze and Heap integration enables you to both [import Heap data to Braze](#data-import-integration) and create segments as well as [export braze data to Heap](#data-export-integration). 

## Prerequisites

| Requirement | Description |
| ----------- | ----------- |
| Heap account | A [Heap](https://heap.io/about) account is required to take advantage of this partnership. |
| Braze REST API key | A Braze REST API key with `users.track` permissions. <br><br> This can be created within the **Braze Dashboard > Developer Console > REST API Key > Create New API Key**. |
| Braze REST endpoint | [Your REST endpoint URL][1]. Your endpoint will depend on the Braze URL for your instance. |
| Braze Currents | In order to export data frpm Braze to Heap, you will need [Braze Currents]({{site.baseurl}}/user_guide/data_and_analytics/braze_currents/#access-currents) enabled on your account.
{: .reset-td-br-1 .reset-td-br-2}

## Use cases

Use cases can be a critical part of your documentation. Although optional, this is a good place to outline typical or even novel use cases for the integration. This can be used as a way to sell or upsell the relationship - it provides context, ideas, and most importantly, a way to visualize the capabilities of the integration.

## Data import integration

Use the Heap to Braze integration in order to automatically sync data from Braze Currents to Heap. 

### Step 1: Get the Braze data import key

In Braze, click on **Technology Partners** and then select Heap. On this page you can find your data import key as well as a REST Endpoint. Take note of both of these values and provide them to your Heap account manager to finish setting up the integration. 

### Step 2: Segment imported users in Braze

In Braze, navigate to **Segments** under **Engagement** and click "Create Segment". After providing a name and optional description to your segment, click "Create Segment" again. On the segment details page, you can add a new filter and select "Heap Cohorts" followed by whichever Heap segment you would like to track.

## Data export integration

Use the Braze Currents in order to automatically sync data from a Heap segment to an equivalent Braze Cohort. 

### Step 1: Get Heap Credentials

You'll need a webhook endpoint URL in order to configure this integration, which you can get from your Heap account manager.

### Step 2: Configure Braze Currents

In Braze, navigate to **Currents** in the **Integrations** section, click "Create New Current", and then select "Custom Currents Export". Give your export a name and then proceed to the Current Details page. On this page, you'll need to enter the endpoint and optional bearer token (if provided) in the Credentials section.

After you've configured your integration's credentials, select all message engagement events as well as customer behavior and user events that you would like to export to Heap, and then click "Update Current".


[1]: {{site.baseurl}}/developer_guide/rest_api/basics/#endpoints