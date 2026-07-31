# Computer Fundamentals

> Module 02 — TryHackMe Pre Security

[![Status](https://img.shields.io/badge/Status-Completed-16A34A?style=flat-square)](#)
[![Topic](https://img.shields.io/badge/Topic-Computer%20Fundamentals-2563EB?style=flat-square)](#)

---

## 🎯 Module Overview / Visão Geral

This module covers the fundamental components of a computer and explains how hardware, software, and the boot process work together.

Este módulo aborda os componentes fundamentais de um computador e explica como hardware, software e o processo de inicialização funcionam em conjunto.

---

## 🧠 Key Concepts / Conceitos-Chave

### Hardware and Software

| Concept | Description |
|---|---|
| **Hardware** | Physical components of a computer, such as CPU, RAM, storage, keyboard, and monitor. |
| **Software** | Programs and instructions executed by a computer. |
| **Operating System** | Software that manages hardware resources and provides an environment for applications and users. |

### Core Components / Componentes Principais

| Component | Purpose / Finalidade |
|---|---|
| **CPU** | Processes instructions and performs calculations. |
| **RAM** | Temporary memory used by active programs and processes. |
| **Storage** | Stores files and programs permanently, such as HDDs and SSDs. |
| **Motherboard** | Connects the internal components of the computer. |
| **Input Devices** | Send information to the computer, such as a keyboard and mouse. |
| **Output Devices** | Present information from the computer, such as a monitor and speakers. |

---

## 💻 Commands & Technical Examples / Comandos e Exemplos Técnicos

### Commands Used / Comandos Utilizados

This module is focused on computer hardware and the boot process. No terminal commands were introduced in my notes for this module.

Este módulo é focado em hardware e no processo de inicialização. Não foram incluídos comandos de terminal nesta anotação.

### Boot Process / Processo de Inicialização

```text
Power Button Pressed
        ↓
BIOS or UEFI Starts
        ↓
Hardware Check (POST)
        ↓
Boot Device Is Selected
        ↓
Bootloader Starts
        ↓
Operating System Loads
        ↓
User Login / Desktop
```

| Stage | Description |
|---|---|
| **BIOS / UEFI** | Firmware that starts the system and checks essential hardware. |
| **POST** | Initial hardware verification process. |
| **Boot Device** | The selected disk or device containing the operating system. |
| **Bootloader** | Program responsible for loading the operating system. |
| **Operating System** | Takes control of hardware resources and allows the system to be used. |

---

## 🛡️ Cybersecurity Relevance / Relevância para Cybersecurity

Understanding computer fundamentals is important for cybersecurity because it helps explain:

- where information is stored;
- how memory is used by applications;
- how an operating system manages users and programs;
- how hardware and software can be affected by vulnerabilities;
- why the boot process and system configuration matter for security.

---

## 📝 Personal Takeaways / Meus Aprendizados

- A computer works through the interaction between hardware, software, and the operating system.
- CPU, RAM, and storage have different functions and directly affect how a system operates.
- The boot process is an important concept because a compromised system can be attacked before the operating system fully loads.

---

## 🔗 References / Referências

- [TryHackMe](https://tryhackme.com/)
- [Main repository README](../../README.md)
