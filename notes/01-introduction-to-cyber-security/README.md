# Introduction to Cyber Security

> Module 01 — TryHackMe Pre Security

[![Status](https://img.shields.io/badge/Status-Completed-16A34A?style=flat-square)](#)
[![Topic](https://img.shields.io/badge/Topic-Cybersecurity-7C3AED?style=flat-square)](#)

---

## 🎯 Module Overview / Visão Geral

This module introduced the purpose of cybersecurity, common threats, and the importance of protecting systems, networks, and information.

Este módulo apresentou os fundamentos da Cybersecurity, ameaças comuns e a importância de proteger sistemas, redes e informações.

---

## 🧠 Key Concepts / Conceitos-Chave

### Cybersecurity

Cybersecurity is the practice of protecting devices, systems, networks, applications, and data from unauthorized access, damage, or disruption.

Cybersecurity é a prática de proteger dispositivos, sistemas, redes, aplicações e dados contra acesso não autorizado, danos ou interrupções.

### CIA Triad

The CIA Triad is a fundamental security model:

| Principle | Meaning |
|---|---|
| **Confidentiality** | Information should only be accessible to authorized people. |
| **Integrity** | Information must remain accurate and protected from unauthorized changes. |
| **Availability** | Systems and data should be available when authorized users need them. |

### Risk, Threat, and Vulnerability

| Term | Description |
|---|---|
| **Asset** | Anything valuable that should be protected, such as data, devices, or accounts. |
| **Threat** | Something that can cause harm, such as malware, phishing, or an attacker. |
| **Vulnerability** | A weakness that can be exploited. |
| **Risk** | The potential impact when a threat exploits a vulnerability. |

---

## 🛡️ Common Threats / Ameaças Comuns

- **Phishing:** attempts to deceive users into revealing information or performing unsafe actions.
- **Malware:** malicious software designed to damage, disrupt, or gain unauthorized access.
- **Social Engineering:** manipulation of people to obtain access or sensitive information.
- **Weak Passwords:** passwords that are easy to guess, reuse, or compromise.
- **Unpatched Systems:** systems with known vulnerabilities that have not been fixed.

---

## ⚖️ Ethical Learning / Aprendizado Ético

Cybersecurity knowledge must be used responsibly.

- Practice only in authorized labs and environments.
- Respect privacy, laws, and system owners.
- Never attempt unauthorized access.
- Document learning without sharing sensitive data, flags, or credentials.

---

## 📝 Personal Takeaways / Meus Aprendizados

- Cybersecurity is not only about attacking systems; it also involves prevention, detection, response, and recovery.
- People can be as important as technology in maintaining security.
- Understanding basic security concepts is essential before learning technical tools.

---

## 🔗 References / Referências

- [TryHackMe](https://tryhackme.com/)
- [Main repository README](../../README.md)

- ## 💻 Commands & Lab Examples / Comandos e Exemplos de Laboratório

> Commands are documented for educational purposes and must only be used in authorized labs or systems where permission was granted.  
> Os comandos são documentados para fins educacionais e devem ser usados somente em laboratórios autorizados ou sistemas com permissão.

### Gobuster — Directory Enumeration

**Purpose / Finalidade:**  
Gobuster can be used to identify publicly accessible directories or pages in an authorized web application test.

O Gobuster pode ser utilizado para identificar diretórios ou páginas publicamente acessíveis em um teste autorizado de aplicação web.

```bash
gobuster dir -u http://TARGET -w /path/to/wordlist.txt
```

| Option | Meaning / Significado |
|---|---|
| `dir` | Directory enumeration mode / Modo de enumeração de diretórios |
| `-u` | Target URL / URL do alvo autorizado |
| `-w` | Path to the wordlist / Caminho para a lista de palavras |

> No lab targets, flags, discovered paths, credentials, or answers are stored in this repository.
