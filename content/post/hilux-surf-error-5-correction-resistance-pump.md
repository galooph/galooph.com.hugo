---
type: post
title: "Hilux Surf: Error 5 - Correction resistance (Pump)"
date: "2014-01-11"
comments: true
categories: [Hilux Surf, Truck]
facebook:
    image: http://galooph.com/images/InjectorPumpPicture.jpg
twitter_card:
    creator: galooph
    image: http://galooph.com/images/InjectorPumpPicture.jpg
---
Error code 5 relates to a pair of resistors on the side of the injection pump, at least on the 2.4TD engine.

{{< figure src="/images/InjectorPumpPicture.jpg" >}}

These resistors are installed when the pump is calibrated and fine tune the timing and fuelling.

<!-- more -->

{{< figure src="/images/grey_ip_resistor.jpg" class="half-width" >}}
{{< figure src="/images/beige_ip_resistor.jpg" class="half-width" >}}


I measured both resistors. The grey one was 0.622kΩ while the beige one was open circuit. The insides are potted in epoxy, so I dug out the trusty Dremel and went in.

{{< figure src="/images/grey_ip_resistor_epoxy.jpg" title="The original epoxy." >}}

{{< figure src="/images/beige_ip_resistor_post_dremel.jpg" title="After a bit of Dremel action." >}}

You can see a pair of solder tabs sticking up - the original resistor, which I ground away, was soldered on here. Judging from the resistor body, it was no more than a standard 0.25W resistor.

The problem now was knowing what value the resistor was originally.

