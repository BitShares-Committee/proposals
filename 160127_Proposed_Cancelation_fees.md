Increase of Cancelation Fees
============================

This proposal is supposed to remove an attack vector that allows to spam
the network for free by placing orders and canceling them if they are
not filled (partially or completely).

Details
-------

The reason for this attack vector has been identified and is caused by
the recent protocol upgrates that allow market makers and liquidity
providers to reclaim their transaction fee from the order creation
operation. The motivation for this update was to incentivize market
making and improve liquidity.

Solutions
---------

To close this attack vector, we apply a slight cancelation fee.

Proposals
---------

Three proposals have been created:

* `1.10.68`: Cancelation fee: 1 BTS
* `1.10.69`: Cancelation fee: 0.1 BTS
* `1.10.70`: Cancelation fee: 0.01 BTS

The committee members are asked to at least approve `1.10.70` and
**also** approve others in increasing fee order if they want a higher
cancelation fee.

This procedure has been chosen to make sure that the attack vector is
closed and still have a means to allow discussion and disagreements
within the committee.

The proposals have been created by `xeroc` with a [python
script](https://raw.githubusercontent.com/BitShares-Committee/Instructions/master/increase_order_cancelation_fee.py).
