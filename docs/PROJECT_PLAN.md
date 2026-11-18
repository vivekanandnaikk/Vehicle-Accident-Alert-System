# Project plan and reproducibility checklist

This plan distinguishes completed author work from future repository and verification work.

## 1. Add implementation artifacts

- [ ] Inspect and document the portfolio ZIP.
- [ ] Add the Arduino firmware used in the project.
- [ ] Add the Python host application.
- [ ] Add configuration and dependency manifests.
- [ ] Identify external libraries and preserve required notices.

## 2. Document hardware

- [ ] Record exact Arduino and sensor module models.
- [ ] Document verified pin assignments and output polarity.
- [ ] Verify supply voltage, logic levels, and GPS UART settings.
- [ ] Document common-ground and level-shifting requirements.
- [ ] Document MQ-3 warm-up and limitations.

## 3. Make software reproducible

- [ ] Define JSONL telemetry fields and validation rules.
- [ ] Document serial settings and host startup commands.
- [ ] Document event thresholds and cooldown behavior.
- [ ] Keep credentials outside the repository.
- [ ] Add unit tests and hardware-independent CI.

## 4. Reproduce results responsibly

- [ ] Record the bench-test setup and observations.
- [ ] Test missing and stale GPS fixes.
- [ ] Test email formatting and SMTP with dry-run and controlled recipients.
- [ ] Define metrics before making reliability or performance claims.
- [ ] Do not describe the prototype as safety-certified or emergency-ready.

## 5. Release responsibly

- [ ] Review archive and third-party component licenses.
- [ ] Select a license for original repository work after checking permissions.
- [ ] Add only authentic, permission-cleared photographs or test artifacts.
- [ ] Keep personal data, credentials, private location traces, and unlicensed assets out of Git.
