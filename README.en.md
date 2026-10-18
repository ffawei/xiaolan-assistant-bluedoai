# 小蓝助手 Blue (BlueDoAI) — Xiaolan Assistant

**When an AI agent cannot handle the work, turn to Xiaolan Assistant.**

Xiaolan Assistant is a Windows AI agent for work that involves applications, websites, local files and scripts. It can break down a task, write and run scripts, and leave editable results in a project folder. Through ADB, it can also operate supported Android applications inside the MuMu emulator and connect those steps with Windows workflows.

[中文介绍](README.md) · [Download for Windows](https://github.com/ffawei/xiaolan-assistant-bluedoai/releases/latest) · [Product](https://www.bluedoai.com/legal/product-overview-en/) · [Models and pricing](https://www.bluedoai.com/model-plaza)

## Download

The current Windows release is **1.11.31**. [Download the installer](https://github.com/ffawei/xiaolan-assistant-bluedoai/releases/download/v1.11.31/xiaolan-1.11.31-setup.exe), browse [all releases](https://github.com/ffawei/xiaolan-assistant-bluedoai/releases), or use the [official download page](https://www.bluedoai.com/tools/).

GitHub hosts unchanged copies of the existing public release files. Installer size and SHA-512 are checked against the original release metadata; each release includes a SHA-256 checksum list. Version 1.11.30 is retained as a historical release. Existing automatic update settings are unchanged.

For normal installation, download the `.exe` file. The `.blockmap` and `latest.yml` files support updates. GitHub's generated “Source code” archives contain this documentation repository, not the desktop installer or client source code.

## Use cases

- Industrial process and R&D work: organizing process documents and experiment records, running data-processing scripts, and reviewing requirement or document changes.
- Photoshop image processing with explicit size, format and visual requirements.
- Android application operations through MuMu and Android Debug Bridge (ADB).
- Saving permitted video materials and organizing titles, descriptions and source links.
- Writing, running and revising scripts for multi-step or batch work.
- Combining website content, Android app content and local files into editable deliverables.

Task outcomes depend on the installed application versions, permissions, selected model and available inputs. Start with a small sample and inspect the results. These are supported directions, not a guarantee that every task or application can be automated.

Xiaolan Assistant has manufacturing customer use cases. Enterprises can discuss applications for their own process documentation, R&D tasks and existing workflows, including local deployment and technical support. Process parameters, equipment actions, safety and product-performance conclusions require review by the responsible professionals.

## Guides and task templates

- [MuMu and ADB setup preparation](docs/mumu-adb.md)
- [Video and text materials](examples/video-materials.md)
- [Photoshop image processing](examples/photoshop-images.md)
- [Cross-application work](examples/cross-app-work.md)

The Chinese templates describe tasks you can adapt. They are not completed customer case studies or execution benchmarks.

## Pricing and repository scope

The assistant itself is free to use. Users can connect their own model API or supported local compute according to the current client documentation. BlueDoAI hosted model calls are billed by actual usage; available models and prices are listed on the website. Enterprise deployment, training and project services are quoted separately.

This repository contains product documentation and task templates, not the desktop client's source code. Use only content you own or are authorized to process, and follow the relevant application's rules. MuMu, Android and Adobe Photoshop are names of their respective owners; no partnership or endorsement is implied.

Website: <https://www.bluedoai.com/>  
Contact: <blue@bluedoai.com>
