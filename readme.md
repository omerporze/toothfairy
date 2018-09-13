# toothfairy
POC for CVE-2018-4330 (probably, read about it on the POC for CVE-2018-4327).
The code is not perfect but it does the job.

Tested on iPhone 6S 11.3.1  
Should work until 11.4

Let's you set the PC (ARM's version for IP register) to a value of your choice on bluetoothd and a few other services. 

Used @raniXCH bluetoothdPoC code to handle all the preparation of the Mach message and the sending of it to the BT service and adapted it to fit into this POC.  
Used jtool to find the ordinal and other stuff.  
Had to do a bit RE to find the correct message sizes.

credits:
@SparkZheng - for his awesome lecture on DEFCON 26.  
@raniXCH - for the excellent HITB presentation and the bluetoothdPoC.  
Jonathan Levin - for the great book and jtool.

refrences:
http://www.newosxbook.com/tools/jtool.html - jtool which I used in order to find the ordinal and other stuff.  
https://www.weibo.com/ttarticle/p/show?id=2309404271293301154324 - @SparkZheng material.  
https://github.com/rani-i/bluetoothdPoC - @raniXCH's POC code.  
https://gsec.hitb.org/materials/sg2018/D2%20-%20The%20Road%20to%20iOS%20Sandbox%20Escape%20-%20Rani%20Idan.pdf - @raniXCH's material part 1.  
https://blog.zimperium.com/cve-2018-4087-poc-escaping-sandbox-misleading-bluetoothd/ - @raniXCH's material part 2.  
https://github.com/omerporze/brokentooth - my POC for CVE-2018-4327.
