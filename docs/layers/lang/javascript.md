---
title: "SpaceVim lang#javascript layer"
description: "This layer is for JaveScript development"
---

# [Available Layers](../../) >> lang#javascript

<!-- vim-markdown-toc GFM -->

- [Description](#description)
- [Install](#install)
- [Features](#features)
- [Layer configuration](#layer-configuration)
- [Key bindings](#key-bindings)
  - [Import key bindings](#import-key-bindings)
  - [Generate key bindings](#generate-key-bindings)

<!-- vim-markdown-toc -->

## Description

This layer is for JavaScript development.

## Install

To use this configuration layer, update custom configuration file with:

```toml
[[layers]]
name = "lang#javascript"
```

## Features

- auto-completion
- syntax checking
- goto definition
- refernce finder

## Layer configuration

`auto_fix`: auto fix problems when saving files, disabled by default.

`enable_flow_syntax`: Enable configuration for [flow](https://flow.org/), disabled by default.

If you need these features, you can enable them in the layer config:
```toml
[[layers]]
name = "lang#javascript"
auto_fix = true
enable_flow_syntax = true
```

## Key bindings

### Import key bindings

| Key Binding          | Description                     |
| -------------------- | ------------------------------- |
| `F4` (Insert/Normal) | Import symbol under cursor      |
| `SPC j i`            | Import symbol under cursor      |
| `SPC j f`            | Import missing symbols          |
| `SPC j g`            | Jump to module under cursor     |
| `<C-j>i` (Insert)    | Import symbol under cursor      |
| `<C-j>f` (Insert)    | Import missing symbols          |
| `<C-j>g` (Insert)    | Jump to module under cursor     |

### Generate key bindings

| Mode          | Key Binding | Description                           |
| ------------- | ----------- | ------------------------------------- |
| normal        | `SPC l g d` | Generate JSDoc                        |
