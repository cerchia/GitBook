# Smart Contract Escrow

A Smart Contract (SC) serves as escrow for the users' deposit funds: A Buyer sends the Premium, and a Seller sends the "discounted notional", i.e. the Notional - Premium. The total amount (the Notional) is locked in the SC if an offer is matched. Both parties can cancel their offer if it has not been matched and receive their funds back.

When the term of the protection starts, the SC fetches the level of the event index through an Oracle SC and compares this level with the level defined by the standardized details of the chosen protection (which is called the Strike \[level]). If the index level reaches the Strike during the term of the protection, a "trigger event" happens, i.e. the protection is "triggered". If, however, no trigger event happens during the term of the protection, then its maturity is reached. In both cases, the amount locked in the smart contract is released, namely:

* A trigger event is observed, and the protection amount locked is sent to the Buyer (**2a** below).
* No trigger event is observed, and maturity is reached. The protection amount locked is sent to the Seller (**2b** below).

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

In both cases, the SC reduces the amount by a platform fee. Hence the Buyer or Seller receives the Notional - Fee.

With the full protection amount securely held in (decentralized) escrow, there remains no counterparty credit risk to the transaction. Hence, no margining or clearing with a central counterparty is required.

&#x20;

![](blob:https://cerchia.atlassian.net/03e298ae-8471-44ed-901a-b7008120fa25#media-blob-url=true\&id=2ff2357b-e7c3-4e69-a71f-3a31749e1105\&collection=contentId-26640401\&contextId=26640401\&height=671\&width=935\&alt=)
