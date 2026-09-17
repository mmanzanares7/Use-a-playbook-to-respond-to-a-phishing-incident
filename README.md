# Incident Handler's Journal

## Project Description

This is a running journal of security incident scenarios I've worked through, documenting each one the way an incident handler would in practice: a description, tools used, the 5 W's (who, what, when, where, why), and any open questions the incident raises. Each entry is dated and numbered chronologically in [`journal.md`](journal.md), so the file grows as I work through new scenarios rather than being a one-off writeup.

## Why keep a journal like this

Documentation is one of the most consistently undervalued skills in incident response. A clear, factual record of what happened, in what order, and why matters just as much during an active incident as it does afterward, when the same notes support root-cause analysis, regulatory reporting, or a lessons-learned review. This journal is where I practice that discipline: treating a scenario as a real incident to be documented, not just a question to answer.

## Entries

See [`journal.md`](journal.md) for the full log. Current entries:

- **Entry #1** (September 15, 2026) - Ransomware incident at a healthcare clinic, initiated via phishing
- **Entry #2** (September 17, 2026) - VirusTotal investigation of a Flagpro/BlackTech malware hash, mapped to the Pyramid of Pain (see the companion [pyramid-of-pain-malware-analysis](https://github.com/mmanzanares7/pyramid-of-pain-malware-analysis) repo)
- **Entry #3** (September 17, 2026) - Phishing alert triage using a formal playbook, escalated based on the Entry #2 hash findings (see the companion [phishing-incident-response](https://github.com/mmanzanares7/phishing-incident-response) repo)
