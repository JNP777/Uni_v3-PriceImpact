# Uni_v3-PriceImpact
Calculate price impact for swapping different qtys in a specific Uniswap_v3 pool

Calling func:
  get_tradeImpact(pool_id,tokenIn,qtyIn)
  
  pool_id (address) = Uniswap_v3 pool address (lowercase)
  tokenIn (int) = token to swap identified as 0 or 1 (i.e. in USDC/WETH pair USDC = 0 and WETH = 1)
  qtyIn (list) = list of tokens quantity to swap (i.e [1,10,100])
  
return a dict with :
  final pool price
  swap price
  price impact of both (%)

This script requires the python file UNI_v3_funcs.py stored on this Github repository UNI_V-Liquidity-calcs
