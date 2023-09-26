# Understanding the Parameters

You can place a deal or match an open order once all parameters are defined.

Parameters include:

* Risk
* Country
* Region
* Strike
* Term

{% hint style="info" %}
Note that the selected currency and the blockchain are essential parameters as well. If the currency or blockchain deviates from a potential counterparty you won't see its open order or vice versa.
{% endhint %}

Once all parameters are selected, the system assigns a "symbol" which is the reference to a marketplace. You can trade with counterparties which are eager to trade with the exact same parameters.

<div align="left">

<figure><img src="../.gitbook/assets/image (29).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

**Symbol/ Standard: AABBCCDDEEFFFGH**

* _AA - Country_
* _BB - Type = Meteorological/ Climatological/ Cyber etc._
* _CC - Peril = Hurricane/ Wildfire etc._
* _DD - Region = Florida/ California etc._
* _EE - Index = e.g. IL (Industry Loss)_
* _FFF - Strike Level in USD bn_
* _G - Month of expiry according to futures codes_
* _H - Year of expiry_

Find in the following two example Symbols:

**GLCYALNOIL010Z23**

* GL = Global
* CY = Cyber
* AP = all perill
* NO = no region
* IL = Industry Loss
* 010 = 10bn
* Z = December
* 23 = 2023

**USMEHUFLIL100U23**

* US - Country
* ME - Type = Meteorological
* HU - Peril = Hurricane
* FL - Region = Florida
* IL - Index = Industry Loss
* 100 - Strike
* U - Month of expiry according to futures codes
* 23 - Year of expiry

An important parameter is the strike level. In below example you see industry loss in USD for a peril. The amount refers to the loss insurance companies expect caused by a peril. Stikes can have any value which can be binary determined - where a true or false condition can be met.

<div align="left">

<figure><img src="../.gitbook/assets/image.png" alt="" width="375"><figcaption></figcaption></figure>

</div>

Terms are mainly set in 3-months units. This supports the mission to standartise Risk Transfer.

<div align="left">

<figure><img src="../.gitbook/assets/image (1).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

Once a Standard is selected you can place your Ask or Bid offer.

* Notional is the full amount of cover which will be held in escrow
* Premium is the amount offered to get Protection
  * the buyer pays the Premium
  * the seller pays the notional (minus the premium)&#x20;

<div align="left">

<figure><img src="../.gitbook/assets/image (2).png" alt="" width="375"><figcaption></figcaption></figure>

</div>
