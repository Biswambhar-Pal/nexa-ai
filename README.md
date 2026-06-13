# Nexa.ai

## 🚀 Agentic Pre-Development Workspace for Enterprise Delivery Teams

**Nexa.ai** is an AI-powered pre-development workspace built by **Team Nexa**. It helps enterprise delivery teams convert raw requirement discussions, meeting transcripts, and business notes into structured, reviewable, and delivery-ready artifacts such as BRDs, user stories, technical design notes, estimates, QA test cases, and approval records.

---

## 🧩 Project Information

| Item | Details |
| :--- | :--- |
| **Team Name** | Nexa |
| **Product Name** | Nexa.ai |
| **Theme** | AI at Work: Productivity and Teamwork Reimagined |
| **Primary Platform** | Microsoft Power Platform |
| **Frontend** | Microsoft Power Pages |
| **Workflow Orchestration** | Microsoft Power Automate |
| **AI Agent Layer** | Microsoft Copilot Studio |
| **Prompt Layer** | AI Prompts |
| **Data Layer** | Microsoft Dataverse |
| **Identity** | Microsoft Entra ID |
| **Delivery Integration** | Jira |

---

## 🎯 1. Project Description and Context

### Problem Statement

Enterprise delivery teams spend significant time converting early requirement conversations into execution-ready delivery artifacts.

During pre-development discussions, business stakeholders, business analysts, scrum masters, technical leads, developers, and QA teams usually collaborate through meetings, chats, documents, and transcripts. However, after the discussion ends, the actual delivery preparation often becomes fragmented.

Key information such as business requirements, acceptance criteria, design assumptions, open questions, estimates, risks, dependencies, and QA scenarios may be spread across meeting notes, transcripts, emails, documents, and manual trackers.

This creates a major pre-development gap:

- Requirement context is lost between discussion and execution.
- Business analysts spend hours preparing BRDs and requirement summaries.
- Scrum teams manually convert requirements into epics and user stories.
- Technical leads recreate design assumptions from scattered notes.
- QA teams receive test coverage context late in the delivery cycle.
- Delivery teams struggle to maintain traceability from discussion to implementation.

The business value of a requirement discussion is highest immediately after the conversation. However, many teams spend hours or days reconstructing the context before development can begin.

---

## 💡 2. The Nexa.ai Solution

**Nexa.ai** solves this problem by providing an AI-powered workspace for pre-development automation.

Users can create a project, upload requirement transcripts or business discussion notes, and allow Nexa.ai to process the content through an agentic AI pipeline.

Nexa.ai then generates structured, role-specific artifacts for delivery teams, while keeping human reviewers in control through approval workflows.

The platform is designed to help teams move from:

```text
Raw business conversation → Structured requirement intelligence → Human-reviewed delivery artifacts
```

Nexa.ai does not simply summarize meeting transcripts. It creates a governed and traceable pre-development workspace where every generated output can be connected back to the original project and transcript source.

---

## 📈 3. Expected Business Impact

Nexa.ai is designed to deliver measurable productivity improvements during the pre-development phase.

### Expected Impact Areas

- **Cycle Time Reduction:** Accelerates the time required to convert raw meeting transcripts into baseline delivery artifacts.
- **Manual Effort Reduction:** Reduces repetitive documentation, formatting, and handoff work across BA, Scrum, Tech Lead, and QA roles.
- **Improved Traceability:** Maintains relationships between projects, transcripts, generated artifacts, reviews, and approvals.
- **Better Delivery Readiness:** Gives each delivery role a structured starting point before development begins.
- **Human-in-the-Loop Governance:** Ensures that AI-generated artifacts are reviewed, approved, rejected, or regenerated before downstream use.
- **Reusable Enterprise Pattern:** Demonstrates how Microsoft Power Platform can support secure, scalable, AI-assisted business process automation.

```
For Business Users, this means less time searching and more time making decisions.

For Project Teams, this means every requirement has context, source, status, and approval history.
```
---

## 🏗️ 4. Architecture Overview

Nexa.ai follows a four-layer Microsoft Power Platform architecture.

