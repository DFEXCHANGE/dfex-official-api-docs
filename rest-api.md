**DFEX**

**HTTP Requests**

GET /api/account/v3/currencies

**Request Sample**

GET /polarisex/coin/currencies

**Return Parameters**

Parameters	    Parameters Types	Description
:---:|:---:|:---:
currency	    String	            Token code
name	        String	            Token name
can_deposit	    String	            availability of depositing, 0 = not available，1 = available
can_withdraw	String	            availability of withdrawal，0 = not available，1 = available
min_withdrawal	String	            the minimum withdrawal limit

Return Sample

{
         "can_deposit":"1",
         "can_withdraw":"1",
         "currency":"BTC",
         "min_withdrawal":"0.01",
         "name":""
     },
     {
         "can_deposit":"1",
         "can_withdraw":"1",
         "currency":"LTC",
         "min_withdrawal":"0.1",
         "name":""
     }