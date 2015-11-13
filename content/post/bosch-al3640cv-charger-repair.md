---
type: post
title: "Repairing a Bosch AL-3640-CV Charger"
date: "2015-11-13T22:34:44+00:00"
published: true
comments: true
categories: [Repair, Electronics]
facebook:
    image: http://galooph.com/images/bosch-al3640cv-charger.jpg
twitter_card:
    creator: galooph
    image: http://galooph.com/images/bosch-al3640cv-charger.jpg
---
My brother has got a Bosch cordless lawnmower that uses 36V battery packs. He presented me with the charger, which was completely dead – no LEDs lit at all when plugged in, and nothing on the output terminals. Checking the circuit board, there was nothing visibly wrong, so it was time to hit Google.

I found an <a href="http://www.elektroda.pl/rtvforum/topic1001850.html">old post on a Polish forum</a> that suggested that a 180k‎&#8486; resistor fails. The resistor looked fine, but after desoldering it, it measured open circuit. It looks as though this is the startup resistor for the switch mode supply. The original resistor was rated around 1W at a guess, so I replaced it with a 3W version.

{{< figure src="/images/bosch-al3640cv-180k.jpg" >}}

**Note: Only poke around in the charger internals if you're confident in your ability to do so! The big capacitor in there is 150&micro;F at 400V and will bite if you don't discharge it safely. I accept no responsibilty if you break your charger or hurt yourself, so there!**

<!-- more -->

While I was checking over the rest of the circuit board, I noticed a pair of 2k2&#8486; resistors that obviously get fairly warm, so I replaced those too.

{{< figure src="/images/bosch-al3640cv-2k2.jpg" >}}

After reassembling everything, it was time to power the charger up. Always fun with offline switch mode supplies, as they can go with a bang. Takes me back to fitting PSU repair kits to Amstrad satellite receivers! I flicked the mains on, and was greeted by a green LED lighting up on the charger. 

{{< figure src="/images/bosch-al3640cv-charger.jpg" >}}

My brother has since tested the charger on a battery and it works fine.
