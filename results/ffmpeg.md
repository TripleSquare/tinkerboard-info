##ffmpeg reencode  

###### Disclaimer, inside the case I used, temperatures under load were very high (80°C) which resulted in thermal throttling  
>(/sys/class/thermal/thermal_zone1/temp)

Source Video File: [Big Buck Bunny 360p m4v](http://download.blender.org/peach/bigbuckbunny_movies/BigBuckBunny_640x360.m4v)  
Big Buck Bunny Website: [click me](https://peach.blender.org/)  


**Used command**  
>```ffmpeg -i BigBuckBunny_640x360.m4v -fs 50MB -vf "scale=trunc(iw/2)*2:trunc(ih/2)*2" -vcodec libx264 -acodec copy encoded.mp4```

**last line of encoding**
>frame=14316 fps= 42 q=-1.0 Lsize=   47577kB time=00:09:56.45 bitrate= 653.4kbits/s speed=1.74x  

**additional info**
>video:37847kB audio:9286kB subtitle:0kB other streams:0kB global headers:0kB muxing overhead: 0.941952%  
[libx264 @ 0x80317a50] frame I:156   Avg QP:17.29  size: 37248  
[libx264 @ 0x80317a50] frame P:5368  Avg QP:22.34  size:  4862  
[libx264 @ 0x80317a50] frame B:8792  Avg QP:27.11  size:   778  
[libx264 @ 0x80317a50] consecutive B-frames: 10.4% 18.7% 13.8% 57.2%  
[libx264 @ 0x80317a50] mb I  I16..4: 23.8% 41.7% 34.5%  
[libx264 @ 0x80317a50] mb P  I16..4:  2.2%  4.7%  1.5%  P16..4: 33.0%  8.6%  5.8%  0.0%  0.0%    skip:44.2%  
[libx264 @ 0x80317a50] mb B  I16..4:  0.1%  0.5%  0.2%  B16..8: 24.5%  1.9%  0.5%  direct: 0.7%  skip:71.6%  L0:47.2% L1:47.2% BI: 5.7%  
[libx264 @ 0x80317a50] 8x8 transform intra:53.1% inter:56.2%  
[libx264 @ 0x80317a50] coded y,uvDC,uvAC intra: 62.4% 66.9% 35.3% inter: 9.8% 10.4% 2.0%  
[libx264 @ 0x80317a50] i16 v,h,dc,p: 25% 26% 18% 31%  
[libx264 @ 0x80317a50] i8 v,h,dc,ddl,ddr,vr,hd,vl,hu: 21% 18% 24%  5%  6%  8%  6%  6%  7%  
[libx264 @ 0x80317a50] i4 v,h,dc,ddl,ddr,vr,hd,vl,hu: 28% 17% 18%  5%  7%  7%  6%  6%  6%  
[libx264 @ 0x80317a50] i8c dc,h,v,p: 48% 23% 18% 11%  
[libx264 @ 0x80317a50] Weighted P-Frames: Y:4.0% UV:2.4%  
[libx264 @ 0x80317a50] ref P L0: 70.1% 14.2% 11.2%  4.3%  0.1%  
[libx264 @ 0x80317a50] ref B L0: 91.1%  7.8%  1.1%  
[libx264 @ 0x80317a50] ref B L1: 95.2%  4.8%  
[libx264 @ 0x80317a50] kb/s:519.76  