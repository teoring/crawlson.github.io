
# What is Crawlson?

Crawlson monitors popular real estate aggregators and agencies and notifies users about new houses according to their preferences. 

It takes Crawlson only 6 minutes to visit over 40 different web-sites of makelaars and aggregators and to notify you about new houses on the market immediately. You would be among the first-one`s to see it online.

## Where to start?
It is important to configure your preferences correctly. If you skip this step you might receive irrelevant notifications.

All settings can be changed in Crawlson telegram channel chat.

 To view your current settings type:
> /settings

To see a list of available commands type:
>/help

Note: In certain cases Crawlson still might decide to send you house notification even if it doesn't match the setting. That's because it is now always possible for Crawlson to determine certain house parameters from the house page.

## Available settings overview
Following filters can be set to refine house notifications you are receiving:

- Minimum house price ( euros )
- Maximum house price ( euros )
- Minimum construction year ( year )
- Cities where you look for house ( comma separated list of cities )
- Minimum living area in the house ( m² )
- The area where you want to buy house ( based on the address )
	- The area is set with the address, we call it a travel address
	- You can configure the Crawlson to search for house that is no more than X minutes from the travel address by walking, bicycling, riding or public transport ( based on Google Map calculations )
	- You can configure the Crawlson to search for house that is within X kilometers radius from the travel address

## Changing settings

### Changing maximum price
To change maximum house price use **/setmaxprice** command.  The price is a number with no comma's or dot's. For example:
>/setmaxprice 500000

Sets maximum house price to 500 k.k. euros.
<br/>

### Changing minimum price
To change minimum house price use **/setminprice** command.  For example:
>/setminprice 500000

Sets minimumm house price to 500 k.k. euros.
<br/>


### Changing the minimum construction year

To change minimum construction year use **/setminconstryear** command.  For example:
>/setminconstryear 1990

Sets minimum construction year to 1990.
<br/>

### Changing cities 

To change cities filter use **/setcities** command. For example:
>/setcities Eindhoven, Helmond, Veghel

Note: new value will overwrite previous value so you need to type a full and complete list of cities.
<br/>


### Changing minimum living area plot size

To change minimum living area plot size  use **/setminlivingarea** command.  The value is in square meters. For example:
>/setminlivingarea 110

Sets minimum living area to 110 square meters.
<br/>

### Configuring location preferences
The travel address setting enables you to find house in a very specific location within any city. For example, it can allow you to search for house that is no more than 20 minutes walking distance from the central station, or to search for house that is no more than 10 kilometers away from the international school.

You can set only one travel address and **this setting will only work if you configure travel address, travel time or travel distance and commute mode**.

Below, you can find step by step instruction how to setup this setting correctly.
<br/>

#### Step #1 | Setting Travel Address
To set a travel address use **/settraveladdress** command where the value is the full address, for example:
>/settraveladdress Eindhoven Centraal, 5612 AZ Eindhoven

Once the address is set, its time to define the distance and/or the travel time settings.
<br/>

#### Step #2 | Setting Commute Mode
Set how do you commute. It used to measure the maximum commute time from the house to the travel address. 

It accepts following values: driving,  walking, bicycling, transit. Transit is public transportation.

To set commute mode use **/setcommutemode** command, for example:
> /setcommutemode driving

Would set commute type to driving.
<br/>

#### Step #3 | Set maximum commute time or maximum distance
You can decide to set both or one of the following filters:
- Maximum time needed to reach the house from travel address using selected commute mode
- Maximum distance from the travel address to the house using commute mode
<br/>

##### Maximum Travel time
To set maximum travel time use **/setmaxtraveltime** command. The value is in minutes. Note that this travel time is based on commute mode you've selected. This an example of how you can configure this value:
> /setmaxtraveltime 60

It  would set maximum travel time to 60  minutes. 
<br/>
##### Maximum Travel distance
To set maximum travel distance use **/setmaxdistance** command. The value is in kilometers. Note that the distance is calculated based on selected commute mode. For example, for commute mode 'driving' - distance will be a car road length. If you want to have pure radius distance, configure commute mode to 'walking'.

This an example how to configure this setting:
> /setmaxdistance 10

It would set maximum travel distance to 10 kilometers.
<br/>
Note: You can define both distance and time settings at the same time. In that case you will receive notification only if both conditions are satisfied.


# What sources Crawlson monitors?
Crawlson monitors following sources: [funda.nl](https://funda.nl/ "https://funda.nl"), [pararius.nl](https://pararius.nl/ "https://pararius.nl"), [vbo.nl](https://vbo.nl/ "https://vbo.nl"), [jaap.nl](https://jaap.nl/ "https://jaap.nl"), [huislijn.nl](https://huislijn.nl/ "https://huislijn.nl"), [maasmakelaars.nl](https://maasmakelaars.nl/ "https://maasmakelaars.nl"), [hypodomus-eindhoven.nl](https://hypodomus-eindhoven.nl/ "https://hypodomus-eindhoven.nl"), [hendriks.nl](https://hendriks.nl/ "https://hendriks.nl"), [vanuffelen.nl](https://vanuffelen.nl/ "https://vanuffelen.nl"), [vbtmakelaars.nl](https://vbtmakelaars.nl/ "https://vbtmakelaars.nl"), [alberti.nl](https://alberti.nl/ "https://alberti.nl"), [raadhage.nl](https://raadhage.nl/ "https://raadhage.nl"), [dpmrobvandelaar.nl](https://dpmrobvandelaar.nl/ "https://dpmrobvandelaar.nl"), [woonplezier.nl](https://woonplezier.nl/ "https://woonplezier.nl"), [makelaardevree.nl](https://makelaardevree.nl/ "https://makelaardevree.nl"), [heuvel.nl](https://heuvel.nl/ "https://heuvel.nl"), [kinmakelaars.nl](https://kinmakelaars.nl/ "https://kinmakelaars.nl"), [kranenmakelaardij.nl](https://kranenmakelaardij.nl/ "https://kranenmakelaardij.nl"), [erafocus.nl](https://erafocus.nl/ "https://erafocus.nl"), [huibers.nl](https://huibers.nl/ "https://huibers.nl"), [vansantvoort.nl](https://vansantvoort.nl/ "https://vansantvoort.nl"), [slippensvermeer.nl](https://slippensvermeer.nl/ "https://slippensvermeer.nl"), [hendrixhuybregts.nl](https://hendrixhuybregts.nl/ "https://hendrixhuybregts.nl"), [mgmmakelaardij.nl](https://mgmmakelaardij.nl/ "https://mgmmakelaardij.nl"), [edwillems.nl](https://edwillems.nl/ "https://edwillems.nl"), [ligtvoetmakelaardij.nl](https://ligtvoetmakelaardij.nl/ "https://ligtvoetmakelaardij.nl"), [metselaarsmakelaardij.nl](https://metselaarsmakelaardij.nl/ "https://metselaarsmakelaardij.nl"), [dekoningmakelaardij.nl](https://dekoningmakelaardij.nl/ "https://dekoningmakelaardij.nl"), [makelaardijolav.nl](https://makelaardijolav.nl/ "https://makelaardijolav.nl"), [kernmakelaars.nl](https://kernmakelaars.nl/ "https://kernmakelaars.nl"), [hartvanbrabantmakelaardij.nl](https://hartvanbrabantmakelaardij.nl/ "https://hartvanbrabantmakelaardij.nl"), [lemmens.nl](https://lemmens.nl/ "https://lemmens.nl"), [huispedia.nl](https://huispedia.nl/ "https://huispedia.nl"), [hansvanberkel.nl](https://hansvanberkel.nl/ "https://hansvanberkel.nl"), [vmg-makelaars.nl](https://vmg-makelaars.nl/ "https://vmg-makelaars.nl"), [broekx.nl](https://broekx.nl/ "https://broekx.nl"), [era.nl](https://era.nl/ "https://era.nl").

