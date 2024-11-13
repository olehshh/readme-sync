---
title: postLocalCommand
excerpt: |
  Blocking/sync call to submit a command for non-transactional execution. In a
  blockchain environment this would be a node-local “dirty read”, which can
  either serve as a node-local repl execution, or fully gassed transaction
  simulation and transaction validation. Any database writes or changes to the
  environment are rolled back.
api:
  file: api.json
  operationId: rpc-kadena-postlocalcommand
hidden: false
---