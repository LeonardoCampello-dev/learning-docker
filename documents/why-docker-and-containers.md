# Why containers?

Why would we want **independent, santandardized "application packages?"**

> Different Development & Production Environments

We want to build and test in exactly (!) the same environment as we later run our app in

> Different Development Environments Within a Team / Company

Every team member should have the exactly (!) same environment when working on the same project

> Clashing Tools / Versions Between Different Projects

When switching between different projects, tools used in project A should not clash with tools used in project B

## The problems

### **Environment:** The runtimes, languages, frameworks you need for development

Development Environment <-> Production Environment

- often not the same

Development Environment for Employee A <-> Development Environment for Employee B

- often not the same

Tools & Libraries required for Project A <-> Tools & Libraries required for Project B

- often not the same

## We Want Reliability & Reproducible Environments

- We want to have the **exact same environment for development and production.** This ensures that it works exactly as tested
- It should be easy to **share a common development environment /** setup with (new) employees and colleagues
- We **dont want to uninstall and re-install** local dependencies and runtimes all the time
