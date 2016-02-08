Shareholder Summary
===================

Thanks to some keen external developers, we are soon to see the [BSIP#10](https://github.com/bitshares/bsips/blob/master/bsip-0010.md) feature that will allow for percentage based transfer fees and give the BitShares ecosystem some much needed flexibility to serve the needs of different cultures. Another idea that came up recently was possibility of rate limiting accounts based on stake but offering transfers for free, which would help us to gain an unfair advantage over other cryptocurrency ecosystems while allowing BitShares to charge for other operations, such as trading and asset registration. At this stage, the the discussions are just beginning and will likely take several more weeks to complete.

To begin to resolve the highly debated fee issue for the BitShares community and most of the existing businesses, the committee members have decided to step up and act now, with the option for modifications once BSIP#10 is available.

After several days of intensive discussion, we've constructed a whole new fee schedule for the BitShares ecosystem that **drastically reduces** the fees required for the **core features**, namely, *transfers* and *trading*, but increases the fees for more specialized operations. By this, we keep the referral program functional and can attract more customers by providing the features that other service providers have, but still offer them at competitive rates and all in one place. 

Even though a lot of ideas and discussion has gone into the schedule we are presenting now, we will still have plenty more options to choose from once BSIP#10 or the rate-limited free transfer is available to be implemented for bitassets owned by the committee. However, for now we propose to give everyone the opportunity to make use of a low flat fee for all transfers within the network, by setting a rate of $0.018 (less than 6 BTS at current valuation) per transfer. Keep in mind that this will be a **limited-time offer**, as the minimum fee may be raised once BSIP#10 is implemented.

We would like to further encourage traders and market makers to provide liquidity by asking for only $0.001 per created order (with 90% refund upon cancellation, if unfilled) and a low 0.1% trading fee for committee owned assets such as bitUSD, etc.

In this proposal, the referral program will receive most of its funds by more advanced operations, such as *proposals*, *withdraw permissions* and *account upgrades*. Also, we propose to implement this new fee schedule for **LTM-only*** for a period of time, and offer it to basic members only later. This way, we effectively upgrade memberships into premium products. As more and more features are added to LTM, we may increase the account upgrading fee accordingly. In this way we encourage power users to upgrade to LTM rather earlier than later. The users who have upgraded to LTM before the fee increases will be happy with that. Occasionally we may offer limited time discounts on account upgrading to advertise new blockchain features. It's also important that some fees may be reduced in the long run to keep us competitive. 

Additionally, going forward with this fee schedule, we will track the **USD denomination** of fees and thus update the schedule if the valuation of BTS changes.


Roadmap
=======

As Soon As Possible
-------------------

* change the flat fee structure to incorporate customer feedback and improve competitiveness and liquidity.
* start implementation of BSIP#10 (if approved)
* start discussions about
  * requiring LTM account status for specific operations (e.g. asset_create)
  * offering a feature to change default split % (referral program/network) of specific operations
* start implementation for distinction of bitasset fees from prediction market fees
* start Implementation of methods to improve liquidity
  * either on protocol level (MAKER, DAC as bitasset provider, ...)
  * improving trading experience (GUI, API)
* elaborate the implementation details and consequences of rate-limited but free transfers throughout the network


As soon as BSIP#10 is approved and ready
----------------------------------------

* upgrade protocol (hard fork) to include BSIP#10
* discuss which committee owned assets should implement BSIP10 and what percentage transfer fees to take


6 months after the last fee schedule change
-------------------------------------------

* obtain input and feedback from businesses taking part in the referral program
* optional minor modifications to the fee schedule


Periodically every 12 months after the last change of the fee schedule
----------------------------------------------------------------------

* re-evaluate revenue of referral program and improve fee schedule given feedback of corresponding businesses and more statistics
* evaluation of revenue and costs of the DAC and the referral program.
* optional changes to the fee schedule

Possible protocol modifications requiring more discussion
---------------------------------------------------------
* distinguish fees for bitassets and prediction markets
* add committee controlled flags to prevent/allow specific operations to be used by basic members or premium members (LTM)
* add committee control over operation-specific fee split between referral program and network
* add period-dependent fee for withdraw_permission_claim
* rate-limited 0-fee transactions


Overview
========

Rationale for changes to the flat fees

  1. The transfer of value (any token) is a core functionality of many crypto currencies and business like dwolla and paypal. In order to be competitive, we need a lower overall cost associated with that operation/transaction. Furthermore, the costs to the network associated with that operation are rather low because only account ids, asset ids and an amount are involved. Optional memo sending can be set to a higher fee. The transfer operation is considered a core functionality of BitShares and uses of it should be incentivized. This way, we can attract more businesses that are looking for micropayment solutions.

  2. Another *core* functionality and major *value proposition* is the decentralized exchange (DEX) which is associated with a different set of fees. Currently, the fees are flat for order creation, cancellation and update, and are independent of the amount actually traded. Hence, small volume orders pay the same fee as large volume orders. Taking a closer look at any competitor reveals that this stands in contrast to the proven business models. Instead of asking for a rather high flat fee to compensate the costs of the DEX (storing and matching orders), We are proposing to reduce the flat fee drastically to an amount will prevent spam, and then set a percentage based trading fee that is levied when an order for any committee-owned asset is filled. The advantages are that the committee (read: DAC) could earn more fees from matching orders. Since cancellation of orders results in a refund of the creation fee, this should also encourage traders to bring liquidity. A disadvantage is that the DAC earns less from trading of assets that are not owned by the committee, such as OPEN.BTC, TRADE.MUSE etc., because the flat fees are reduced and the percentage market fees go to the corresponding issuer. In any case, this approach should result in more traders using the DEX and an increase of liquidity.
 
  What percentage should be used? Since we are using a fixed percentage independent of volume, to be competitive we should choose a percentage that is lower than the highest fee levied by big exchanges such as Kraken, Coinbase, BTC38, etc. Furthermore, regional difference should be taken into account eventually. For now I propose a fee of

                           0.10%

  of the matched volume which is less than most centralized competitors, even though we offer a more secure platform. This fee may be considered as a welcome package and may eventually be increased to something close to 0.5% to reflect the marketable value decentralized and trust-free nature of the DEX.

  3. Now that we have reduced the fees for our two core functionalities, how can we compensate the referral program that pays the registrar/affiliate a fraction of the paid fee from referrers? The transfer and trading fees certainly don't motivate business to bring in more users if they don't get paid!

  The solution is rather simple: The above mentioned transfer and trade operations are only two out of many operations that can be used by customers to make full use of BitShares. There is also the creation of assets and withdrawal permissions as well as worker, committee member creation and proposals. These fees can be used to benefit the referral program.

  As a strategy, we distinguish power users from regular users. Power users should are encouraged to upgrade their account to a lifetime membership (or annual membership) to reduce their fees by 80% (receive cash back). The regular users will use the network less frequently, and are also less likely to  have a need for other functions like the creation of new assets and other more advanced features. If he does, we can ask for a comparably high fee since there are few competitors out there who also offer these features. A power user that wants to see reduced fees and benefit from cheaper advanced features should be asked to pay a higher fee to upgrade his account.

In short: The referral program should only receive minor benefit from the core value proposition (transfers and trades) of the DEX but instead make its profit from the advanced features of the network, such as:

* memberships (for reduced fees)
* individual assets
* withdrawal permissions
* proposals
* prediction market
* among others


Important factors:
------------------

- All flat fees here are basic member fees. For LTM, most fees get cut by 80%

- The flat fees below are denominated in USD, even though the network asks for fees in BTS. This means that the BTS fees have to be adjusted from time to time to follow BTS' volatility. This can be easily achieved through scripting.

- In order to bring stability for investors, businesses, and customers, the flat USD denominated fees should not be changed for an interval of AT LEAST 6 months. Hence, we should find a consensus for a USD denominated fee schedule and stick with it.

- All fees in this document are proposals, and thus are not final. Everything is subject to final approval by the committee, and thus the shareholders.

- If this proposal is accepted, it will revise the 3x transfer price vision for STEALTH transfers to a 7x factor to let the investor(s) reach their ROI at a faster rate. 

- It makes sense to incorporate the opinions and requirements of businesses running on top of BitShares as much as possible. We need them! Hence, we should talk to:

  * OpenLedger
  * metaexchange
  * bitcash
  * transwiser
  * freebie
  * bunkerchainlabs
  * peermit
  * blocktrades.us
  * BitShares POS
  * OnceUponATime (STEALTH)
  * Others who come forward

Centralized exchanges are not part of this list since they mainly benefit from reduced transfer fees and don't run a business *within* BitShares (i.e. no referral program, no use of special blockchain capabilities)


Conclusion:
===========

The proposal above as well as the flat fees below try to find a balance between cheaper transfers and improving the liquidity of the DEX while still allowing marketers to benefit from the referral program. This is achieved by reducing the flat fees of the core transfer and trading operations, adding a percentage based market fee and increasing the fees associated with operations that are unique to BitShares. In order to attract people to the DEX, we need to be competing with centralized exchanges in terms of fees, and then once people migrate to our platform in sufficient numbers, we have the eventual option to raise fees slightly. 


High Level Overview of changes:
-------------------------------

The scripts used to track the USD fee are [publicly
auditable](https://github.com/BitShares-Committee/Instructions/tree/master/usd-denominated-fees).
A detailed descriptipon about every single operation and it's associated
fee is available under
[github](https://github.com/BitShares-Committee/Instructions/blob/master/usd-denominated-fees/fee-schedule-proposed-by-xeroc.py).

### Fee Types:

* `fee` is a flat price that has to be paid per operation
* `price_per_kbyte` is a fee that has to be paid per kilobyte of transaction size
  (i.e. longer memos cost more than shorter memos)
* `account_create` distinguishes `premium_fee` names (expensive) from `basic_fee`
  names (cheap)
* `account_upgrade` distinguishes between a annual subscription and a life time
  subscription
* `asset_create` distinguishes between the number of characters of the symbol (i.e.
  short symbols are very expensive, longer ones are cheap)
* blind transfers have to pay per output.

```
        price_per_kbyte price for                                  transfer differs by    0.133x (network:    0.0754 USD / proposal:    0.0100 USD)
                    fee price for                                  transfer differs by    0.159x (network:    0.1132 USD / proposal:    0.0180 USD)
                    fee price for                        limit_order_create differs by    0.027x (network:    0.0377 USD / proposal:    0.0010 USD)
                    fee price for                        limit_order_cancel differs by  999.000x (network:    0.0000 USD / proposal:    0.0001 USD)
                    fee price for                         call_order_update differs by    0.265x (network:    0.0038 USD / proposal:    0.0010 USD)
        price_per_kbyte price for                            account_create differs by    0.928x (network:    0.0075 USD / proposal:    0.0070 USD)
              basic_fee price for                            account_create differs by    0.279x (network:    0.3583 USD / proposal:    0.1000 USD)
            premium_fee price for                            account_create differs by    0.331x (network:   15.0868 USD / proposal:    5.0000 USD)
        price_per_kbyte price for                            account_update differs by    0.928x (network:    0.0075 USD / proposal:    0.0070 USD)
                    fee price for                            account_update differs by    0.265x (network:    0.0038 USD / proposal:    0.0010 USD)
                    fee price for                         account_whitelist differs by    4.419x (network:    0.0226 USD / proposal:    0.1000 USD)
membership_lifetime_fee price for                           account_upgrade differs by    1.591x (network:   75.4340 USD / proposal:  120.0000 USD)
  membership_annual_fee price for                           account_upgrade differs by    0.994x (network:   15.0868 USD / proposal:   15.0000 USD)
                    fee price for                          account_transfer differs by    1.326x (network:    3.7717 USD / proposal:    5.0000 USD)
                symbol4 price for                              asset_create differs by    2.039x (network:  980.6426 USD / proposal: 2000.0000 USD)
        price_per_kbyte price for                              asset_create differs by    1.326x (network:    0.0075 USD / proposal:    0.0100 USD)
                symbol3 price for                              asset_create differs by    2.121x (network: 3771.7025 USD / proposal: 8000.0000 USD)
            long_symbol price for                              asset_create differs by    2.651x (network:   18.8585 USD / proposal:   50.0000 USD)
        price_per_kbyte price for                              asset_update differs by    0.928x (network:    0.0075 USD / proposal:    0.0070 USD)
                    fee price for                              asset_update differs by   26.513x (network:    0.0754 USD / proposal:    2.0000 USD)
                    fee price for                     asset_update_bitasset differs by    1.326x (network:    3.7717 USD / proposal:    5.0000 USD)
                    fee price for               asset_update_feed_producers differs by    1.326x (network:    3.7717 USD / proposal:    5.0000 USD)
        price_per_kbyte price for                               asset_issue differs by    0.928x (network:    0.0075 USD / proposal:    0.0070 USD)
                    fee price for                               asset_issue differs by    6.628x (network:    0.1509 USD / proposal:    1.0000 USD)
                    fee price for                             asset_reserve differs by    6.628x (network:    0.1509 USD / proposal:    1.0000 USD)
                    fee price for                       asset_fund_fee_pool differs by   66.283x (network:    0.0075 USD / proposal:    0.5000 USD)
                    fee price for                              asset_settle differs by    0.066x (network:    0.7543 USD / proposal:    0.0500 USD)
                    fee price for                       asset_global_settle differs by    1.326x (network:    3.7717 USD / proposal:    5.0000 USD)
                    fee price for                        asset_publish_feed differs by  999.000x (network:    0.0000 USD / proposal:    0.0001 USD)
                    fee price for                            witness_create differs by    1.326x (network:   37.7170 USD / proposal:   50.0000 USD)
                    fee price for                            witness_update differs by    0.066x (network:    0.1509 USD / proposal:    0.0100 USD)
        price_per_kbyte price for                           proposal_create differs by    6.628x (network:    0.0075 USD / proposal:    0.0500 USD)
                    fee price for                           proposal_create differs by    0.994x (network:    0.1509 USD / proposal:    0.1500 USD)
        price_per_kbyte price for                           proposal_update differs by    0.928x (network:    0.0075 USD / proposal:    0.0070 USD)
                    fee price for                           proposal_update differs by    0.663x (network:    0.0075 USD / proposal:    0.0050 USD)
                    fee price for                           proposal_delete differs by    0.000x (network:    0.0075 USD / proposal:    0.0000 USD)
                    fee price for                withdraw_permission_create differs by   19.885x (network:    0.0075 USD / proposal:    0.1500 USD)
                    fee price for                withdraw_permission_update differs by    0.066x (network:    0.1509 USD / proposal:    0.0100 USD)
        price_per_kbyte price for                 withdraw_permission_claim differs by    0.928x (network:    0.0075 USD / proposal:    0.0070 USD)
                    fee price for                 withdraw_permission_claim differs by  999.000x (network:    0.0000 USD / proposal:    0.0144 USD)
                    fee price for                withdraw_permission_delete differs by    0.000x (network:   37.7170 USD / proposal:    0.0000 USD)
                    fee price for                   committee_member_create differs by  662.831x (network:    0.0075 USD / proposal:    5.0000 USD)
                    fee price for                   committee_member_update differs by 1325.661x (network:    0.0075 USD / proposal:   10.0000 USD)
                    fee price for committee_member_update_global_parameters differs by    0.066x (network:    0.1509 USD / proposal:    0.0100 USD)
                    fee price for                    vesting_balance_create differs by    0.133x (network:   37.7170 USD / proposal:    5.0000 USD)
                    fee price for                  vesting_balance_withdraw differs by  265.132x (network:    0.0075 USD / proposal:    2.0000 USD)
                    fee price for                             worker_create differs by  662.831x (network:    0.0075 USD / proposal:    5.0000 USD)
        price_per_kbyte price for                                    custom differs by    1.326x (network:    0.0075 USD / proposal:    0.0100 USD)
                    fee price for                                    custom differs by   13.257x (network:    0.0075 USD / proposal:    0.1000 USD)
                    fee price for                                    assert differs by   66.283x (network:    0.1509 USD / proposal:   10.0000 USD)
        price_per_kbyte price for                         override_transfer differs by    0.928x (network:    0.0075 USD / proposal:    0.0070 USD)
                    fee price for                         override_transfer differs by   26.513x (network:    0.0377 USD / proposal:    1.0000 USD)
       price_per_output price for                         transfer_to_blind differs by    0.928x (network:    0.0754 USD / proposal:    0.0700 USD)
                    fee price for                         transfer_to_blind differs by    2.784x (network:    0.0754 USD / proposal:    0.2100 USD)
                    fee price for                       transfer_from_blind differs by    2.784x (network:    0.0754 USD / proposal:    0.2100 USD)
```
