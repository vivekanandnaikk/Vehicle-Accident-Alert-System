# Project plan and reproducibility checklist

This repository is currently a documentation foundation. The checklist below is a roadmap, not a statement that implementation or validation work is complete.

## 1. Establish source and provenance

- [ ] Inspect the supplied portfolio ZIP and document its files, origin, and redistribution terms.
- [ ] Locate original firmware, Python application, circuit diagrams, and project records if they exist.
- [ ] Clearly identify recovered original work versus newly reconstructed reference implementation.
- [ ] Record contributors, author naming preference, external libraries, and license requirements.

## 2. Verify hardware and electrical design

- [ ] Record exact Arduino, vibration-module, MQ-3 module, and GPS breakout model numbers.
- [ ] Verify pin assignments, vibration output polarity, UART baud rate, logic levels, regulator details, and supply/current requirements from component documentation.
- [ ] Document common-ground and level-shifting requirements in a reviewed wiring diagram.
- [ ] Document MQ-3 warm-up and limitations; do not label raw ADC counts as alcohol concentration or impairment.
- [ ] Keep initial testing on a current-limited, controlled bench setup; do not connect to vehicle control systems.

## 3. Make the software reproducible

- [ ] Add firmware source and document Arduino board/core and TinyGPSPlus versions.
- [ ] Add Python source and a tested dependency manifest if the host program is available.
- [ ] Define JSONL fields, types, ranges, units, invalid-data behavior, and GPS freshness semantics.
- [ ] Document serial port selection and robust handling of disconnects, malformed records, and shutdown.
- [ ] Define event and cooldown semantics; treat vibration as a trigger, not crash confirmation.
- [ ] Keep credentials out of Git and make dry-run the safe initial notification mode.
- [ ] Add unit tests and CI that do not require hardware, secrets, or live email.

## 4. Validate and report responsibly

- [ ] Record actual bench setup, sensor warm-up, observations, and limitations; do not fabricate results.
- [ ] Test GPS availability and stale-fix handling in controlled conditions.
- [ ] Test notification formatting and SMTP only with a controlled account/recipient after dry-run checks.
- [ ] Define objective metrics and repeatable procedures before making reliability or performance claims.
- [ ] Do not claim emergency-response suitability or safety certification.

## 5. Release responsibly

- [ ] Review license and terms for the portfolio archive, third-party libraries, diagrams, and any recovered code.
- [ ] Select a license for original repository work only after provenance and permissions are clear.
- [ ] Add authentic, permission-cleared photographs or test artifacts only when they document actual work.
- [ ] Keep personal data, location traces, credentials, and unlicensed assets out of the repository.
