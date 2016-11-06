RESUME

RETRIVE DATA GEOSPECIAL

Pembahasan

1.  Retrive data geospecial kita tau yaitu mengambil data vector ESRI/shapefile dibagi 2 terdapat data DBF dan SHP. DBF dalah table atribut data sedangkan SHP adalah data geometri.

Terdapat 3 geometri standar ESRI

1.  Point

2.  Poline

3.  Poligon

<!-- -->

1.  Operasi pada Pyhton

    Library pyshp yaitu adalah IMPORT SHAPFILE penjelasan instansi kelas shapfile kepada sebuah variable

    Sf = shapefile.Reader(‘Bts.shp’)

    Penjelasan :

    SF = Variable

    Shapfile = Sebuah class

    Reader = Method

    Bts,shp = Parameter file

    Method method pada data DBF dan SHP

<!-- -->

1.  Method pada data DBF

    sf.fileds() adalah untuk melihat attribute table

    sf.records() adalah untuk mengambil semua record

    sf.record(n) adalah untuk isi record

2.  Method pada data SHP

> Sf.shapes() adalah untuk mengambil semua record geometri
>
> Sf.shape(n) adalah untuk mengambil 1 record pada baris n

Cara untuk mengambil 1 record dengan parameter nilai atau Array

1.  sf.records(0) \[8\]

2.  sf.field(0) \[8\]

Titik koordinat terdapat 4 titik

1.  BBOX

2.  POINT

3.  SHAPETYPE

Contoh Code untuk menampilkan nama Negara memakai contruk .

For a in sf.records():

If a\[8\] = “Indonesia””

Print a

Atau bisa juga

I = 0

For a in sf.records():

If a\[8\] ==”Zimbabwe”:

Print a :

I = i+1
