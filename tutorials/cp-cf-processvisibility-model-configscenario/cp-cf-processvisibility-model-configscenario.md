---
title: Create a Visibility Scenario for a Deployed Workflow
description: Create a visibility scenario based on a workflow using the Configure Visibility Scenarios application.
auto_validation: true
time: 10
tags: [tutorial>beginner, products>sap-business-technology-platform]
primary_tag: products>sap-business-technology-platform
author_name: Kavya M Gowda
author_profile: https://github.com/I540620
---

## Prerequisites
 1. You have set up SAP Workflow Management service. For more information, see the [Set Up Workflow Management in Cloud Cockpit](cp-starter-ibpm-employeeonboarding-1-setup) tutorial.
 2. You have a deployed workflow. If you do not have a workflow deployed, then refer to steps 5 and 6 in [Configure Business Rules, Workflow and Process Visibility](cp-starter-ibpm-employeeonboarding-2-configure) tutorial.
 3. You have set up business rules for determining equipment. To set up the business rules, see steps 1 to 4 in [Configure Business Rules, Workflow and Process Visibility](cp-starter-ibpm-employeeonboarding-2-configure) tutorial.

## Details
### You will learn
  - How to use the Configure Visibility Scenarios application
  - How to create a visibility scenario by adding workflows
  - How to activate a visibility scenario  

Visibility scenarios allow you to track the performance of end-to-end processes. You can configure the aspects of a scenario such as events and context of the processes, correlation conditions, status, attributes, and performance indicators for the end-to-end processes of a scenario.

In this tutorial, you will learn how to add a workflow to your visibility scenario to gain visibility on the workflow. In this tutorial we create a visibility scenario named **Employee Onboarding Process** and then add the **onboard** workflow from workflow capability as a process participant to the  visibility scenario. For more information, see [Creating a Scenario](https://help.sap.com/viewer/62fd39fa3eae4046b23dba285e84bfd4/Cloud/en-US/df284fd12073454392c5db8913f82d81.html).

---

[ACCORDION-BEGIN [Step 1:](Create a scenario)]
1. Open the **Workflow Management** dashboard and choose the **Configure Visibility Scenarios** tile present under **Development Tools**.

    !![Home screen](config-flp.png)

2. Create a visibility scenario by choosing the **+** icon.

    !![Add scenario](Config-Step1-plus.png)

3. In the **New Scenario** dialog, provide a **Name** and optionally a description for the scenario and choose **Create**. On providing the name, the **ID** field gets populated automatically.

    !![visibility scenario name](scenario-name.PNG)

    You can see the **Employee Onboarding Process** scenario listed in the **Scenarios** table in **Draft** state.

4. Now, select the **Employee Onboarding Process** scenario in the **Draft** state to edit it.

    !![Draft](Config-Step1-draft.png)

[VALIDATE_1]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 2: ](Add workflow to the Visibility scenario)]

In this step, you will add the **onboard** workflow to your **Employee Onboarding Process** scenario.

1. Under the **Processes** tab, choose the **+** icon and then choose **Add Workflow from SAP Workflow Service** to add a workflow to the visibility scenario.

    !![import workflow](Add-workflow.png)

2. In the **Add Workflow from SAP Workflow Service** dialog, choose the workflow named **onboard**.

    !![Choose workflow](onboard.png)

    Now, the workflow is added as a process participant to your visibility scenario. By default all the events provisioned by the workflow along with the corresponding context of is added into the visibility scenario.

    >Check the default **State**, **Status**, **Attributes**, and **Performance Indicators** that are pre-created for the given workflow.

3. **Save** the changes.

    !![After import](Config-Step1-onboardafter.png)

  You have now created an **Employee Onboarding Process** visibility scenario with an **onboard** workflow as a process participant.

[DONE]
[ACCORDION-END]



---
