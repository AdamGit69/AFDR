# AFDR
Australian Fire Danger Ratings Card For Home Assistant - Under Construction! 

I dunno what I am doing on Github however I've whipped up a Australian Fire Danger Rating card for Home Assistant!

Anyway, to get this running, you'll need the BOM integration installed (https://github.com/bremor/bureau_of_meteorology) and set to your location.

 Once your home location is set correctly, the BOM integration will make entities called:
"sensor.YOURLOCATION_fire_danger_0" 
"sensor.YOURLOCATION_fire_danger_1"
"sensor.YOURLOCATION_fire_danger_2"
"sensor.YOURLOCATION_fire_danger_3"
"sensor.YOURLOCATION_fire_danger_4"
and
"sensor.YOURLOCATION_fire_danger_5"

To use these entities (if you have BOM installed already, you should have these) you just need to copy and past the code below into a new "manual card" (add new card/right down the bottom), editing your location/sensor name and save the images in your HA www directory.

The FDR images need to be saved (and as stated, saved into your HA www folder):

none.png
moderate.png
high.png
extreme.png
catastrophic.png

Step by step once you have BOM and the attached images saved:

Create a new "manual card" (add new card/right down the bottom) on your dashboard

Copy & paste the YAML into the card you just created.

Don't forget to change every instace of "YOURLOCATION" to your location/sensor name...

Hit save and then done on your dashboard and it should now work. I hope. lol
