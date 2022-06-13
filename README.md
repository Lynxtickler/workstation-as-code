# Workstation-as-code
A framework for workstation state maintenance, and interface definition for implementing engines.

## What?
This project is the framework definition for maintaining a workstation as code configuration.
It consists of two parts:
1. The interface regarding the whole file and directory structure.
1. The required interface(s) for any engines that implement the actual file processing.

## Why?
I have worked closely with DevOps and Infrastructure as Code (IaC) nearly the whole time I've worked in IT.
During that time, I've developed a strong love towards Everything as Code.
Nowadays I absolutely despise setting up anything by clicking around, making it hard to replicate the perfect setup.
This is why I'm suggesting Workstation as Code (WaC) for maintaining ideal and identical configurations between workstations.

## How?
The user of this framework is to set up a repository, carefully placing the desired config files in right places, according to the defined structure interface.
Afterwards, they select an engine or multiple engines to be imported as git submodules.
The engine will then handle copying the right files into the right destinations.
The target computer has to only have git and the requirements for any of the engines installed.
