# Operating Systems Basics

> Module 03 — TryHackMe Pre Security

[![Status](https://img.shields.io/badge/Status-Completed-16A34A?style=flat-square)](#)
[![Topic](https://img.shields.io/badge/Topic-Operating%20Systems-7C3AED?style=flat-square)](#)

---

## 🎯 Module Overview / Visão Geral

This module introduced the role of operating systems and how they manage hardware, applications, files, users, and system resources.

Este módulo apresentou a função dos sistemas operacionais e como eles gerenciam hardware, aplicações, arquivos, usuários e recursos do sistema.

---

## 🧠 Key Concepts / Conceitos-Chave

### What Is an Operating System?

An operating system (OS) is the software layer between the user, applications, and computer hardware.

Um sistema operacional (SO) é a camada de software entre o usuário, as aplicações e o hardware do computador.

Examples / Exemplos:

- Windows
- Linux
- macOS
- Android
- iOS

### Main Responsibilities / Principais Responsabilidades

| Responsibility | Description |
|---|---|
| **Process Management** | Manages programs that are running. |
| **Memory Management** | Controls how RAM is allocated to applications. |
| **File Management** | Organizes files, directories, and storage devices. |
| **User Management** | Controls users, authentication, and permissions. |
| **Device Management** | Allows the operating system to communicate with hardware. |
| **Security** | Applies permissions and helps protect system resources. |

---

## ⚙️ Kernel Space and User Space

```text
User
  ↓
Applications
  ↓
User Space
  ↓
System Calls
  ↓
Kernel Space
  ↓
Hardware
```

| Area | Description |
|---|---|
| **User Space** | Where normal applications run with restricted access to hardware. |
| **Kernel Space** | Protected area of the operating system with direct access to hardware and critical resources. |
| **System Calls** | Controlled requests that allow applications to interact with the kernel. |

> The separation between user space and kernel space helps protect the operating system from unstable or malicious applications.

---

## 💻 Commands & Technical Examples / Comandos e Exemplos Técnicos

### Commands Used / Comandos Utilizados

No terminal commands are documented in this module because this note only records commands personally practiced during the lab.

Nenhum comando de terminal foi incluído nesta anotação, pois este repositório registra apenas comandos praticados pessoalmente durante o laboratório.

### System Exploration / Exploração do Sistema

Useful places to inspect in an operating system environment:

| Area | What to Observe |
|---|---|
| **System Information** | Operating system version, hardware details, and available resources. |
| **System Monitor** | Running processes, CPU usage, memory usage, and file systems. |
| **File Manager** | Directories, files, ownership, and organization of user data. |
| **User Settings** | User accounts, permissions, and authentication options. |

---

## 📂 File Systems / Sistemas de Arquivos

A file system organizes how data is stored and accessed on a storage device.

Um sistema de arquivos organiza como os dados são armazenados e acessados em um dispositivo de armazenamento.

Important examples:

| Concept | Description |
|---|---|
| **Directory** | A location used to organize files and other directories. |
| **File Path** | The address that identifies a file or directory within a system. |
| **Permissions** | Rules that control who can read, write, or execute files. |
| **File System Type** | The format used to organize data on a disk, such as ext4, NTFS, or FAT32. |

---

## 🛡️ Cybersecurity Relevance / Relevância para Cybersecurity

Operating system knowledge is essential in cybersecurity because it helps with:

- understanding user accounts and permissions;
- investigating running processes;
- analyzing files and directories;
- identifying unusual system behavior;
- protecting operating system resources;
- understanding the difference between normal user access and privileged access.

---

## 📝 Personal Takeaways / Meus Aprendizados

- The operating system manages the connection between applications and computer hardware.
- Kernel space has privileged access to critical system resources.
- File systems, users, processes, and permissions are important security concepts.
- Understanding how an operating system works is necessary before studying Linux, Windows security, and system investigation.

---




## 💻 CLI Commands & Examples / Comandos e Exemplos de CLI

> The commands below are documented for study and should be used only on personal systems or authorized labs.  
> Os comandos abaixo são documentados para estudo e devem ser usados somente em sistemas próprios ou laboratórios autorizados.

### 🐧 Linux CLI Basics

| Command | Purpose / Finalidade |
|---|---|
| `pwd` | Shows the current working directory / Mostra o diretório atual |
| `ls` | Lists files and directories / Lista arquivos e diretórios |
| `ls -la` | Lists all files, including hidden files / Lista inclusive arquivos ocultos |
| `cd <directory>` | Changes directory / Altera o diretório atual |
| `cd ..` | Moves one directory back / Volta um diretório |
| `cat <file>` | Displays the content of a text file / Exibe o conteúdo de um arquivo |
| `whoami` | Shows the current user / Mostra o usuário atual |
| `hostname` | Shows the machine name / Mostra o nome da máquina |
| `uname -a` | Shows system and kernel information / Mostra informações do sistema e kernel |
| `df -h` | Shows disk usage in a readable format / Mostra uso de disco de forma legível |

```bash
# Check the current directory
pwd

# List files, including hidden files
ls -la

# Enter a directory and read a text file
cd /path/to/directory
cat example.txt

# Check user, host, system, and disk information
whoami
hostname
uname -a
df -h
```

---

### 🪟 Windows CLI Basics

| Command | Purpose / Finalidade |
|---|---|
| `cd` | Shows or changes the current directory / Mostra ou altera o diretório |
| `dir` | Lists files and directories / Lista arquivos e diretórios |
| `dir /a` | Lists all files, including hidden files / Lista inclusive arquivos ocultos |
| `cd ..` | Moves one directory back / Volta um diretório |
| `type <file>` | Displays the content of a text file / Exibe o conteúdo de um arquivo |
| `whoami` | Shows the current user / Mostra o usuário atual |
| `hostname` | Shows the computer name / Mostra o nome do computador |
| `systeminfo` | Displays operating system and hardware information / Exibe informações do sistema |
| `ipconfig` | Displays basic network configuration / Exibe configuração de rede básica |
| `help` | Displays available CMD commands / Exibe ajuda do CMD |

```cmd
:: Show the current directory and list all files
cd
dir /a

:: Move to a directory and display a text file
cd C:\path\to\directory
type example.txt

:: Gather basic system information
whoami
hostname
systeminfo
ipconfig
```

---

### 🔁 Linux and Windows Comparison / Comparação

| Task / Tarefa | Linux | Windows |
|---|---|---|
| Current directory / Diretório atual | `pwd` | `cd` |
| List files / Listar arquivos | `ls` | `dir` |
| Show hidden files / Exibir ocultos | `ls -la` | `dir /a` |
| Read a text file / Ler arquivo | `cat example.txt` | `type example.txt` |
| Current user / Usuário atual | `whoami` | `whoami` |
| Machine name / Nome da máquina | `hostname` | `hostname` |
| System information / Informações do sistema | `uname -a` | `systeminfo` |
| Network information / Informações de rede | `ip addr` | `ipconfig` |

> Examples use generic paths and files. No TryHackMe flags, credentials, machine IPs, target names, or challenge answers are included.

## 🔗 References / Referências

- [TryHackMe](https://tryhackme.com/)
- [Main repository README](../../README.md)
