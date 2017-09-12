# Proof helper library for interacting with truffle contract objects. 
Useful for scripts and tests within the truffle environment

# API Reference

## Modules

<dl>
<dt><a href="#module_token-sale-helpers">token-sale-helpers</a></dt>
<dd><p>Token Sale Helpers Module</p>
</dd>
<dt><a href="#module_token-helpers">token-helpers</a></dt>
<dd><p>Token helpers module</p>
</dd>
<dt><a href="#module_pausable-helpers">pausable-helpers</a></dt>
<dd><p>Pausable helpers module</p>
</dd>
<dt><a href="#module_ownership-helpers">ownership-helpers</a></dt>
<dd><p>Ownership helpers module</p>
</dd>
</dl>

<a name="module_token-sale-helpers"></a>

## token-sale-helpers
Token Sale Helpers Module


* [token-sale-helpers](#module_token-sale-helpers)
    * [getWallet](#exp_module_token-sale-helpers--getWallet) ⇒ <code>String</code> ⏏
    * [getToken](#exp_module_token-sale-helpers--getToken) ⇒ <code>String</code> ⏏
    * [getPresaleToken](#exp_module_token-sale-helpers--getPresaleToken) ⇒ <code>String</code> ⏏
    * [getCap](#exp_module_token-sale-helpers--getCap) ⇒ <code>String</code> ⏏
    * [getPriceInWei](#exp_module_token-sale-helpers--getPriceInWei) ⇒ <code>String</code> ⏏
    * [buyTokens](#exp_module_token-sale-helpers--buyTokens) ⇒ <code>Object</code> ⏏
    * [tokenPriceInWei](#exp_module_token-sale-helpers--tokenPriceInWei) ⇒ <code>Number</code> ⏏
    * [tokenPrice](#exp_module_token-sale-helpers--tokenPrice) ⇒ <code>Number</code> ⏏
    * [numberOfTokensFor](#exp_module_token-sale-helpers--numberOfTokensFor) ⇒ <code>Number</code> ⏏

<a name="exp_module_token-sale-helpers--getWallet"></a>

### getWallet ⇒ <code>String</code> ⏏
Returns wallet address for input token sale contract

**Kind**: Exported member  
**Returns**: <code>String</code> - wallet  

| Param | Type | Description |
| --- | --- | --- |
| tokenSale | <code>Object</code> | Truffle Contract Object |

<a name="exp_module_token-sale-helpers--getToken"></a>

### getToken ⇒ <code>String</code> ⏏
Returns token address for input token sale contract

**Kind**: Exported member  
**Returns**: <code>String</code> - token  

| Param | Type | Description |
| --- | --- | --- |
| tokenSale | <code>Object</code> | Truffle Contract Object |

<a name="exp_module_token-sale-helpers--getPresaleToken"></a>

### getPresaleToken ⇒ <code>String</code> ⏏
Returns presale token for input token sale contract

**Kind**: Exported member  
**Returns**: <code>String</code> - token  

| Param | Type | Description |
| --- | --- | --- |
| tokenSale | <code>Object</code> | Truffle Contract Object |

<a name="exp_module_token-sale-helpers--getCap"></a>

### getCap ⇒ <code>String</code> ⏏
Returns cap for input token sale contract

**Kind**: Exported member  
**Returns**: <code>String</code> - token sale cap  

| Param | Type | Description |
| --- | --- | --- |
| tokenSale | <code>Object</code> | Truffle Contract Object |

<a name="exp_module_token-sale-helpers--getPriceInWei"></a>

### getPriceInWei ⇒ <code>String</code> ⏏
Returns the price in wei of one token sold by the input token sale contract

**Kind**: Exported member  
**Returns**: <code>String</code> - token price in wei  

| Param | Type | Description |
| --- | --- | --- |
| tokenSale | <code>Object</code> | Truffle Contract Object |

<a name="exp_module_token-sale-helpers--buyTokens"></a>

### buyTokens ⇒ <code>Object</code> ⏏
Performs an token order from sender to the input token sale contract

**Kind**: Exported member  
**Returns**: <code>Object</code> - txnReceipt  - Transaction receipt  

| Param | Type | Description |
| --- | --- | --- |
| tokenSale | <code>Object</code> | Truffle Contract Object corresponding to token sale contract |
| sender | <code>String</code> | Ethereum address from which ether is being sent |
| value | <code>Number</code> | Value to be send to the contract |

<a name="exp_module_token-sale-helpers--tokenPriceInWei"></a>

### tokenPriceInWei ⇒ <code>Number</code> ⏏
Returns the token price in wei

**Kind**: Exported member  
**Returns**: <code>Number</code> - token price in wei  

| Param | Type | Description |
| --- | --- | --- |
| tokenSale | <code>Object</code> | Truffle Contract Object |

<a name="exp_module_token-sale-helpers--tokenPrice"></a>

### tokenPrice ⇒ <code>Number</code> ⏏
Returns the token price

**Kind**: Exported member  
**Returns**: <code>Number</code> - token price in ether  

| Param | Type | Description |
| --- | --- | --- |
| tokenSale | <code>Object</code> | Truffle Contract Object |

<a name="exp_module_token-sale-helpers--numberOfTokensFor"></a>

### numberOfTokensFor ⇒ <code>Number</code> ⏏
Returns number of tokens for a certain amount of ether sent to a token sale contract

**Kind**: Exported member  
**Returns**: <code>Number</code> - number of tokens  

| Param | Type | Description |
| --- | --- | --- |
| tokenSale | <code>Object</code> | Truffle Contract Object |
| weiAmount | <code>Number</code> |  |

<a name="module_token-helpers"></a>

## token-helpers
Token helpers module


* [token-helpers](#module_token-helpers)
    * [~getOwner](#module_token-helpers..getOwner) ⇒
    * [~getTotalSupply](#module_token-helpers..getTotalSupply) ⇒
    * [~getTokenBalance](#module_token-helpers..getTokenBalance) ⇒
    * [~transferToken](#module_token-helpers..transferToken) ⇒
    * [~transferTokens](#module_token-helpers..transferTokens) ⇒
    * [~mintToken](#module_token-helpers..mintToken) ⇒
    * [~finishMinting](#module_token-helpers..finishMinting) ⇒
    * [~baseUnits](#module_token-helpers..baseUnits) ⇒
    * [~ERC20Units](#module_token-helpers..ERC20Units) ⇒
    * [~claimTokens](#module_token-helpers..claimTokens) ⇒
    * [~importBalances](#module_token-helpers..importBalances) ⇒

<a name="module_token-helpers..getOwner"></a>

### token-helpers~getOwner ⇒
Get owner of token contract

**Kind**: inner property of [<code>token-helpers</code>](#module_token-helpers)  
**Returns**: owner  

| Param |
| --- |
| token | 

<a name="module_token-helpers..getTotalSupply"></a>

### token-helpers~getTotalSupply ⇒
Get total supply of token contract

**Kind**: inner property of [<code>token-helpers</code>](#module_token-helpers)  
**Returns**: total supply  

| Param |
| --- |
| token | 

<a name="module_token-helpers..getTokenBalance"></a>

### token-helpers~getTokenBalance ⇒
Get token balance of owner

**Kind**: inner property of [<code>token-helpers</code>](#module_token-helpers)  
**Returns**: token balance  

| Param |
| --- |
| token | 
| owner | 

<a name="module_token-helpers..transferToken"></a>

### token-helpers~transferToken ⇒
Transfer amount of token from sender to receiver

**Kind**: inner property of [<code>token-helpers</code>](#module_token-helpers)  
**Returns**: transaction receipt  

| Param |
| --- |
| token | 
| sender | 
| receiver | 
| amount | 

<a name="module_token-helpers..transferTokens"></a>

### token-helpers~transferTokens ⇒
Transfer amount of each token in the tokens array from sender to receiver

**Kind**: inner property of [<code>token-helpers</code>](#module_token-helpers)  
**Returns**: transaction receipts  

| Param |
| --- |
| token | 
| sender | 
| receiver | 
| amount | 

<a name="module_token-helpers..mintToken"></a>

### token-helpers~mintToken ⇒
Mint amount of token for the receiver. Only works if minter is the owner of the token

**Kind**: inner property of [<code>token-helpers</code>](#module_token-helpers)  
**Returns**: transaction receipt  

| Param |
| --- |
| contract | 
| minter | 
| receiver | 
| amount | 

<a name="module_token-helpers..finishMinting"></a>

### token-helpers~finishMinting ⇒
Finish minting period for the token contract. Only works if sender is the owner of the token

**Kind**: inner property of [<code>token-helpers</code>](#module_token-helpers)  
**Returns**: transaction receipt  

| Param |
| --- |
| token | 
| sender | 

<a name="module_token-helpers..baseUnits"></a>

### token-helpers~baseUnits ⇒
Convert ERC20 units (=number of base units times 10^decimals) to base units

**Kind**: inner property of [<code>token-helpers</code>](#module_token-helpers)  
**Returns**: base units  

| Param |
| --- |
| token | 
| amount | 

<a name="module_token-helpers..ERC20Units"></a>

### token-helpers~ERC20Units ⇒
Convert base units (=number of ERC20 units divided by 10^decimals) to ERC20 units

**Kind**: inner property of [<code>token-helpers</code>](#module_token-helpers)  
**Returns**: ERC20 units  

| Param |
| --- |
| token | 
| amount | 

<a name="module_token-helpers..claimTokens"></a>

### token-helpers~claimTokens ⇒
Allocates (presale) tokens to the sender

**Kind**: inner property of [<code>token-helpers</code>](#module_token-helpers)  
**Returns**: transaction receipt  

| Param |
| --- |
| token | 
| sender | 

<a name="module_token-helpers..importBalances"></a>

### token-helpers~importBalances ⇒
Import presale tokens to the token sale contract

**Kind**: inner property of [<code>token-helpers</code>](#module_token-helpers)  
**Returns**: transaction receipt  

| Param |
| --- |
| token | 
| addresses | 
| balances | 

<a name="module_pausable-helpers"></a>

## pausable-helpers
Pausable helpers module


* [pausable-helpers](#module_pausable-helpers)
    * [~pause](#module_pausable-helpers..pause)
    * [~unpause](#module_pausable-helpers..unpause)

<a name="module_pausable-helpers..pause"></a>

### pausable-helpers~pause
Pause the contract and wait until the transaction is mined

**Kind**: inner property of [<code>pausable-helpers</code>](#module_pausable-helpers)  

| Param | Description |
| --- | --- |
| contract | Token truffle contract |
| owner | Ethereum Address |

<a name="module_pausable-helpers..unpause"></a>

### pausable-helpers~unpause
Unpause contract and wait until the transaction is mined

**Kind**: inner property of [<code>pausable-helpers</code>](#module_pausable-helpers)  

| Param | Description |
| --- | --- |
| contract | Token Truffle Contract |
| owner | Ethereum Address |

<a name="module_ownership-helpers"></a>

## ownership-helpers
Ownership helpers module


* [ownership-helpers](#module_ownership-helpers)
    * [~transferOwnership](#module_ownership-helpers..transferOwnership) ⇒ <code>Object</code>
    * [~transferOwnerships](#module_ownership-helpers..transferOwnerships)
    * [~lockOwnership](#module_ownership-helpers..lockOwnership) ⇒ <code>Object</code>

<a name="module_ownership-helpers..transferOwnership"></a>

### ownership-helpers~transferOwnership ⇒ <code>Object</code>
Transfer ownership of input contract and wait until corresponding transaction is mined

**Kind**: inner property of [<code>ownership-helpers</code>](#module_ownership-helpers)  
**Returns**: <code>Object</code> - transaction receipt  

| Param | Type | Description |
| --- | --- | --- |
| contract | <code>Object</code> | Truffle Contract Object |
| sender | <code>String</code> |  |
| receiver | <code>String</code> |  |

<a name="module_ownership-helpers..transferOwnerships"></a>

### ownership-helpers~transferOwnerships
Transfer the ownerships of input contracts and wait until corresponding transactions are mined

**Kind**: inner property of [<code>ownership-helpers</code>](#module_ownership-helpers)  

| Param | Type | Description |
| --- | --- | --- |
| contracts | <code>Object</code> | Truffle Object Contract Array |
| sender | <code>String</code> |  |
| receiver | <code>String</code> |  |

<a name="module_ownership-helpers..lockOwnership"></a>

### ownership-helpers~lockOwnership ⇒ <code>Object</code>
Lock ownership of input contract and wait until corresponding transaction is mined

**Kind**: inner property of [<code>ownership-helpers</code>](#module_ownership-helpers)  
**Returns**: <code>Object</code> - Transaction Receipt  

| Param | Type | Description |
| --- | --- | --- |
| contract | <code>Object</code> | Truffle Object Contract Array |
| owner | <code>String</code> | - |

