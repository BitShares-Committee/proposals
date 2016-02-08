Shareholder Summary
===================

Thanks to some keen external developers we are soon to see what is referred to as BSIP#10
and will allow percentage based transfer fees and give the BitShares ecosystem some needed
flexibility to distinguish between different cultures. Another idea that came up recently,
was the limitation of transfers by rate and offering it for free to get an unfair
advantage over other crypto currencies and ecosystem while still having ways to monetize
by other operations, such as trading. However, the development is quite intensive and will
take some more weeks to complete.

To resolve the highly discussed fee issue of many shareholders, the BitShares community
and most of the existing businesses, the committee has decided to step up and act now with
the option for modifications once BSIP#10 is available.

After several days of intensive discussion, we've constructed a whole new fee schedule for
the BitShares ecosystem that has **drastically reduces** the fees required for the **core
features**, namely, *transfers* and *trading*, but increases the fees of more specialized
operations. By this, we keep the referral program attractive and can attract more
customers as we become more competitive with other service providers for these features,
but have them at one place.

Even though this fee schedule has had a lot of thoughts, we we will have more options once
BSIP#10 or the rate-limited free transfer is available to be implemented for bitassets
owned by the committee. In the mean time, however, we would like to give everyone the
opportunity to make use of a low flat fee for all transfers with in the network and have
decided to ask for $0.018 (less than 6 BTS at current valuation) per transfer! Keep in
mind that this will be a **limited-time offer** and the minimum fee may be raised once
BSIP#10 is implemented.

We would further like to encourage traders and market makers to provide liquidity by
asking for only $0.001 per created order (with 90% refund on cancelation if unfilled) and
a low 0.10% trading fee for committee owned assets such as bitUSD, etc.

In this proposal, the referral program will receive most of its funds by more advanced
operations, such as *proposals*, *withdraw permissions* as well as *account upgrades*. The
committee will keep the option to change old (non basic) features and implement new
features for **LTM-only** for a period of time and offer it to basic members only later.
This way, we effectivley, upgrade memberships into premium products.

Additionally, going forward with this fee schedule, we will track the **USD denomination**
of fees and thus update the schedule if the valuation of BTS changes.

Roadmap
=======

As Soon As Possible
-------------------

* change the flat fee strucutre to incorporate customer feedback
  and improve competitiveness and liquidity.
* start implementation of BSIP#10 (if approved)
* start discussions about
  * requiring LTM-ship for specific operations (e.g. asset_create)
  * removing of specific operations from Referral program (e.g. account_upgrade)
* start Implementation for distiction of bitasset fees from prediction
  market fees
* start Implemenation of methods to improve liquidity
  * either on protocol level (MAKER, DAC as bitasset provider, ...)
  * improving trading experience (GUI, API)
* elaborate the implementation details and consequences of rate-limited but free
  transfers throughout the network

As soon as BSIP#10 is approved and ready
----------------------------------------

* upgrade protocol (hard fork) to include BSIP#10
* modify committee owned assets to ask for percentage transfer fees
* start discussion about possible protocol modifications:
  * protocol upgrade to distinguish fees for bitassets and prediction markets
  * add committee controlled flags to prevent/allow specific operations
    to be used by basic members but allowed for premium members (LTM)
  * add committee controlled flags to include/exclude specific
    operations from the referral program
  * add period-dependent fee for withdraw_permission_claim

6 months after the last fee schedule change
-------------------------------------------

* obtain input and feedback from businesses taking part in the referral program
* optional minor modifications to the fee schedule

Periodically every 12 months after the last change of the fee schedule
----------------------------------------------------------------------

* re-evaluate revenue of referral program and improve fee schedule given
  feedback of corresponding businesses and more statistics
* evaluation of revenue and costs of the DAC and the referral program.
* optional changes to the fee schedule

Overview
========

Rational for changes to the flat fees now

1. The transfer of value (any token) is a core functionality of many crypto
   currencies and business like dwolla and paypal. In order to be competitive,
   we need a lower over all cost associated with that operation/transaction.
   Furthermore, the costs associated with that operation are rather low because
   only account ids, asset ids and an amount are involved. Optional memos can be
   set a higher fee. The transfer operation is considered a *core* functionality
   of BitShares and its used should be incentivized. This way, we can
   even attract more businesses that are looking for micropayment
   solutions.

