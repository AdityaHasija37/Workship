# Use cases

[← Back to README](../README.md)

## Middleweight

### UC-1: Quick Apply to verified jobs (job seeker)

| | |
|---|---|
| **Primary actor** | Alex (job seeker) |
| **Stakeholders** | Job seeker, hiring companies |
| **Precondition** | Alex has a verified profile and is logged in |
| **Trigger** | Alex wants to apply to several verified jobs quickly |

**Basic flow**

1. Alex logs in and sees jobs matched to his profile.
2. He selects **Quick Apply** on the jobs he wants.
3. Applications are submitted without re-entering any details.
4. He gets a confirmation and real-time status updates.

**Alternate flow:** if a submission fails, Alex sees an error and can retry.

### UC-2: Post a job (recruiter)

| | |
|---|---|
| **Primary actor** | Recruiter |
| **Stakeholders** | Recruiter, job seeker, WorkShip |
| **Precondition** | Recruiter has a verified WorkShip account and is logged in |
| **Trigger** | Recruiter wants to post a new opening |

**Basic flow**

1. The recruiter clicks **Post a Job** on the home screen.
2. WorkShip shows the job-details form.
3. The recruiter fills in the required details.
4. WorkShip posts the job.
5. WorkShip confirms with a notification.

**Alternate flows:** if posting fails, WorkShip shows an error and prompts a retry. If required fields are incomplete, it flags them and asks the recruiter to complete them before posting.

## Heavyweight

### UC-3: Seamless profile verification (job seeker)

| | |
|---|---|
| **Primary actor** | Alex (job seeker) |
| **Stakeholders** | Job seeker, hiring companies |
| **Precondition** | Alex has a WorkShip account and is logged in |
| **Trigger** | Alex wants more relevant recommendations |

**Basic flow**

1. Alex uploads his education certificates and work experience.
2. The system verifies the credentials and marks Alex as a **verified candidate**.
3. Alex gets exclusive recommendations that prioritize verified applicants.

**Alternate flows**

- If verification fails, Alex sees an error and can retry.
- Alex can skip verification, but his applications are put **on hold** until he verifies.

### UC-4: Application follow-up with Wingman AI (job seeker)

| | |
|---|---|
| **Primary actor** | Alex (job seeker) |
| **Stakeholders** | Job seeker, hiring companies |
| **Precondition** | Alex is logged in and has received an offer |
| **Trigger** | Alex wants to follow up on his application |

**Basic flow**

1. Alex opens the **Career Compass** dashboard.
2. He expands the **Offer Received** tile.
3. He chooses to follow up.
4. WorkShip opens **Wingman AI**.
5. Wingman AI drafts a professional email to the hiring manager.
6. Alex sends it directly from Wingman AI.

**Alternate flows:** if sending fails, Alex sees an error and can retry. Alex can edit the draft manually or decide not to send.
