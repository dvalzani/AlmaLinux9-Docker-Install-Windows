# Installation Guide: AlmaLinux 9 on Docker

## Introduction

This guide explains what Docker is, why it is useful, and how to install and run AlmaLinux 9 inside a Docker container on Windows

## What is Docker and Why we use it?
Docker is a containerization platform that allows you to run applications or entire operating systems in an isolated environment called a container. Unlike virtual machines, containers share the host OS kernel, making them lighter, faster, and more efficient.

## STEP 1: Install Docker
First we have to check if WSL 2 is enabled, WSL 2 (Windows Subsystem for Linux 2) is a feature in Windows 10 and Windows 11 that allows you to run a full Linux environment directly inside Windows without using a virtual machine. We use Power Shell (or any other terminal is good):
1.  Check if WSL 2 is enabled by running: `wsl --list --verbose`  
 If note installed, run: `wsl --install`  
 Then restart your computer.
2. Download and Install Docker Desktop from https://www.Docker.com
   ![Alt Text](images/docker_windows_download.png)
3. Enable WSL 2 Beckend during installation
4. Verify installation by running:  
   `docker --version`  
   `docker run hello-world`  
   If you see "Hello from Docker!", installation is successful!

## STEP 2: Download and Run AlmaLinux 9
## Why AlmaLinux 9
AlmaLinux 9 is a free, open-source Linux distribution designed as a binary-compatible replacement for Red Hat Enterprise Linux (RHEL). It is widely used in enterprise environments, cloud computing, and server applications due to its stability, security, and long-term support. When combined with Docker, AlmaLinux becomes even more powerful, allowing users to run it in an isolated containerized environment without needing a full installation on their system. This makes it ideal for testing, development, and deployment while maintaining consistency across different machines. Using AlmaLinux with Docker ensures that applications run in a predictable and controlled Linux environment, independent of the host operating system.

