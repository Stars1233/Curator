---
description: "Essential concepts for video data curation including distributed processing, pipeline stages, and execution modes"
categories: ["concepts-architecture"]
tags: ["concepts", "video-curation", "distributed", "pipeline", "ray", "autoscaling"]
personas: ["data-scientist-focused", "mle-focused"]
difficulty: "beginner"
content_type: "concept"
modality: "video-only"
only: not ga
---

(about-concepts-video)=
# Video Curation Concepts

This document covers the essential concepts for video data curation in NVIDIA NeMo Curator. These concepts assume basic familiarity with data science and machine learning principles.

## Core Concept Areas

Video curation in NVIDIA NeMo Curator focuses on these key areas:

::::{grid} 1 1 1 2
:gutter: 1 1 1 2

:::{grid-item-card} {octicon}`server;1.5em;sd-mr-1` Architecture
:link: about-concepts-video-architecture
:link-type: ref

Core concepts for distributed processing, Ray foundation, and autoscaling
:::

:::{grid-item-card} {octicon}`gear;1.5em;sd-mr-1` Key Abstractions
:link: about-concepts-video-abstractions
:link-type: ref

Stages, pipelines, and execution modes in video curation workflows
:::

:::{grid-item-card} {octicon}`sync;1.5em;sd-mr-1` Data Flow
:link: about-concepts-video-data-flow
:link-type: ref

How data moves through the system, from ingestion to output
:::

::::

## Infrastructure Components

The video curation concepts build on NVIDIA NeMo Curator's core infrastructure components, which are shared across all modalities (text, image, video). These components include:

::::{grid} 1 1 1 2
:gutter: 1 1 1 2

:::{grid-item-card} {octicon}`server;1.5em;sd-mr-1` Distributed Computing
:link: reference-infra-dist-computing
:link-type: ref
Configure and manage distributed processing across multiple machines
+++
{bdg-secondary}`dask`
{bdg-secondary}`clusters`
{bdg-secondary}`scaling`
:::

:::{grid-item-card} {octicon}`database;1.5em;sd-mr-1` Memory Management
:link: reference-infra-memory-management
:link-type: ref
Optimize memory usage when processing large datasets
+++
{bdg-secondary}`partitioning`
{bdg-secondary}`batching`
{bdg-secondary}`monitoring`
:::

:::{grid-item-card} {octicon}`zap;1.5em;sd-mr-1` GPU Acceleration
:link: reference-infra-gpu-processing
:link-type: ref
Leverage NVIDIA GPUs for faster data processing
+++
{bdg-secondary}`cuda`
{bdg-secondary}`rmm`
{bdg-secondary}`performance`
:::

:::{grid-item-card} {octicon}`sync;1.5em;sd-mr-1` Resumable Processing
:link: reference-infra-resumable-processing
:link-type: ref
Continue interrupted operations across large datasets
+++
{bdg-secondary}`checkpoints`
{bdg-secondary}`recovery`
{bdg-secondary}`batching`
:::

::::

```{toctree}
:maxdepth: 2
:titlesonly:
:hidden:

Architecture <architecture.md>
Key Abstractions <abstractions.md>
Data Flow <data-flow.md>
```
