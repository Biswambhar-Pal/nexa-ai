# Nexa.ai — One-Page Demo Guide

**Team:** Nexa  
**Product:** Nexa.ai  
**Purpose:** Quick guide for judges/evaluators to access and review the Nexa.ai live demo.

---

## 1. Demo Access

**Portal URL**

```text
https://nexa-ai-enterprise-portal.powerappsportals.com/
```

**Recommended browser:** Microsoft Edge or Google Chrome  
**Recommended mode:** InPrivate / Incognito window

**Demo credentials**

```text
Username: microsoftbuildai@biswapal.onmicrosoft.com
Password: MNexa@2026
```

> These credentials are for hackathon evaluation only. Please do not upload sensitive or production data.

---

## 2. First-Time Sign-In

1. Open the portal URL.
2. Click **Sign in**.
3. Enter the demo username and password.
4. If Microsoft asks for additional security setup, install **Microsoft Authenticator** on a phone.
5. In Microsoft Authenticator, choose **Add account → Work or school account → Scan QR code**.
6. Scan the QR code shown on the browser.
7. Approve the verification request in the Authenticator app.
8. Return to the browser and continue to the Nexa.ai portal.

**If sign-in fails:** use InPrivate/Incognito mode, check the password carefully, or restart the QR setup flow.

---

## 3. What Nexa.ai Solves

Business requirement discussions often become scattered across transcripts, notes, emails, documents, and manual trackers. Nexa.ai converts those discussions into structured, traceable, and reviewable delivery artifacts.

Nexa.ai helps teams move from:

```text
Raw Transcript → AI-Generated Artifacts → Human Approval → Delivery-Ready Output
```

---

## 4. Demo Journey

### 1. Home Page
Start from the Nexa.ai workspace. This is the secure Power Pages portal where users access project creation, transcript upload, pipeline tracking, approvals, and admin controls.

### 2. Dashboard
Review project activity, transcript processing, generated artifacts, and approval status in one consolidated view.

### 3. New Project
Create or open a project. The project becomes the parent workspace connecting transcripts, AI outputs, approvals, and processing history.

### 4. Transcript Upload
Upload a requirement transcript (You can download "SampleTranscript.txt" from this github reposatory)or business discussion note. This becomes the source context for AI-assisted artifact generation.

### 5. Processing Pipeline
Track the transcript as it moves through ingestion, AI processing, draft generation, review, and approval stages. Power Automate orchestrates this workflow.

### 6. Generated Artifacts
Review AI-generated outputs such as requirement summaries, BRDs, user stories, acceptance criteria, technical notes, QA scenarios, risks, and open questions.

### 7. Approvals
Approve, reject, or request changes to generated artifacts. This demonstrates human-in-the-loop governance.

### 8. Admin Console
Review prompt versioning, pipeline configuration, processing status, and governance controls.

---

## 5. Microsoft Stack Used

- **Power Pages:** Portal and user experience
- **Dataverse:** Structured project, transcript, artifact, approval, and log data
- **Power Automate:** Workflow orchestration, approvals, and status tracking
- **Copilot Studio + AI Prompts:** Agentic AI and artifact generation
- **Microsoft Entra ID:** Secure sign-in
- **Jira / Azure DevOps ready:** Downstream delivery integration path

---

## 6. Expected Takeaway

After the demo, evaluators should see that Nexa.ai:

- Reduces manual pre-development documentation effort.
- Converts transcripts into role-based delivery artifacts.
- Maintains traceability from project to transcript to artifact.
- Uses human approval for governed AI output.
- Demonstrates a practical Microsoft Power Platform pattern for AI at work.

---

**Built by:** Team Nexa - Biswambhar Pal and Owendrila Saha  
**Tagline:** Turning business conversations into structured delivery intelligence.
