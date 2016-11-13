**RESUME**

**MEMBUAT DATA GEOSPASIAL**

1.  Import Shapefile

2.  a = shapefile.Writer(*param*)

Apa yang dimaksud dengan Param ? Param dalam writer ini menunjukan shapetype apa yang akan kita buat contohnya **polygon, polyline,** dan **point**.

1.  a.point(x,y)

> Atau,
>
> a.poly(\[x,y\],\[v,w\])
>
> Perintah ini digunakan jika akan membuat file shp.

1.  a.field(‘nama’,’typedata’,’90’)

Perintah ini digunakan jika akan membuat file dbf.

a.record(‘isi’)

Perintah ini digunakan untuk mengisi file dbf.

1.  a.shp(‘namafile.shp’)

2.  save(‘namafile’)

Perintah untuk menyimpan file.

**Contoh Pembuatan field dalam dbf**

field(‘kota’,’b’,’50’)

Peritah ini berarti kita membuat sebuah atribut table bernama **kota** dengan tipedata **varchar** dengan panjang **50** karakter, kemudian jika ingin menambahkan data maka dapat dilakukan dengan perintah :

Record(‘Jakarta’)
