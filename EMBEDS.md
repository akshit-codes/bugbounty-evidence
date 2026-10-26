# Paste-ready image embeds

Repo assumed: **akshit-codes/bugbounty-evidence**, branch **main**. If you name it differently, find-replace the URL base.

Paste each block into that issue's body (CDS: inside Reproduction or at the end; DVFS: under Visual Evidence).

## CDS-01 (force on cancelled job)

**Application rejected; both Reinstate and Force transition enabled**
![01-1-record-before-cancel](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/01-1-record-before-cancel.png)

**Cancelling the Quantitative Researcher job**
![01-2-cancel-dialog](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/01-2-cancel-dialog.png)

**After cancel: Reinstate disabled, Force transition still enabled**
![01-3-reinstate-disabled-force-enabled](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/01-3-reinstate-disabled-force-enabled.png)

**Force preview succeeds, recommends reinstate_application**
![01-4-force-preview](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/01-4-force-preview.png)

**IN PROGRESS at Quant Test while the round ledger reads ELIMINATED / ABSENT**
![01-5-in-progress-on-cancelled-job](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/01-5-in-progress-on-cancelled-job.png)

**Consistency checker: nothing has drifted, 0 violations**
![01-6-checker-zero-violations](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/01-6-checker-zero-violations.png)

**Student sees it as in progress with Edit and Withdraw**
![01-7-student-my-applications](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/01-7-student-my-applications.png)

**Clicking through to the job: Job not found**
![01-8-student-job-not-found](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/01-8-student-job-not-found.png)

---

## CDS-02 (SCREEN_DEPS)

**Offers screen: Bikram OFFERED**
![02-1-offers-bikram-offered](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/02-1-offers-bikram-offered.png)

**Forced to declined on the student record**
![02-2-record-declined](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/02-2-record-declined.png)

**Back on Offers via in-app nav (no reload): still OFFERED with Terminate**
![02-3-offers-STALE-still-offered](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/02-3-offers-STALE-still-offered.png)

**After a hard reload: correctly DECLINED**
![02-4-offers-reload-declined](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/02-4-offers-reload-declined.png)

---

## CDS-03 (phantom offer)

**Force to offered; preview says no offer row is created**
![03-1-force-no-offer-row-text](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/03-1-force-no-offer-row-text.png)

**Record shows OFFERED with an empty offers block**
![03-2-record-offered-no-offers](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/03-2-record-offered-no-offers.png)

**Offers screen: OFFERED chip, no current offered or accepted offer, no actions**
![03-3-offers-asha-offered-no-actions](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/03-3-offers-asha-offered-no-actions.png)

**Consistency checker: 0 violations**
![03-4-checker-zero-violations](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/03-4-checker-zero-violations.png)

**Dashboard: 0 offers awaiting above OFFERED - Respond to your offer**
![03-5-dashboard-offered-vs-no-offer-awaiting](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/cds/03-5-dashboard-offered-vs-no-offer-awaiting.png)

---

## DVFS-01 (cputemp cache)

**Repro test fails: sensors forked 3x in 3 calls; upstream tests leak host sensors**
![evidence-01-test](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/dvfs/evidence-01-test.png)

**6 live /metrics scrapes fork sensors 6 times, ~103ms each**
![evidence-01-metrics](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/dvfs/evidence-01-metrics.png)

---

## DVFS-02 (disk reserve)

**12-byte upload rejected on a 15.5 GiB disk; no startup warning**
![evidence-02-upload-rejected](https://raw.githubusercontent.com/akshit-codes/bugbounty-evidence/main/dvfs/evidence-02-upload-rejected.png)

---
