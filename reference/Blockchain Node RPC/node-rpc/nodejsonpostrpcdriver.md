---
title: Connect to the blockchain node through an RPC driver
excerpt: >
  <p><b>The number of credits consumed depends on the number of methods
  submitted in an API call:<br/>

  * 50 credits per debug*/trace* method (for EVM-based blockchains)<br/>

  * 50 credits per EOS <a
  href="https://developers.eos.io/manuals/eos/v2.0/nodeos/plugins/trace_api_plugin/api-reference/index"
  target="_blank">Trace API</a> methods <br/>

  * 5 credits per eth_call method (for EVM-based blockchains)<br/>

  * 2 credits per any other RPC method</b></p>

  <p>Connect directly to the blockchain node provided by Tatum.</p>

  <p>The <code>POST</code> method is used. The API endpoint URL acts as an
  HTTP-based RPC driver.</p>
api:
  file: api.json
  operationId: NodeJsonPostRpcDriver
hidden: false
---