2. Another *core* functionality and major *value proposition* is the
   decentralized exchange (DEX) which is associated with a different set of feed.
   Currently, the fees are flat fees for order creation, cancellation and update,
   and are independent of the amount actually traded. Hence, small volume orders
   pay the same fee as large volume orders. Taking a closer look at any
   competitor reveals that this should certainly chance. Instead of asking for a
   rather high flat fee to compensate the costs of the DEX (storing and matching
   orders), I here propose to reduce the flat fee drastically to an amount that
   mostly to prevents spam and instead set a percentage trading fee for every
   committee-owned asset. The advantages are that the committee (read: DAC) could
   earn more fees from matching orders. Since cancellation of orders results in a
   refund of the creation fee, this should also encourage traders to bring
   liquidity. A disadvantage is that the DAC earns less from trading of assets
   that are not owned by the committee, such as OPEN.BTC, TRADE.MUSE etc. because
   the flat fees are reduced and the percentage market fees go to the
   corresponding issuer. Anyway, this approach should result in more traders
   using the DEX and an increase of liquidity.

   What percentage should be used? Since we are using a fixed percentage
   independent of an individuals volume, we should choose a percentage that is
   lower than the highest fee asked for by big exchanges such as Kraken,
   Coinbase, BTC38, etc. Furthermore, regional difference should be
   taken into account eventually. For now I propose a fee of

                           0.10%

   of the matched volume which is less than most centralized competitors even
   though we offer an increased security over them. This fee may be considered as
   a welcome package and may probably be increased to something close to 0.5% to
   reflect the decentralized and trust-free nature of the DEX.

3. Now that we have reduced the fees for our two core functionalities, how can we
   rescue the referral program that pays the registrar/affiliate a fraction of
   the payed fee from referrers? The transfer and trading fees certainly don't
   motive business to bring in more users if they don't get paid!

   The solution is rather simple: The above mentioned transfer and trade
   operations are only two out of many operations that can be used by customers
   to make full use of BitShares. There is also the creation of assets,
   withdrawal permissions as well as worker, committee member creation and
   proposals. These fees can be used to let the referral program benefit from
   customers.

   So, we distinguish power users from regular users. Power users should be
   encouraged to upgrade their account to a life-time membership (or annual
   membership) to reduce their fees by 80% (receive cashback). The regular users
   rarely creates new assets and uses it frequently, as well as use more advanced
   features of the network, but if he does, we can ask for a comparably high fee
   since there are only few competitors with these functionalities, if at all.
   A power users that wants to see constantly reduced fees and benefit from
   cheaper advanced features should be asked to pay a higher fee to upgrade his
   account.

In short: The referral program should only receive minor benefit from the core
value proposition (transfers and trades) of the DEX but instead make
its profit from the advanced features of the network, such as:

* memberships for reduced fees
* individual assets
* withdrawal permissions
* proposals
* prediction market
* among others

Important factors:
------------------

- All flat fees here are basic member fees. For LTM, most fees get cur
  by 80%

- The flat fees below are denoted in USD even though the network asks for fees
  in BTS. This means that the BTS fees have to be adjusted from time to time
  to follow BTS' volatility. This can be achieved by scripting easily.

- In order to show stability to investors, businesses, and customers, the flat
  USD denoted fees should not be changed for an interval of AT LEAST 6 months.
  Hence, we should find a consensus for a USD-denoted fee schedule and
  stick with it.

- All fees in this document are proposals, ands thus not final. They further
  require committee's approval.

- Shall this proposal be accepted, it will revise the 3x transfer
  price vision for STEALTH transfers to a 7x factor to let the
  investor(s) reach their ROI as has been initially promised.

- It makes sense to incorporate the opinions and requirements of businesses
  running on top of BitShares as far as possible. We need them! Hence, we should
  talk to:

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

  Centralized exchanges are not part of this list since they mainly benefit from
  reduced transfer fees and don't run a business *whithin* BitShares (i.e. no
  referral program, no use of special blockchain capabilities)

Conclusion:
===========

The proposal above as well as the flat fees below try to find a balance
between cheaper transfers and improving the liquidity of the DEX while still
having marketers benefit from the referral program. This is achieved by
reducing the flat fees of the core transfer and trading operations, adding a
percentage market fee and increasing the fees associated with operations that
are special to BitShares alone and have only fee competitors. In order to
attract people to the DEX, we need to be competing with centralized exchanges
in terms of fees in the beginning and once people realize the power of
decentralized trading, the fees could potentially be raised slightly.

High Level Overview of changes:
-------------------------------

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