```text
┌─────────────────────────────────────────────────────────────────────┐
│ 1. Experience Layer                                                  │
│ Microsoft Power Pages                                                │
│ - Secure web workspace                                               │
│ - Project creation                                                   │
│ - Transcript upload                                                  │
│ - Dashboards and review screens                                      │
└───────────────────────────────┬─────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────┐
│ 2. Workflow Layer                                                    │
│ Microsoft Power Automate                                             │
│ - Intake orchestration                                               │
│ - Status tracking                                                    │
│ - AI processing coordination                                         │
│ - Approval routing                                                   │
│ - Notification and integration flows                                 │
└───────────────────────────────┬─────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────┐
│ 3. Intelligence Layer                                                │
│ Microsoft Copilot Studio and AI Prompts                              │
│ - Agent-based processing                                             │
│ - Role-specific artifact generation                                  │
│ - Prompt-driven structured extraction                                │
│ - Validation and quality checks                                      │
└───────────────────────────────┬─────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────┐
│ 4. Data and Governance Layer                                         │
│ Microsoft Dataverse, Microsoft Entra ID                              │
│ - Project and transcript data                                        │
│ - Artifact metadata                                                  │
│ - Review and approval history                                        │
│ - Secure document storage                                            │
│ - Identity and access control                                        │
└─────────────────────────────────────────────────────────────────────┘
```

---

## 🔄 5. End-to-End Solution Workflow

### Step 1: Project Creation

A user signs in to the Nexa.ai workspace through the Power Pages portal and creates a new project.

The project record is stored in Microsoft Dataverse with key metadata such as project name, owner, business context, status, and created date.

---

### Step 2: Transcript Upload

The user uploads a meeting transcript, requirement document, or business discussion note.

Supported input formats can include:

- TXT
- DOCX (Coming soon)
- PDF (Coming soon)
- Meeting transcript exports

The uploaded file is linked to the project and stored securely.

---

### Step 3: Intake and Metadata Tracking

Power Automate triggers the intake pipeline.

The flow records the transcript metadata in Dataverse and updates the processing status.

Typical statuses include:

- Submitted
- Ingestion Started
- AI Processing
- Draft Generated
- Pending Review
- Approved
- Rejected

---

### Step 4: AI Ingestion and Context Analysis

The transcript content is processed using AI prompts and Copilot Studio agent logic.

The AI processing layer extracts key information such as:

- Business goals
- Functional requirements
- Non-functional requirements
- Decisions
- Assumptions
- Constraints
- Risks
- Dependencies
- Open questions
- Stakeholder action items

---

### Step 5: Role-Based Artifact Generation

Nexa.ai uses role-specific AI prompt patterns to generate artifacts for different delivery roles.

Generated outputs may include:

- Business Requirement Document
- Epics, User stories
- Acceptance criteria
- Technical design notes
- Data model suggestions
- API and integration considerations
- QA test scenarios
- Positive and negative test cases
- Open question register
- Risk and dependency summary
- Developer guidance

---

### Step 6: Validation and Quality Review

A validation step reviews the generated outputs for completeness and consistency.

The validation layer checks for:

- Missing requirement details
- Ambiguous statements
- Conflicting assumptions
- Incomplete acceptance criteria
- Missing QA coverage
- Weak traceability to transcript content

A readiness score or validation status can be stored in Dataverse for reviewer visibility.

---

### Step 7: Human Approval Workflow

Generated artifacts are routed to reviewers using Power Automate approval workflows.

Reviewers can:

- Approve the generated artifact
- Reject the artifact with comments
- Request regeneration
- Add reviewer notes
- Track approval history

This ensures that AI assists the delivery team but does not bypass human governance.

---

### Step 8: Export and Downstream Integration

After approval, artifacts can be exported or synchronized with delivery tools.

Possible outputs include:

- Text documents
- Word documents ```(Coming soon)```
- PDF packages ```(Coming soon)```
- Structured JSON ```(Coming soon)```
- Jira backlog items ```(Coming soon)```


---

## 🤖 6. AI Agent and Prompt Design

Nexa.ai uses persona-based prompt design to generate outputs aligned with enterprise delivery roles.

### Transcript Intake Agent

Responsible for cleaning and structuring raw transcript content.

Primary functions:

- Remove meeting noise
- Identify discussion context
- Extract key decisions
- Capture assumptions
- Identify unresolved questions
- Prepare normalized content for downstream agents

---

### Business Analyst Agent

Responsible for business requirement generation.

Primary outputs:

- Business Requirement Document
- Business objectives
- In-scope and out-of-scope items
- Functional requirements
- Non-functional requirements
- Acceptance criteria
- Business rules
- Stakeholder questions

---

### Scrum Agent

Responsible for agile delivery breakdown.

Primary outputs:

- Epics
- User stories
- Acceptance criteria
- Subtasks
- Priority recommendations
- Story point estimate suggestions
- Sprint readiness notes

