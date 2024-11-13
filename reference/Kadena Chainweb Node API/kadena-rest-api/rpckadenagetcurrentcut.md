---
title: getCurrentCut
excerpt: |
  A cut represents a distributed state of a chainweb. It references one
  block header for each chain, such that those blocks are pairwise
  concurrent.

  Two blocks from two different chains are said to be concurrent if either
  one of them is an adjacent parent (is a direct dependency) of the other or
  if the blocks do not depend at all on each other.
api:
  file: api.json
  operationId: rpc-kadena-getcurrentcut
hidden: false
---