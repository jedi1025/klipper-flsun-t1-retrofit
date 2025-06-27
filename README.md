Welcome to the Klipper project!

[![Klipper](docs/img/klipper-logo-small.png)](https://www.klipper3d.org/)

https://www.klipper3d.org/

The Klipper firmware controls 3d-Printers. It combines the power of a
general purpose computer with one or more micro-controllers. See the
[features document](https://www.klipper3d.org/Features.html) for more
information on why you should use the Klipper software.

Start by [installing Klipper software](https://www.klipper3d.org/Installation.html).

Klipper software is Free Software. See the [license](COPYING) or read
the [documentation](https://www.klipper3d.org/Overview.html). We
depend on the generous support from our
[sponsors](https://www.klipper3d.org/Sponsors.html).


all that out of the way...


DO NOT USE THIS YET.  IT IS STILL A WORK IN PROGRESS!!!!!
...
HOWEVER...

Update 06/01/2025:
~~/config/flsun-retrofit/WIP-printer.cfg "SHOULD" be good enough to get started with.~~

I have a new Intel SBC and BTT Kraken arriving tomorrow (hopefully...thanks Amazon) and 
will begin actual testing once all is wired up.  If you wish to test this config file on 
your own, you may freely do so, however it is YOUR responsibility to make sure all 
precautions are taken not to damage anything when those arms start swinging around.  

I TAKE NO RESPONSIBILITY for anybody using something i haven't personally tested yet.  

That being said, if you try it, whatever the results, please do share them.

Update 06/02/2025:
Yup, Amazon strikes again.  Kraken DOA...3 more days...

Update 06/13/2025:
It's a functional printer!  Haven't tested anything higher than 400mm/s due to belt and hot end mechanical issues.
But, up to that speed is a good printer.  ADXL is currently disabled, as is load cell bed leveling.  In it's place, and end stop connector is wired up to 
the nozzle and the metallic side of the bed.  SLOW approach to avoid ramming the bed...cold delta calibrate and ONE hot bed mesh should not damage either hotend or nozzle.
When they contact circuit closes and next spot to test.  Working config file can be found at:
 
/config/flsun-retrofit/basic_printer.cfg

If you want to try going for full stock speed up front:
 
/config/flsun-retrofit/stock_speed_printer.cfg

My current useable config file:

/config/flsun-retrofit/current/printer.cfg

Either way you will almost certainly have to reconfigure the pin assignments.  Odds are the rest of klipper's config files should have something that matches your board.  Just grab the  appropriate config file and copy ONLY pin assignments and driver configs over they're RESPECTIVE entries.  That should get you functional, then 
you'll need to iron out whatever little details specific to your setup.

I still TAKE NO RESPONSIBILITY for YOUR hardware.  This works on MINE...at least well enough that i feel confident sharing.  It is YOUR RESPONSIBILITY to confirm all data contained
in these config files BEFORE applying any of them.  IF YOU ARE ATTEMPTING THIS, I EXPECT THAT:

     1. YOU KNOW WHAT YOU ARE DOING

     2. YOU ARE COMFORTABLE WORKING WITH SENSITIVE ELECTRONICS AND POTENTIALLY DANGEROUS VOLTAGES AND AMPERAGES
     
     3. YOU ARE ASSUMING ALL RESPONSIBILITY FOR ANY DAMAGE AS A RESULT OF TRYING THIS
     
     4. YOU HAVE THE SAME LOVE/HATE RELATIONSHIP WITH THESE PRINTERS THAT I DO...or something like that.

More to come...
