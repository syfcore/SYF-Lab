# FRAME-R — Systemic Signal Framing

**Layer:** SYF-Lab (Derived Instrument)  
**Status:** Specification · v0.1-docs  
**Role:** Interpretation-free transport frame

---

## Role

FRAME-R defines **how R exists outside the law**:
- format
- structure
- encoding
- temporal anchoring

FRAME-R defines signal transport only.
Inoculums are defined separately as read-only observers consuming framed signals.

FRAME-R does not interpret R.  
It does not act on R.  
It does not modify R.

---

## 1. Definition

FRAME-R is the transport and structural framing layer for the invariant signal **R** produced by the SYF Core.

It is not a control system, but a deterministic envelope ensuring the signal remains portable, integral, and identical for any observer—human or machine.

---

## 2. Core Constraints

FRAME-R operates under absolute "Machine World" constraints:

**No Interpretation:** FRAME-R does not treat the value of R as "high", "low", "good", or "bad".

**No Thresholds:** FRAME-R contains no comparison logic, alerts, or conditional triggers.

**No Semantic Fields:** No metadata describing intent, context, or human meaning can be injected into the frame.

**No Feedback:** FRAME-R never transmits information back to the kernel.

---

## 3. Strict-Mode: Bit-Exact Integrity

To ensure the law is verifiable and reproducible across all platforms, FRAME-R strict-mode mandates:

**Payload Identity:** Independent instances observing the same Core state must produce bit-identical FRAME-R payloads.

**Deterministic Encoding:** Exclusive use of canonical serialization formats (e.g., Canonical JSON or Protobuf with no optional fields).

**Exogenous Timestamping:** If a timestamp is included, it is treated as transport metadata and must never influence the value of R.

---

## 4. Technical Specification Structure

A FRAME-R packet must consist solely of the elements required for portability:

**Core-ID:** SHA-256 hash of the frozen SYF Core implementation.

**R-Value:** The invariant scalar encoded with fixed precision (e.g., float64).

**Sequence/Time:** An ordering marker to ensure temporal continuity of observation.

**Integrity-H:** A checksum or hash ensuring the signal was not altered during transport.

---

## 5. Non-Intervention Guarantee

FRAME-R guarantees the integrity of the signal, not its correctness, safety, or meaning.

If the Core produces an R value at the FirePlank™ threshold, FRAME-R transmits this value with the same fidelity as any nominal value.

The authority to act upon the signal resides exclusively in higher layers (Inoculums or Userland), never within the framing layer.

**Machine World Only.**