I managed to find a [scan of the manual](https://picasaweb.google.com/toddmcclendon/DensoPump?feat=directlink#) for the Denso injector pump. I've also [converted it into a pdf](/assets/surf_ip_manual.pdf).

From that, I was able to work out the resistance value from the part numbers. Here's a list linking to the resistors which are available from Farnell. First, the grey one.

{{< figure src="/images/grey_ip_resistor_part_no.jpg" >}}

Code|Resistance
---|--------------------------------------------------------------------------------------------------------
001|[0.243kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8243rbya/resistor-0-25w-0-1-243r/dp/1751378)
002|[0.267kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8267rbya/resistor-0-25w-0-1-267r/dp/1751382)
003|[0.294kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8294rbya/resistor-0-25w-0-1-294r/dp/1751387)
004|[0.316kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8316rbya/resistor-0-25w-0-1-316r/dp/1751390)
005|[0.348kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8348rbya/resistor-0-25w-0-1-348r/dp/1751394)
006|[0.384kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8383rbya/resistor-0-25w-0-1-383r/dp/1751399)
007|[0.412kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8412rbya/resistor-0-25w-0-1-412r/dp/1751403)
008|[0.453kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8453rbya/resistor-0-25w-0-1-453r/dp/1751407)
009|[0.487kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8487rbya/resistor-0-25w-0-1-487r/dp/1751410)
010|[0.523kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8523rbya/resistor-0-25w-0-1-523r/dp/1751413)
011|[0.576kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8576rbya/resistor-0-25w-0-1-576r/dp/1751418)
012|[0.619kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8619rbya/resistor-0-25w-0-1-619r/dp/1751421)
013|[0.681kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8681rbya/resistor-0-25w-0-1-681r/dp/1751425)
014|[0.732kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8732rbya/resistor-0-25w-0-1-732r/dp/1751429)
015|[0.787kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8787rbya/resistor-0-25w-0-1-787r/dp/1751432)
016|[0.866kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8866rbya/resistor-0-25w-0-1-866r/dp/1751436)
017|[0.931kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8931rbya/resistor-0-25w-0-1-931r/dp/1751441)
018|[1.020kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h81k02bya/resistor-0-25w-0-1-1k02/dp/1751445)
019|[1.100kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h81k1bya/resistor-0-25w-0-1-1k1/dp/1751448)  
020|[1.210kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h81k21bya/resistor-0-25w-0-1-1k21/dp/1751453)
021|[1.330kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h81k33bya/resistor-0-25w-0-1-1k33/dp/1751457)
022|[1.430kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h81k43bya/resistor-0-25w-0-1-1k43/dp/1751460)
023|[0.068kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h868r1bya/resistor-0-25w-0-1-68r1/dp/1751308)
025|[0.100kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8100rbya/resistor-0-25w-0-1-100r/dp/1751317)
026|[0.121kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8121rbya/resistor-0-25w-0-1-121r/dp/1751326)
027|[0.133kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8133kbya/resistor-0-25w-0-1-133k/dp/1751672)
028|[0.154kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8154rbya/resistor-0-25w-0-1-154r/dp/1751337)
029|[0.174kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8174rbya/resistor-0-25w-0-1-174r/dp/1751343)
030|[0.196kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8196rbya/resistor-0-25w-0-1-196r/dp/1751361)
031|[0.221kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8221rbya/resistor-0-25w-0-1-221r/dp/1751374)

Now the beige one.

{{< figure src="/images/beige_ip_resistor_part_no.jpg" >}}

Code|Resistance
---|--------------------------------------------------------------------------------------------------------
001|[0.154kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8154rbya/resistor-0-25w-0-1-154r/dp/1751337)
002|[0.174kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8174rbya/resistor-0-25w-0-1-174r/dp/1751343)
003|[0.196kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8196rbya/resistor-0-25w-0-1-196r/dp/1751361)
004|[0.221kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8221rbya/resistor-0-25w-0-1-221r/dp/1751374)
005|[0.243kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8243rbya/resistor-0-25w-0-1-243r/dp/1751378)
006|[0.267kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8267rbya/resistor-0-25w-0-1-267r/dp/1751382)
007|[0.294kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8294rbya/resistor-0-25w-0-1-294r/dp/1751387)
008|[0.316kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8316rbya/resistor-0-25w-0-1-316r/dp/1751390)
009|[0.348kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8348rbya/resistor-0-25w-0-1-348r/dp/1751394)
010|[0.383kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8383rbya/resistor-0-25w-0-1-383r/dp/1751399)
011|[0.412kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8412rbya/resistor-0-25w-0-1-412r/dp/1751403)
012|[0.453kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8453rbya/resistor-0-25w-0-1-453r/dp/1751407)
013|[0.487kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8487rbya/resistor-0-25w-0-1-487r/dp/1751410)
014|[0.523kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8523rbya/resistor-0-25w-0-1-523r/dp/1751413)
015|[0.576kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8576rbya/resistor-0-25w-0-1-576r/dp/1751418)
016|[0.619kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8619rbya/resistor-0-25w-0-1-619r/dp/1751421)
017|[0.681kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8681rbya/resistor-0-25w-0-1-681r/dp/1751425)
018|[0.732kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8732rbya/resistor-0-25w-0-1-732r/dp/1751429)
019|[0.782kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8787rbya/resistor-0-25w-0-1-787r/dp/1751432)
020|[0.866kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8866rbya/resistor-0-25w-0-1-866r/dp/1751436)
021|[0.931kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h8931rbya/resistor-0-25w-0-1-931r/dp/1751441)
022|[1.020kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h81k02bya/resistor-0-25w-0-1-1k02/dp/1751445)
023|[1.100kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h81k1bya/resistor-0-25w-0-1-1k1/dp/1751448)
024|[1.210kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h81k21bya/resistor-0-25w-0-1-1k21/dp/1751453)
025|[1.330kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h81k33bya/resistor-0-25w-0-1-1k33/dp/1751457)
026|[1.430kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h81k43bya/resistor-0-25w-0-1-1k43/dp/1751460)
027|[1.580kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h81k58bya/resistor-0-25w-0-1-1k58/dp/1751465)
028|[1.780kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h81k78bya/resistor-0-25w-0-1-1k78/dp/1751470)
029|[1.960kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h81k96bya/resistor-0-25w-0-1-1k96/dp/1751474)
030|[2.210kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h82k21bya/resistor-0-25w-0-1-2k21/dp/1751480)
031|[2.490kΩ](http://uk.farnell.com/te-connectivity-holsworthy/h82k49bya/resistor-0-25w-0-1-2k49/dp/1751485)

Solder the appropriate resistors in.

{{< figure src="/images/ip_resistors_soldered.jpg" >}}

Now they need sealing from the elements. Check they read ok on a multimeter first though! After a good clean in some isopropyl alcohol, I used some [Sugru](http://sugru.com/) to seal them up.

{{< figure src="/images/ip_resistors_sugru.jpg" >}}

Instead of Sugru, you could use some proper potting compound or even some mastic, but ONLY neutral cure mastic. If the mastic smells of vinegar, don't use it! The acetic acid released as it cures will eat into the resistor wires.

After all that, I reset the ECU and the code 5 had been eliminated.