# What is SAST? 

**Static Application Security Testing** or **SAST** is an Application Security Tool. It is used to test an application’s binary, source, or byte code during the development cycle or code reviews. A white-box testing solution can discover the root cause of vulnerabilities and help in remedying the underlying security defects.

Many SAST application can analyze source code inside-out and it doesn’t require a running system for performing a code evaluation to locate security weaknesses.

Static application security scanning can reduce security vulnerabilities in programs by presenting immediate remarks to developers on problems introduced in the application source code during the application security testing. So, it educates developers about security flaws when they're working, providing them real-time access to line-of-code navigation and recommendations that allow quicker collaborative auditing and vulnerability discovery. 

A SAST solution aid developers create secure code that is much less vulnerable to compromise and leads to the development of a more secure software.

The term 'Static Code Analysis' is used to refer to program comprehension. SAST is an automated tool for secure code review.

# SAST advantages?

- Examine the codebase of a software in a single test

- Test a software before compiling or running the code

- Identify vulnerabilities early in the software program SDLC. At this phase vulnerability are simplest and cheapest to fix

- Reduction in manual evaluation efforts by an analyst

- Effective and efficient in identifying all the instances of a specific vulnerability

- Scans source code to discover weaknesses that cause vulnerabilities

- Provides real-time reporting

- Cover multiple languages that developers use

# How Does Static Code Analysis Work?

![This is an image](https://deepsource.io/images/blog/static-analysis-python/pipeline.png)
For more information about how Static Code Analysis work check the following article:
- [A hands-on introduction to static code analysis](https://deepsource.io/blog/introduction-static-code-analysis/)
- 
# Open Source SAST tools

## Semgrep

### What is Semgrep?

![This is an image](https://raw.githubusercontent.com/returntocorp/semgrep/develop/semgrep.svg)

- Semgrep is a fast, open-source, static analysis tool for finding bugs and enforcing code standards at editor, commit, and CI time.

- Semgrep analyzes code locally on the computer or in the build environment: code is never uploaded.

- Semgrep supports 20+ languages [[Link](https://semgrep.dev/docs/)].

### Requirements

You need to install [Docker](https://github.com/ArijMekki/Open-Source-SAST/blob/main/Docker.md) and [Docker compose](https://github.com/ArijMekki/Open-Source-SAST/blob/main/Docker_Compose.md) in order to run the Semgrep and [ELK](https://github.com/ArijMekki/Open-Source-SAST/blob/main/ELK.md) images.

### Installation

#### Docker image installation

To install the semgrep docker image, you can run the following command:

  `$docker pull returntocorp/semgrep:latest`

To verify your installation: 

  `$docker run  -v "${PWD}:/src" returntocorp/semgrep semgrep scan --version`

### Usage

