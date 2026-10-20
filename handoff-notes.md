# Developer handoff notes

## What I delivered
I delivered a static customer support portal page (`index.html`) styled with a clean layout via a companion stylesheet (`styles.css`). This includes primary contact details, supported hours, and an explicit reminder for customers to provide their order numbers when reaching out. Additionally, I implemented an FAQ section addressing how customers can check their order status, satisfying the request from the product manager.

## How I verified the page
I created a tracking document (`support-checklist.md`) and verified the following elements locally:
- Confirmed the page title and contact email are visible and accessible.
- Verified that support hours clearly specify the Central Time zone.
- Ensured the reminder text asks for order numbers during contact.
- Verified the FAQ section accurately maps out how to check order statuses.
- Resized the browser window to confirm the CSS remains responsive and readable in narrow viewports.

## Remote change I received
I received an update documenting the billing escalation process, which was appended to the bottom of the remote `README.md` file. To pull this change safely from the shared repository into my local environment without creating an accidental merge commit, I executed:
`git pull --ff-only origin main`

## Git workflow explanation
Running `git commit` only updates your local repository history inside the hidden `.git` folder on your machine. Git operates entirely offline for day-to-day work, meaning local commits are isolated snapshots. To share those snapshots and update the remote repository on GitHub, a separate network operation—`git push`—is strictly required.
