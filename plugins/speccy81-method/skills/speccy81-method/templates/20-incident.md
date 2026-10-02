# Security incident (exposed key, datum or channel)

Opened as soon as it is suspected, without waiting to be sure. No secrets or personal data in this document:
of keys, only their internal name and their hash; of people, only their role.

## Steps
1. **Contain** what is urgent: deactivate the key, cut the access or the channel. If it is a key, with the rule of the
   exposed key: the replacement first; if it is public and urgent, it is deactivated right away, saying beforehand what stops
   working and for whom. It is never reactivated.
2. **Diagnose by reading only:** what was exposed, since when, where and who could have seen it. It is measured (rule 2):
   figure, query or command, date.
3. **Decide and notify:** the user decides. If there is a client's personal data, the client is the **controller**
   and you are the **processor**: you notify them in writing **without undue delay** (art. 33(2) GDPR) with what happened, since
   when, what has been done and what cannot be ruled out. The controller assesses whether to notify the data protection
   authority within **72 hours** (art. 33). If the data is yours, you are the controller.
4. **Record** every incident, even if it is not notified (art. 33(5)): facts, effects and measures.
5. **Lesson:** the new rule or the improvement to the method that prevents it from happening again.

## Record sheet
```markdown
# Incident <n> · opened <date time> · status: open | contained | closed
What: <what was exposed, by internal name and hash; never the value>
Where and since when: <channel, file or service · earliest possible date>
Who could have seen it: <public | clients | staff | nobody outside the team> — Proof: <log or command>
Containment: <what was deactivated or cut, when> — Proof: <…>
What stops working and for whom: <…>
Personal data affected: yes | no | cannot be ruled out — why
Data controller: <client | us> · notice sent?: <date, by whom> | draft in <path>
Notification to the authority (decided by the controller): yes | no — reason
Measures: <…>
Lesson: <new rule or improvement>
```

## Example
An API token appears in a configuration file that was published in a repository. Contain: a new
token is generated, put in every place that uses it and the old one is revoked. Diagnose: the
provider's log says whether anyone used the token and since when. Record: sheet filled in even if there is no personal data.
Lesson: the configuration file goes in `.gitignore` and the repository is reviewed before publishing.
