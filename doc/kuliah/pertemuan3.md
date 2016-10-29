RESUME

RETRIVE DATA GEOSPECIAL

A. Retrive data yaitu adalah melakukan select/ view data record pada file dbf dan gometri dari file shp. Tool yang dipake ya itu adlaah lip physhp

Cara terdapat 2 cara yaitu dengan menggunakan dbf dan shp sebelum nya apa itu sbf dan apa itu shp berikut penjelasanya

| DBF                                | SHP                                  |
|------------------------------------|--------------------------------------|
| -   Membuka data record            | -   Membuka geometri record          |
| -   Sf.records() = semua data      | - -   Sf.shpes() = mengambil semua   |
| - Sf.record(n) = ambil data ke N   | - Sf.shape = mengambil record ke n   |
| -   Sf.fileds = Melihat nama filed | -   dir                              |

1.  Example cara Hitung Record
 
A = sf.shapes() \# retrieve data geospecial 
 Len (A)                                                                    
 -   penjelasan A yang dimaksud adalah variable itu bebas mau denan variable apa saja                 
 -   Menghitung jumlah record di variable A dimana len() fungsi menghitung jumlah Array dala variale
 -   

1.  Example Melihat nama field

Nama-filed = sf.field                                                 
Print nama filed                                                               
 -   Penjelasan diatas merupakan cara meilhat nama filed dengan mengetikan di python  |
|-------------------------------------------------------------------------------------|

1.  Bagimana cara mengganti shapefile dengan nama yang lain caranya sbgai berikut
Import shapefile as coba     
                               
 Sf = coba.reader(‘Nama.shp’)  
                               
 Varjah = sf.shapes            
                               
 Len(varjah) 
Geom = sf.shape(1) 
                     
 Dir(geom) 
A.  shapefile terdapat beberapa isi diantaranya yaitu adalah

1.  Bbox : boundary box yaotu adalah box melihat peta atau koordinat

2.  Port : dibagi menjadi 1 record artinya secara keseluruhan

3.  Point : koordinat ketikan di cmd (gem.point).

B. SHAPETYPE

Shapetype adalah standar nomor jenis data geometri oleh ESRI

Link nya terdapat disini : shapefile.esri

Ingin melihat record bagaimana caranya , caranya sebagai berikut

Geom = sf.records() 
                          
Geom(1)              
                          
Atau bisa juga       

Geom = sf.record(1)  
                          
geom

C. Bagaimana Cara membuat Class Phthon

Code yang harus di ketik pada cmd bisa seperti dibawah

| Import shapefile                
                                  
 Class Gede(object):              
                                  
 Deff itungBaris(self.namafile):  
                                  
 Sf shapefile.Reader(namafile)    
                                  
 Rec = sf.shapes()                
                                  
 Return len(rec)                  |
|---------------------------------|

Apaila ingin memakai contruk jadi langsung tidak harus menginputkan seperti diatas bisa dengan code dibawah ini

| Import shapefile                     
                                       
 Class Gede(object):                   
                                       
 Def\_\_\_init\_\_(self.namafile):     
                                       
 Self.sf = shapefile,Reader(namafile)  
                                       
 Def itungBaris(self)                  
                                       
 Rec = self.sf.shapes()                
                                       
 Return len(rec)                       |
|--------------------------------------|
