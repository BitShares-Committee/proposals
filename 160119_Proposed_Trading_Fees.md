Proposed by clayop

#Current Problems: 

Order creation fee can be regarded as an additional fee on top of percentage based trading fee (market fees). Although the current network income from order creation fee is very small ($60/month), it can be a serious barrier against active traders or potential business owners (e.g. Metaexchange, https://bitsharestalk.org/index.php/topic,21060.0.html ).

The ideal role of order creation fee is preventing spam attacks without making any negative impacts on trading activities and businesses. The present fee system (10 BTS for order creation / 0 BTS for cancellation / full refund for cancellation of non-filled order) is very strong against the attack by filling witness servers' memory, more specifically, an attacker requires $400,000 to completely consume the server's memory (4 GB) in 7 days (under 100 TPS). (see https://bitsharestalk.org/index.php/topic,19890.msg255704.html#msg255704 ).

However, it may discourage traders, especially when they compare BitShare's current trading fee system with external trading fee system, which only charges percentage based fee for filled orders and no order creation fee.
In addition, the current fee system has no way to prevent flooding attack because the cancellation fee is free in combination of full refund.

Given these problems, we need to restructure the trading fee system, balancing in between spam prevention and encouraging traders and business runners.

#Suggestions:

(normal / lifetime member)

- Limit order create: 1 / 0.2 BTS

  Spammers(LTM) need $40,000 to fill witnesses' memory. But this takes seven days. When we detect the attack, committee members can quickly increase order creation fee.

- Limit order cancel: 0.05 / 0.01 BTS

  It's for preventing flooding attacks. Attacker need 1 BTS (0.01*100) per second to flood network (under 100 TPS)

- Call order update: 1 / 0.2 BTS

  No change

- Fill order: 0 / 0 BTS

  No change

- Market fee on Smartcoins and BTS: 0.1%

  Reducing order creation fee surely induce reduced network profit. To compensate network income, we can charge market fees on Smartcoins and BTS.

  I expect that there will be some backlash from traders, because the current market fee is free. But with decreased order creation fee, orders under 11,000 BTS will pay less. Surely the 0.1% rate is lower than other exchanges on average. (They usually charge over 0.2%)


#Expected Outcomes:

Unortunately, we cannot expect immediate ten-times market activities compared to ten times less order creation fee. However, the restructured fee system can encourage more trading activity and attract more businesses that will bring more users. Consequently, BitShares ecosystem will be expanded.
