# Learn-SecByte-CTF-Labs-Collection-Process-Injection-Persistence-Memory-Evasion-Labs
A curated collection of hands-on cybersecurity CTF labs covering Process Hollowing, Reflective DLL Injection, APC &amp; Thread Injection, Parent PID Spoofing, AtomBombing, WMI Persistence, and Credential Dumping from Learn SecByte.
# Learn SecByte CTF & Cybersecurity Labs Collection

Welcome to the **Learn SecByte CTF & Cybersecurity Labs Collection**. This repository is a dedicated, searchable index of hands-on Windows memory injection, evasion tradecraft, persistent backdoor, and credential dumping labs designed for cybersecurity students, CTF players, malware analysts, penetration testers, and threat hunters.

---

## Table of Contents
- [Introduction](#introduction)
- [Lab Collection & Index](#lab-collection--index)
- [Categories](#categories)
- [Learning Path](#learning-path)
- [How to Use the Labs](#how-to-use-the-labs)
- [Disclaimer](#disclaimer)

---

## Introduction

Understanding low-level Windows internals, memory manipulation, and silent persistence mechanisms is essential for both red team tradecraft and blue team threat detection. Hosted on [Learn SecByte](https://learn.secbyte.org/), this collection of CTF challenge labs focuses on practical execution evasion, memory injection, and management plane persistence.

From fundamental process injection mechanics, Process Hollowing, and Reflective DLL Injection to advanced techniques like APC Injection, AtomBombing, Parent PID Spoofing, DLL Search Order Hijacking, COM Hijacking, and WMI Event Subscription persistence, these exercises build job-ready security engineering capabilities.

---

## Lab Collection & Index

Below is the complete, searchable index of all process injection, persistence, and credential tradecraft challenges in this collection:

| # | Lab / Challenge Name | Category | Focus / Key Topics | Lab Link |
|---|----------------------|----------|---------------------|----------|
| 1 | **Credential Dumping Techniques Lab** | Credential Access | LSASS memory inspection, SAM/SYSTEM registry hives, token theft, LSA secrets | [Access Lab](https://learn.secbyte.org/ctf/credential-dumping-techniques-lab) |
| 2 | **Parent PID Spoofing: Process Lineage Deception Lab** | Execution Evasion | `CreateProcess` API, `STARTUPINFOEX` structures, process tree obfuscation | [Access Lab](https://learn.secbyte.org/ctf/parent-pid-spoofing-process-lineage-deception-lab) |
| 3 | **AtomBombing Memory Injection Tradecraft** | Process Injection | Atom tables, `GlobalAddAtom`, `QueueUserAPC`, payload execution without write access | [Access Lab](https://learn.secbyte.org/ctf/atombombing-memory-injection-tradecraft) |
| 4 | **APC Injection Lab: Queueing Code into Remote Threads** | Process Injection | Asynchronous Procedure Calls, `QueueUserAPC`, alertable thread exploitation | [Access Lab](https://learn.secbyte.org/ctf/apc-injection-lab-queueing-code-into-remote-threads) |
| 5 | **Thread Injection: Remote Threading in Windows Memory** | Process Injection | `OpenProcess`, `VirtualAllocEx`, `WriteProcessMemory`, `CreateRemoteThread` | [Access Lab](https://learn.secbyte.org/ctf/thread-injection-remote-threading-in-windows-memory) |
| 6 | **Process Hollowing: From Theory to Detection** | Process Injection | Unmapping image sections, `NtUnmapViewOfSection`, context manipulation (`SetThreadContext`) | [Access Lab](https://learn.secbyte.org/ctf/process-hollowing-from-theory-to-detection) |
| 7 | **Reflective DLL Injection in-Memory Loader Lab** | Process Injection | In-memory PE loading, custom API resolution, reflective loader execution | [Access Lab](https://learn.secbyte.org/ctf/reflective-dll-injection-in-memory-loader-lab) |
| 8 | **DLL Injection: Threadless Entry Points** | Process Injection | Indirect code execution, memory hook execution, threadless injection tradecraft | [Access Lab](https://learn.secbyte.org/ctf/dll-injection-threadless-entry-points) |
| 9 | **Process Injection Fundamentals** | Process Injection | Windows memory management, virtual memory allocations, injection primitives | [Access Lab](https://learn.secbyte.org/ctf/process-injection-fundamentals) |
| 10 | **DLL Search Order Hijacking: From Theory to Detection** | Hijacking & Escalation | Windows DLL search path, phantom DLLs, application directory hijacking | [Access Lab](https://learn.secbyte.org/ctf/dll-search-order-hijacking-from-theory-to-detection) |
| 11 | **COM Hijacking Startup Persistence and Trust Abuse** | Persistence | Component Object Model (COM) registry keys, `InprocServer32` hijacking, CLSID abuse | [Access Lab](https://learn.secbyte.org/ctf/com-hijacking-startup-persistence-and-trust-abuse) |
| 12 | **WMI Persistence: Living Off the Management Plane** | Persistence | WMI Event Filters, Event Consumers (`CommandLineEventConsumer`), Binding execution | [Access Lab](https://learn.secbyte.org/ctf/wmi-persistence-living-off-the-management-plane) |

---

## Categories

### 1. Process Injection & Memory Manipulation
Master techniques used to inject code into remote process memory spaces to bypass process-based monitoring controls.
- [Process Injection Fundamentals](https://learn.secbyte.org/ctf/process-injection-fundamentals)
- [Thread Injection: Remote Threading in Windows Memory](https://learn.secbyte.org/ctf/thread-injection-remote-threading-in-windows-memory)
- [Process Hollowing: From Theory to Detection](https://learn.secbyte.org/ctf/process-hollowing-from-theory-to-detection)
- [Reflective DLL Injection in-Memory Loader Lab](https://learn.secbyte.org/ctf/reflective-dll-injection-in-memory-loader-lab)
- [DLL Injection: Threadless Entry Points](https://learn.secbyte.org/ctf/dll-injection-threadless-entry-points)
- [APC Injection Lab: Queueing Code into Remote Threads](https://learn.secbyte.org/ctf/apc-injection-lab-queueing-code-into-remote-threads)
- [AtomBombing Memory Injection Tradecraft](https://learn.secbyte.org/ctf/atombombing-memory-injection-tradecraft)

### 2. Execution Evasion & Process Spoofing
Analyze tradecraft designed to hide process relationships, obfuscate execution lineages, and deceive security monitoring tools.
- [Parent PID Spoofing: Process Lineage Deception Lab](https://learn.secbyte.org/ctf/parent-pid-spoofing-process-lineage-deception-lab)
- [DLL Search Order Hijacking: From Theory to Detection](https://learn.secbyte.org/ctf/dll-search-order-hijacking-from-theory-to-detection)

### 3. Management Plane Persistence
Deconstruct fileless and registry-based persistence vectors operating natively through Windows core subsystems.
- [COM Hijacking Startup Persistence and Trust Abuse](https://learn.secbyte.org/ctf/com-hijacking-startup-persistence-and-trust-abuse)
- [WMI Persistence: Living Off the Management Plane](https://learn.secbyte.org/ctf/wmi-persistence-living-off-the-management-plane)

### 4. Credential Dumping & Theft
Investigate local security authority memory structures and registry stores to extract cached credentials and hashes.
- [Credential Dumping Techniques Lab](https://learn.secbyte.org/ctf/credential-dumping-techniques-lab)

---

## Learning Path

Follow this structured learning pathway to master Windows memory injection and persistence analysis:

1. **Phase 1: Memory Injection Fundamentals** — Understand basic process memory allocation and thread creation:
   - [Process Injection Fundamentals](https://learn.secbyte.org/ctf/process-injection-fundamentals)
   - [Thread Injection: Remote Threading in Windows Memory](https://learn.secbyte.org/ctf/thread-injection-remote-threading-in-windows-memory)
   - [Reflective DLL Injection in-Memory Loader Lab](https://learn.secbyte.org/ctf/reflective-dll-injection-in-memory-loader-lab)

2. **Phase 2: Advanced Memory Tradecraft & Evasion** — Master APC queuing, AtomBombing, and lineage spoofing:
   - [APC Injection Lab: Queueing Code into Remote Threads](https://learn.secbyte.org/ctf/apc-injection-lab-queueing-code-into-remote-threads)
   - [Process Hollowing: From Theory to Detection](https://learn.secbyte.org/ctf/process-hollowing-from-theory-to-detection)
   - [AtomBombing Memory Injection Tradecraft](https://learn.secbyte.org/ctf/atombombing-memory-injection-tradecraft)
   - [DLL Injection: Threadless Entry Points](https://learn.secbyte.org/ctf/dll-injection-threadless-entry-points)
   - [Parent PID Spoofing: Process Lineage Deception Lab](https://learn.secbyte.org/ctf/parent-pid-spoofing-process-lineage-deception-lab)

3. **Phase 3: Persistence Mechanics & Search Order Hijacking** — Audit registry hooks and management plane triggers:
   - [DLL Search Order Hijacking: From Theory to Detection](https://learn.secbyte.org/ctf/dll-search-order-hijacking-from-theory-to-detection)
   - [COM Hijacking Startup Persistence and Trust Abuse](https://learn.secbyte.org/ctf/com-hijacking-startup-persistence-and-trust-abuse)
   - [WMI Persistence: Living Off the Management Plane](https://learn.secbyte.org/ctf/wmi-persistence-living-off-the-management-plane)

4. **Phase 4: Credential Access** — Extract secrets from memory and registry hives:
   - [Credential Dumping Techniques Lab](https://learn.secbyte.org/ctf/credential-dumping-techniques-lab)

---

## How to Use the Labs

1. Select a challenge link from the index or category sections above.
2. Read the scenario directives and target requirements on [Learn SecByte](https://learn.secbyte.org/).
3. Use debugging and memory inspection utilities (e.g., Process Hacker/System Informer, x64dbg, WinDbg, Volatility, Autoruns) inside a dedicated, isolated VM.
4. Trace memory allocations, inspect injected threads, identify persistence mechanisms, extract credentials, and retrieve challenge flags.

---

## Disclaimer

This repository and its linked challenge resources are strictly created for educational, threat research, and authorized security training purposes. Performing process injection, credential dumping, or persistence testing on production machines or unapproved networks is strictly prohibited.
