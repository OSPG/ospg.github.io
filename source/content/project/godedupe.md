---
title: "Godedupe"
description: ""
date: 2018-07-29T12:16:37+02:00
categories: ["go", "utilities"]
tags: ["go","deduplication"]
layout: subsection
slug: godedupe
draft: false
weight: 201
---

#### *Project URL*: [github.com/OSPG/godedupe](https://github.com/OSPG/godedupe)
#### *Language*: Go
#### *Summary*: An utility to find duplicated files.

---

Godedupe finds duplicated files like fdupes does. Unlike fdupes, we focus on
speed and features. It also have sane defaults which should make it easier to
use than fdupes.

It have been tested to work on Linux and Windows.

The algoirhtm consist of three phases.

  * First it checks the file size of the files.
  * For files that have the same size, the checksum of a first block (1024B) is
    used
  * For files that have the same checksum, it generate a checksum of all the
    file which

If two files have the same checksum, they are considered to be the same file.



