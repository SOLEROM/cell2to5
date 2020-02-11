

https://docs.legato.io/latest/c_mrcNeighborCells.html


## examples


```
You don’t need to be attached but a SIM card is required.

ati
Manufacturer: Sierra Wireless, Incorporated
Model: WP7607-1
Revision: SWI9X07Y_02.18.05.00 000000 jenkins 2018/07/19 17:40:21
IMEI: 359780080103033
IMEI SV:  5
FSN: VP804370370310
+GCAP: +CGSM


OK
at+kcell=0
+CME ERROR: SIM not inserted

```

```
AT+KSRAT=1
OK
+CGREG: 1,“2540”,“7ACA”,3,“02”
+CGREG: 1,“2540”,“7ACA”,3,“02”
AT+COPS?
+COPS: 0,0,“CHN-UNICOM”,0
OK
AT+CGREG?
+CGREG: 2,1,“2540”,“7ACA”,3,“02”
OK
AT+KCELL=0
+KCELL: 7,
0,688,25,64f010,2540,7aca,25,255, //0 GSM serving cell
1,783,57,64f010,2540,7c3d,24, //1 GSM neighbor cell
1,641,13,64f010,2540,7acc,14, //1 GSM neighbor cell
1,640,38,64f010,2540,ffff,11, //1 GSM neighbor cell
1,690,255,64f010,ffff,ffff,0, //1 GSM neighbor cell
1,645,255,64f010,ffff,ffff,0, //1 GSM neighbor cell
1,648,255,64f010,ffff,ffff,0 //1 GSM neighbor cell
+KCELL: 0
OK
```
