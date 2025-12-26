# Primordial Pipeline Overview

⚠️ **Important**: This file is a read-only reference. The canonical version is maintained separately and is frozen at v0.1.

This document defines the **primordial scientific pipeline** of the SYF project.

It describes the logical order in which the law, its signal,  
and its experimental instruments must exist.

This is not a software stack.  
It is a **laboratory structure**.

---

## Guiding Principle

A law must exist before it can be observed.  
An observation must exist before experimentation.  
An experiment must never modify the law.

---

## Pipeline

```
SYF Core
    ↓
FRAME-R
    ↓
SEW
    ↓
CoreXalt
```

---

## Layer Roles (Summary)

### SYF Core
The immutable law-bearing core.  
Produces a deterministic invariant (R).  
Has no intent, no governance, no feedback.

### FRAME-R
Defines how the signal exists outside the law.  
Formatting, normalization, encoding only.

### SEW
Passive observation.  
Visualization and inspection without control.

### CoreXalt
Interface and adaptation layer.  
Connects SYF-based systems to external environments without mutation.

---

## Boundary Rule

If a component can be removed without invalidating the law,  
it does not belong to SYF Core.

---

This pipeline defines the **only valid order** of construction.
