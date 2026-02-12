# Week 1–2 Work Notes (CRUD & Workflow Processes)

## 02/12/2026 (Thursday)

### TL;DR

### Speaking with Andrew

**CodeApps and Dataverse**
**Focus on functionality > minor details**
 * Friday Meeting




---

* **CRUD PowerApps Continuation**
*➡️ **Implemented Search Functionality**
*➡️ **Implemented Edit Functionality**


---


## 02/10/2026 (Tuesday)

### TL;DR

* **CRUD PowerApps Kickoff**
* **Link to PowerApps Progress:** [https://csulb-my.sharepoint.com/shared?listurl=https%3A%2F%2Fcsulb%2Dmy%2Esharepoint%2Ecom%2Fpersonal%2Fangel%5Fmendez%2Dsa%5Fcsulb%5Fedu%2FDocuments&id=%2Fpersonal%2Fangel%5Fmendez%2Dsa%5Fcsulb%5Fedu%2FDocuments%2FPowerApps%20Progress%202%2D10%2D2026%2Epng&parent=%2Fpersonal%2Fangel%5Fmendez%2Dsa%5Fcsulb%5Fedu%2FDocuments&shareLink=1&ga=1](https://csulb-my.sharepoint.com/shared?listurl=https%3A%2F%2Fcsulb%2Dmy%2Esharepoint%2Ecom%2Fpersonal%2Fangel%5Fmendez%2Dsa%5Fcsulb%5Fedu%2FDocuments&id=%2Fpersonal%2Fangel%5Fmendez%2Dsa%5Fcsulb%5Fedu%2FDocuments%2FPowerApps%20Progress%202%2D10%2D2026%2Epng&parent=%2Fpersonal%2Fangel%5Fmendez%2Dsa%5Fcsulb%5Fedu%2FDocuments&shareLink=1&ga=1)
* **Research Workflows for Dev Team**
* **Link to Flowchart:** [https://csulb-my.sharepoint.com/:i:/g/personal/angel_mendez-sa_csulb_edu/IQD4P9OlKRKhTJq3bb3Kr7PJAer7TN-nJy7zkCKNABtSLKk?e=Xcow7y](https://csulb-my.sharepoint.com/:i:/g/personal/angel_mendez-sa_csulb_edu/IQD4P9OlKRKhTJq3bb3Kr7PJAer7TN-nJy7zkCKNABtSLKk?e=Xcow7y)

---

## Workflow Flowcharts

* **Intent (what & why)** → Jira / GitHub Issues
* **Execution (how & when)** → GitHub (code, PRs)
* **Artifacts (thinking)** → Google Drive

---

## BEGIN DEV WORKFLOWS

### Tools

* *Jira ticket* = a tracked work item (bug, task, feature)
* *PR (Pull Request)* = a request to merge code you wrote into the main codebase
* *Done criteria* = how we know the work is finished (2–5 bullets)
* *Smoke check* = quick check to see if the app still works after deploy
* *Procedure* = step-by-step instructions for repeating a task
* *Repo* = the GitHub project where the code lives

---

### Roles

* *Requester* — Anyone asking for work (manager, teammate, you)
* *Lead* — Person who prioritizes work (manager or senior dev)
* *Developer (Dev)* — Person doing the work
* *Reviewer* — Another dev who reviews code
* *(Small team: one person may fill multiple roles.)*

---

## THE WORKFLOW (STEP BY STEP)

### 1) Someone asks for work

**Who:** Manager, teammate, customer, or you

* If the work will take more than ~30 minutes, a Jira ticket is created
* Ticket says:

  * what the problem is
  * what “done” looks like (example: “login works, no errors in logs”)

➡️ **Strict:** work starts only after a ticket exists (same day is okay)

---

### 2) Ticket is made ready

**Who:** Manager / team lead (or dev if small team)

* Sets priority (high / medium / low)
* Assigns ticket to a dev (or puts it in “Ready”)

➡️ **Strict:** every ticket has an owner and priority

---

### 3) Dev starts work

**Who:** Developer

* Moves Jira ticket to In Progress
* Creates a branch in GitHub named after the ticket (example: DEV-42)
* Starts a daily log (private notes):

  * what you tried
  * what worked / failed

➡️ **Strict:** ticket status matches reality
➡️ **Not strict:** how neat the notes are

---

### 4) Dev writes code

**Who:** Developer

* Makes code changes
* Runs tests or manually checks the feature
* If something feels confusing or painful, notes it

➡️ **Strict:** code changes relate to the ticket

---

### 5) Dev opens a PR

**Who:** Developer

* Opens a Pull Request (PR) in GitHub
* PR includes:

  * link to Jira ticket
  * short explanation of what changed
  * how it was tested (“clicked login, saw success”)

➡️ **Strict:** every PR links to a Jira ticket

---

### 6) Code is reviewed

**Who:** Another developer

* Reviews PR
* Checks:

  * does it work?
  * does it make sense?
* Approves or asks for changes

➡️ **Strict:** no merging without review

---

### 7) Changes go live

**Who:** Developer or DevOps

* PR is merged
* Code is deployed
* Smoke check:

  * open the app
  * basic feature works
  * no obvious errors

➡️ **Strict:** always do a quick smoke check

---

### 8) Knowledge is saved (only if needed)

**Who:** Developer

* If this task will happen again:

  * write a procedure
  * store it in the repo

```
repo/docs/procedures/<topic>.md
```

Examples:

* “How to deploy”
* “How to fix login errors”

➡️ **Strict:** repeated pain becomes a procedure
➡️ **Not strict:** perfect wording

---

### 9) Ticket is closed

**Who:** Developer

* Updates Jira ticket with:

  * what was done
  * link to PR
  * link to procedure (if written)
* Moves ticket to Done

➡️ **Strict:** ticket closes with links and a summary

---

## WHAT WE ARE STRICT ABOUT

* Jira ticket exists for real work
* Ticket has an owner and “done” criteria
* PRs link to Jira
* Code is reviewed
* Smoke check after deploy
* Procedures live in the repo under docs/procedures/

---

## WHAT WE ARE NOT STRICT ABOUT

* Fancy writing
* Perfect formatting
* Extra tools
* Writing docs during emergencies

---

## END DEV WORKFLOWS

---

## For School Workflows

* **GitHub Issues** → tasks, experiments, TODOs
* **GitHub Repo** → code, scripts, LaTeX, notebooks
* **Google Drive** → papers, sources, rough notes, slides

### Simple school-project workflow (low stress)

* Create GitHub repo

**Use GitHub Issues for:**

* experiments
* writing tasks
* milestones

**Use Drive folder for:**

* research notes

* paper drafts

* slides

* Link everything

* Close issues when artifacts or code exist

---

## Notes Outline

### 2026-02-10

* Jira
* What I did
* Notes
* Tomorrow
---

## 02/05/2026 (Tuesday Meeting)

* next week starting on CUP

* How we're going to model bigger changes to

* Make sure Angel has access to all webpages

* Angel needs to do Power App, Luis provide instructions on how to load up? the time off app on the machine?

* Luis' environment is still active. Angel needs to be hooked up onto GitHub, etc.

* Proof of concept

* CUP going to be the heavy stuff

---




