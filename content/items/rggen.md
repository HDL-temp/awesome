---
title: "RgGen"
description: "Code generator for configuration and status registers"
authors:
  - Taichi Ishitani
links:
  gh: "rggen/rggen"
  docs: "https://github.com/rggen/rggen/wiki"
tags:
  - code-generator
  - csr
  - configuration-register
  - systemverilog
  - verilog
  - UVM-reg
categories:
  - Tools
licenses:
  - MIT
active:
  from: 2016
talk: 208
---

RgGen is a code generator tool to generate source files for configuration and status registers (CSR) from human readable register map specifications.

RgGen has following features:

* Generate following source files for CSR automatically from register map specifications
    * SystemVerilog/Verilog RTL
    * VHDL RTL
        * Now implementing
    * UVM register model (RAL)
    * Markdown documents
* Register map specifications can be written in following format
    * YAML
    * JSON
    * TOML
    * Spreadsheet (xlsx/xls/ods/csv/tsv)
    * SiFive DUH
    * Ruby
    * SystemRDL
        * Now planning
* Plugin feature
    * Add your own bit field types
    * Add your own bus protocol
