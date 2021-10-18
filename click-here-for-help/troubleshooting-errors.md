---
description: Common error messages. Use the sidebar ➡️to jump to the error you're seeing.
---

# Troubleshooting Errors

![](../.gitbook/assets/NEWBAN.jpg)

Sometimes you may find yourself facing a problem that doesn't have a clear solution. These troubleshooting tips may help you solve problems you run into.

## Issues with the Farms

### Out of Gas Error

> Warning! Error encountered during contract execution \[out of gas]

You have set a low gas limit when trying to make a transaction.

{% tabs %}
{% tab title="Solution" %}
Try manually increasing the **gas limit** (not gas price!) in your wallet before signing the transaction.

A limit of 200000 is usually enough.

![](https://files.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-MHREX7DHcljbY5IkjgJ%2F-MWxtg35bMTu-jgHaZjz%2F-MWy0GU0AvB9KPJgcCYV%2Fimage.png?alt=media\&token=e4850a43-199f-4dac-8c0d-fdbc68453121)

The above example is from Metamask; check your wallet's documentation if you aren't sure how to adjust the gas limit.
{% endtab %}

{% tab title="Reason" %}
This happens when you set a limit on your spend allowance when you first approved the contract, then try to swap more than the limit.
{% endtab %}
{% endtabs %}

### BEP20: transfer amount exceeds allowance

> Fail with error 'BEP20: transfer amount exceeds allowance'

{% tabs %}
{% tab title="Solution" %}
1. Use Unrekt.net to revoke approval for the smart contract you're trying to interact with
2. Approve the contract again, without setting a limit on spend allowance
3. Try interacting with the contract again.
{% endtab %}

{% tab title="Reason" %}
This happens when you set a limit on your spend allowance when you first approved the contract, then try to swap more than the limit
{% endtab %}
{% endtabs %}

## Other Issues

### Provider Error

> Provider Error\
> No provider was found

This happens when you try to connect via a browser extension like MetaMask or Binance Chain Wallet, but you haven’t installed the extension.

{% tabs %}
{% tab title="Solution" %}
Install the official browser extension to connect, or read our guide on [how to connect a wallet to PancakePoll](../get-started/connection-guide.md).
{% endtab %}
{% endtabs %}

### Unsupported Chain ID

{% tabs %}
{% tab title="Solution" %}
Switch your chain to Binance Smart Chain. Check your wallet's documentation for a guide if you need help.
{% endtab %}
{% endtabs %}

### Internal JSON-RPC errors

> "MetaMask - RPC Error: Internal JSON-RPC error. estimateGas failed removeLiquidityETHWithPermitSupportingFeeOnTransferTokens estimateGas failed removeLiquidityETHWithPermit "

Happens when trying to remove liquidity on some tokens via Metamask. Root cause is still unknown. Try using an alternative wallet.

> Internal JSON-RPC error. { "code": -32000, "message": "insufficient funds for transfer" } - Please try again.

You don't have enough BNB to pay for the transaction fees. You need more BEP-20 network BNB in your wallet.

### Error: \[ethjs-query]

> Error: \[ethjs-query] while formatting outputs from RPC '{"value":{"code":-32603,"data":{"code":-32000,"message":"transaction underpriced"}}}"

Increase the gas limit for the transaction in your wallet. Check your wallet's documentation to learn how to increase gas limit.

> Swap failed: Error: \[ethjs-query] while formatting outputs from RPC '{"value":{"code":-32603,"data":{"code":-32603,"message":"handle request error"}}}'

Cause unclear. Try these steps before trying again:

1. Increase gas limit
2. Increase slippage
3. Clear cache

## Issues with the Profie