---

### Technical Lead Agent

Responsible for technical interpretation and design guidance.

Primary outputs:

- Technical design notes
- Architecture considerations
- Data entity recommendations
- Integration considerations
- API contract suggestions
- Development checklist
- Technical risks and dependencies

---

### QA Agent

Responsible for test planning and coverage mapping.

Primary outputs:

- Test scenarios
- Positive test cases
- Negative test cases
- Boundary test cases
- Regression considerations
- Requirement-to-test mapping

---

### Validator Agent

Responsible for quality control and governance checks.

Primary outputs:

- Completeness score
- Risk indicators
- Missing information report
- Contradiction detection
- Artifact readiness recommendation
- Regeneration suggestion, if required

---

## 💻 7. Technology Stack

| Layer | Microsoft / Platform Component | Purpose |
| :--- | :--- | :--- |
| Experience Layer | Microsoft Power Pages | Provides the web-based user workspace for project creation, transcript upload, dashboards, and review screens. |
| Identity Layer | Microsoft Entra ID | Supports secure authentication and identity-based access. |
| Workflow Layer | Microsoft Power Automate | Orchestrates intake, AI processing, status updates, notifications, approvals, and integrations. |
| AI Agent Layer | Microsoft Copilot Studio | Provides the agent experience and coordinates AI-driven interactions. |
| Prompt Layer | AI Prompts | Processes transcripts and generates structured role-based outputs. |
| Data Layer | Microsoft Dataverse | Stores project data, transcript metadata, generated artifacts, approval records, and operational tracking. |
| Delivery Integration Layer | Jira | Supports downstream synchronization of approved work items into delivery tools. |

---

## 🗂️ 8. Core Data Model

Nexa.ai uses Dataverse as the structured data backbone.

### Key Tables

| Table | Purpose |
| :--- | :--- |
| Nexa Project | Stores project-level information and ownership details. |
| Nexa Transcript | Stores uploaded transcript metadata and source reference details. |
| Nexa Artifact | Stores AI-generated outputs such as BRDs, user stories, test cases, and technical notes. |
| Nexa Approval | Stores review decisions, comments, approval status, and reviewer information. |
| Nexa Prompt Version | Stores prompt versioning information for governance and auditability. |
| Nexa Processing Log | Tracks pipeline execution, errors, timestamps, and status transitions. |

### Key Relationships

- One project can have multiple transcripts.
- One transcript can generate multiple artifacts.
- One artifact can have multiple approval records.
- Each artifact can reference the prompt version used during generation.
- Each processing event can be tracked through pipeline logs.

---
## 🧪 9. Demo Access and Live Demo Flow

This section is intended for hackathon evaluators, judges, and non-technical reviewers who want to access the Nexa.ai portal and run through the product experience.

### 9.1 Portal URL

Open the Nexa.ai portal using the link below:

```text
https://nexa-ai-enterprise-portal.powerappsportals.com/
```

If the link does not open immediately, copy the URL and paste it into a browser address bar.

Recommended browsers:

- Microsoft Edge
- Google Chrome

For the cleanest demo experience, use a private browser session:

- In Microsoft Edge: **InPrivate window**
- In Google Chrome: **Incognito window**

This helps avoid conflicts with any Microsoft account that may already be signed in on the evaluator's browser.

---

### 9.2 Demo Sign-In Credentials

Use the following demo account to access the portal:

```text
Username: microsoftbuildai@biswapal.onmicrosoft.com
Password: MNexa@2026
```

> **Important security note:** These credentials are intended only for hackathon evaluation and demo access. The account should not be used with production data. The password should be changed or the account should be disabled after the evaluation window is completed.

---

### 9.3 Step-by-Step Sign-In Guide

Follow these steps carefully to sign in to the Nexa.ai portal.

#### Step 1: Open the Portal

1. Open Microsoft Edge or Google Chrome.
2. Paste the portal URL into the address bar:

```text
https://nexa-ai-enterprise-portal.powerappsportals.com/
```

3. Press **Enter**.
4. Wait for the Nexa.ai portal home page to load.

#### Step 2: Start Sign-In

1. Click **Sign in** on the portal page.
2. If the portal shows multiple sign-in options, select the Microsoft or organizational account sign-in option.
3. When the Microsoft sign-in page appears, enter the demo username:

```text
microsoftbuildai@biswapal.onmicrosoft.com
```

4. Click **Next**.
5. Enter the demo password:

