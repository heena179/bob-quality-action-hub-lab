# IBM Bob Hands-On Lab: Manufacturing Quality Dashboard

## Lab overview

In this hands-on lab, you will use IBM Bob to understand a set of manufacturing application requirements, create an implementation plan, and build the first version of a manufacturing quality dashboard.

The lab follows a simple development workflow:

1. **Ask mode:** Understand what needs to be built.
2. **Plan mode:** Decide how to build it.
3. **Agent mode:** Build and validate the first version.

> **Important:** All information used in this lab is synthetic. Do not add any production data, source code, credentials, personal information, or other confidential information to the project.

## Business scenario

A fictitious automotive manufacturer wants to improve how its teams monitor production-quality incidents across multiple plants.

The proposed application is called the **Manufacturing Quality Action Hub**. It will help quality and operations teams identify Critical incidents, recognize repeat defects, monitor corrective actions, and view quality trends from a single dashboard.

## Learning objectives

By the end of this lab, you will be able to:

- Use Bob to summarize project requirements.
- Ask Bob to create an implementation plan before changing code.
- Use Bob to build a first application increment.
- Review Bob's output, tests, and implementation summary.
- Understand when to use Ask, Plan, and Agent modes.

## Project files

Download Project Files from ibm.biz/quality-hub-files

Your project folder should contain these three files:

- `01_Manufacturing_Quality_Business_Requirements.docx`
- `02_Functional_Requirements_and_Sample_Data.xlsx`
- `03_Application_Configuration_and_Reference_Data.json`

These files represent information supplied by different stakeholders:

- The **Word document** describes the business problem and goals.
- The **Excel workbook** contains functional requirements and synthetic incident data.
- The **JSON file** contains application configuration, reference values, and business-rule thresholds.

  1. Download and unzip the starter folder
Download the starter folder from ibm.biz/bob-quality-hub to your laptop. Unzip it somewhere easy to find. Unzip the folder and ensure that you have the 3 files in it.

## Before you begin

1. Open the prepared project folder in the IBM Bob development environment.

<img width="440" height="632" alt="image" src="https://github.com/user-attachments/assets/a2478611-f535-4641-b7e4-99683ba55ce9" />

Trust the folder
Bob opens new folders in Restricted Mode until you trust them. You'll see a Restricted Mode badge in the bottom-left status bar.

<img width="508" height="160" alt="image" src="https://github.com/user-attachments/assets/7fab0c64-0147-442e-acb7-4de4cfc64acc" />

Click the badge, then click Trust for the folder. Only trust a folder you downloaded from the event team.

<img width="2310" height="1352" alt="image" src="https://github.com/user-attachments/assets/53c13f9d-08b5-4520-93ad-42735d1ee3d8" />

   
2. Confirm that all three project files are visible in the left pane on your Bob IDE.
   
3. Open the Bob chat panel.

---

## Exercise 1: Understand the requirements with Ask mode

### Goal

Use Bob to understand the project without creating or changing any files.

### Instructions

1. Select **Ask mode**.

Use the mode selector in the chat panel ('+' icon) and choose Ask.

<img width="2878" height="1800" alt="image" src="https://github.com/user-attachments/assets/56d68b49-593d-4d63-bae1-fe4ec960d73f" />

   
2. Copy and submit the following prompt:

```text
Summarize these project requirements in 5 bullets. What are we building, for whom, and what must it do? Do not modify anything.
```

3. Review Bob's response.

### Check your result

Bob's summary should identify:

- The manufacturing-quality application being proposed.
- The primary business users.
- Quality incidents and corrective actions.
- Critical and repeat-defect identification.
- Dashboard, search, filtering, and incident-detail needs.

---

## Exercise 2: Create an implementation plan with Plan mode

### Goal

Ask Bob to determine how the application should be built before it modifies the project.

### Instructions

1. Switch to **Plan mode**.
2. Copy and submit the following prompt:

```text
Create a simple implementation plan for this application using HTML, CSS, and JavaScript and the provided data.

Tell me:
- What we will build
- Recommended architecture
- Key components
- Order of implementation

Keep it under 8 bullets. Do not build anything yet.
```

3.  Bob may ask follow-up questions or approval for actions, please provide the information. 
4.  Review the proposed plan before continuing.

### Check your result

The plan should include:

- A locally runnable web application.
- A simple architecture appropriate for a prototype.
- Dashboard, data, business-logic, and testing components.
- A logical implementation sequence.
- No application files created or modified yet.

### Review point

Before moving forward, confirm that the plan is consistent with the supplied requirements. In a real project, this is where the development team and business stakeholders could adjust the scope or approach.

---

## Exercise 3: Build the first version with Agent mode

### Goal

Use Bob to implement and validate the first version of the application.

### Instructions

1. Switch to **Agent mode**.
2. Copy and submit the following prompt:

```text
Build the first version of the application based on the requirements and plan.

Create a professional manufacturing dashboard with:
- Quality KPIs
- Incidents by plant and severity
- Search and filters
- Critical and repeat-defect indicators
- Incident details

Use the provided data. Keep the solution simple, no frameworks, backend, database, or external APIs. Create an index.html that works directly in the browser.
```

3. Review any actions or file changes proposed by Bob.
4. Allow Bob to complete the implementation.
5. Follow the run instructions Bob provides for the application.

### Check your result

The application should include most or all of the following:

- A clear **Synthetic Demo Data** indicator.
- KPI cards for manufacturing-quality information.
- Incident views by plant and severity.
- Search and filter controls.
- Clear Critical and repeat-defect indicators.
- Incident details and related actions.
- Automated tests for important business logic.
- Setup or run instructions.

> The exact design and technology choices may vary. Focus on whether the application meets the supplied requirements and whether Bob explains what it created.

---


## What the three modes demonstrated

| Mode | Purpose | Simple question |
|---|---|---|
| Ask | Understand without modifying the project | What are we building? |
| Plan | Design and review an approach before implementation | How should we build it? |
| Agent | Create, modify, test, and validate the application | Can you build it? |

Note on Modes : You could use Agent mode for many tasks, but the separate modes make your intention clear and provide useful control over when Bob should only explain, when it should plan, and when it can act.

## Troubleshooting

### Bob cannot find the requirements

Confirm that the Word, Excel, and JSON files are inside the open project folder. Then retry the prompt and explicitly mention the filenames.

### The application does not start

Ask Bob:

```text
Review the startup error, fix the issue, and verify the application runs. Do not change the business requirements.
```

### A test fails

Ask Bob:

```text
Explain the failing test, determine whether the issue is in the test or implementation, fix it, and run the tests again.
```

### The implementation is too complex

Ask Bob:

```text
Simplify the implementation while preserving the required dashboard, search, filters, incident details, and business rules.
```

## Closing discussion

Consider how the same workflow could apply to an existing application:

- Where does your team spend the most time today: understanding, planning, building, testing, or modernization?
- Which application would be a safe candidate for a focused proof of value?
- What standards, approvals, and controls would Bob need to follow in your development environment?

## Lab completion

You have completed the lab when you have:

1. Used Ask mode to summarize the requirements.
2. Used Plan mode to create and review an implementation plan.
3. Used Agent mode to build and validate the first application version.
4. Reviewed the application and its tests.

---

*This lab uses a fictitious automotive manufacturing scenario and synthetic data for demonstration purposes only.*