```text
MNexa@2026
```

6. Click **Sign in**.

---

### 9.4 Microsoft Authenticator Setup for First-Time Login

During first-time sign-in, Microsoft may ask for additional security setup. This is normal. The evaluator may see a message such as:

```text
More information required
```

or

```text
Your organization needs more information to keep your account secure
```

If this appears, follow the steps below.

#### What is needed

The evaluator needs:

- A laptop or desktop browser where the portal sign-in page is open.
- A smartphone with internet access.
- The Microsoft Authenticator mobile app installed on the smartphone.

#### Step 1: Install Microsoft Authenticator

1. On the smartphone, open the official app store:
   - **iPhone:** App Store
   - **Android:** Google Play Store
2. Search for:

```text
Microsoft Authenticator
```

3. Install the app published by **Microsoft Corporation**.
4. Open the app after installation.
5. If the phone asks for notification permission, allow notifications. This helps the app show approval prompts during sign-in.

#### Step 2: Continue Setup on the Browser

1. On the browser sign-in page, click **Next** when the additional security setup message appears.
2. Microsoft may show a page explaining that the Authenticator app is required.
3. Click **Next** again until a QR code appears on the browser screen.
4. Do not close this browser window. The QR code displayed on this page will be scanned from the phone.

#### Step 3: Add the Demo Account in Microsoft Authenticator

1. On the smartphone, open the **Microsoft Authenticator** app.
2. Tap **Add account** or the **+** icon.
3. Select **Work or school account**.
4. Select **Scan QR code**.
5. If the phone asks for camera permission, allow camera access.
6. Point the phone camera at the QR code shown on the browser screen.
7. Wait until the account is added successfully in the Authenticator app.

The account name should appear similar to:

```text
microsoftbuildai@biswapal.onmicrosoft.com
```

#### Step 4: Complete Verification

1. Return to the browser.
2. Click **Next**.
3. Microsoft may send a test approval request to the Authenticator app.
4. On the phone, open the notification from Microsoft Authenticator.
5. If the browser shows a number, enter the same number in the Authenticator app.
6. Tap **Yes** or **Approve** in the Authenticator app.
7. Return to the browser.
8. Click **Next** or **Done** when setup completes.

After this step, the evaluator should be signed in to the Nexa.ai portal.

---

### 9.5 If QR Code Scanning Does Not Work

If the smartphone camera cannot scan the QR code:

1. On the browser setup page, select **Can't scan image** or **I can't scan the QR code** if that option appears.
2. Microsoft will show a manual setup code and URL.
3. In the Authenticator app, choose the manual entry option.
4. Enter the code shown on the browser screen.
5. Continue with verification.

If the setup still fails, close the browser, open an InPrivate or Incognito window, and start the sign-in process again.

---

### 9.6 Common Sign-In Troubleshooting

#### Issue: Browser automatically signs in with another Microsoft account

Use an InPrivate or Incognito window and try again.

#### Issue: Password is rejected

Carefully copy the password exactly as provided. Check for extra spaces before or after the password.

#### Issue: Authenticator approval request is not visible

Open the Microsoft Authenticator app manually and check for the pending approval request.

#### Issue: Number matching screen appears

Enter the number shown on the browser into the Microsoft Authenticator app, then approve the request.

#### Issue: QR code expired

Go back one step in the browser or restart the sign-in process to generate a new QR code.

#### Issue: Account was added incorrectly in Authenticator

Remove the incorrect account from Microsoft Authenticator and repeat the QR code setup process.

---

### 9.7 Recommended Live Demo Journey

After successful sign-in, use the following path to review the product.

#### 1. Home Page

The home page introduces Nexa.ai as an AI-powered pre-development workspace. It provides the entry point for project creation, transcript ingestion, pipeline tracking, approvals, and admin controls.

#### 2. Dashboard

The dashboard provides a consolidated view of project activity, transcript processing, generated artifacts, review status, and approval progress.

#### 3. New Project

Use the **New Project** page to create a project workspace. The project becomes the parent record that connects transcripts, generated artifacts, approvals, and processing history.

#### 4. Transcript Upload

Upload a requirement discussion transcript, meeting note, or business input document. Nexa.ai uses this content as the source for AI-assisted pre-development artifact generation.

#### 5. Processing Pipeline

Open the pipeline view to track the status of ingestion and AI processing. The pipeline shows how the transcript moves from submitted input to structured draft output.

#### 6. Generated Artifacts

Review the AI-generated artifacts such as requirement summaries, user stories, technical notes, QA scenarios, and open questions. Each artifact is linked back to the project and source transcript.

#### 7. Approvals

Open the approval screen to review, approve, reject, or request changes to generated artifacts. This demonstrates the human-in-the-loop governance model.

#### 8. Admin Console

Use the admin console to review operational controls such as prompt versioning, pipeline configuration, processing status, and governance settings.

---

### 9.8 Suggested Demo Talk Track

Use the following short talk track while showing the portal:

```text
Nexa.ai starts with a secure Power Pages portal where business users can create a project and upload requirement transcripts.

Once a transcript is submitted, Power Automate orchestrates the ingestion pipeline, stores metadata in Dataverse, and triggers the AI processing layer.

Copilot Studio agents and AI prompts then convert the raw business discussion into structured delivery artifacts for business analysts, scrum teams, technical leads, and QA teams.

The generated outputs remain connected to the original project and transcript, giving teams traceability from discussion to execution.

Before anything is exported or synchronized downstream, reviewers can approve, reject, or request changes through a human-in-the-loop approval process.

This makes Nexa.ai a governed AI workspace for turning scattered requirement conversations into delivery-ready intelligence.
```

---

## 🔐 10. Security and Governance

Nexa.ai is designed with enterprise governance principles in mind.

### Security Considerations

- Users authenticate through Microsoft Entra ID.
- Power Pages access is controlled through web roles and table permissions.
- Dataverse security roles manage access to project, transcript, artifact, and approval data.
- Prompt versions are tracked to support auditability.
- Approval history is stored for governance and compliance review.
- Generated outputs require human approval before export or downstream synchronization.

### Governance Features

- Prompt version management
- Human-in-the-loop approvals
- Processing status tracking
- Error and exception logging
- Artifact source traceability
- Reviewer comments and rejection reasons
- Export readiness control

---

## 🧭 11. Product Roadmap

### Current Prototype Capabilities

- Project creation
- Transcript upload
- AI-based requirement extraction
- Role-based artifact generation
- Dataverse-based traceability
- Approval workflows
- Prompt version tracking

### Planned Enhancements

- Admin console
- Microsoft Teams integration
- Advanced Jira synchronization
- Multi-language transcript support
- Power BI reporting dashboard
- Enhanced validation scoring
- Role-specific Copilot chat experience
- Advanced document export templates

---

## 👥 12. Team Member Roles

Nexa.ai was built by a focused two-member team: **Biswambhar Pal** and **Owendrila Saha**.

### Biswambhar Pal — Solution Architect and AI Power Platform Lead

- Defined the problem statement, solution scope, and product flow.
- Built the Power Pages portal, Dataverse structure, and Power Automate orchestration.
- Managed lookup relationships, approval flow, pipeline tracking, and demo preparation.

### Owendrila Saha — AI Experience and Product Strategy Lead

- Designed AI prompt flows for transcript analysis and artifact generation.
- Supported the portal user experience across dashboard, project, pipeline, approvals, and admin screens.
- Tested generated outputs, validation logic, and end-to-end demo readiness.

### Shared Contribution

- Product ideation and problem framing
- Microsoft Power Platform implementation
- AI workflow and prompt design
- Portal experience and demo flow
- Testing, documentation, and hackathon submission

---

## 📦 14. Deliverables

Nexa.ai can generate or manage the following pre-development deliverables:

- Business Requirement Document
- Requirement summary
- Epics, User stories
- Acceptance criteria
- Technical design notes
- Development checklist
- QA test scenarios
- Positive and negative test cases
- Risk and dependency register
- Approval history
- Exportable delivery package

---

## 🏁 15. Conclusion

Nexa.ai transforms scattered requirement conversations into structured, traceable, and governed delivery intelligence.

By combining Power Pages, Power Automate, Copilot Studio, AI Prompts, Dataverse, Microsoft Entra ID, and downstream delivery integrations, Nexa.ai demonstrates how enterprise teams can use Microsoft Power Platform to accelerate the pre-development lifecycle.

Nexa.ai helps teams move faster from discussion to delivery while keeping business context, approval control, and traceability intact.

---

## 📄 License and Ownership

This project is open-source and distributed under the ownership of team **Nexa**.

---

## 💙 Built By

Developed by **Team Nexa** for a Microsoft Build AI hackathon.

**Product:** Nexa.ai  
**Tagline:** Turning business conversations into structured delivery intelligence.
```````