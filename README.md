# apiapi
Sebuah latihan membuat API menggunakan python dan kawan-kawannya. Hasilnya bisa dicoba di [sini.](http://apiapi-1349.appspot.com/api/v1.0/news?key=d42a9ad09e9778b177d409f5716ac621)

Studi kasus: mengambil daftar berita (scraping menggunakan librari Bs4) dari situs [inilahkoran](http://www.inilahkoran.com). Keluaran berupa berkas json yang memuat data tautan, judul, kategori, dan id berita.

Contoh hasil keluaran:
```
{
  "page": "1",
  "results": [
    {
      "id": 0,
      "img": "http://www.inilahkoran.com/gallery/content/bandung/hut-cimahi-2016-fhi.jpg",
      "judul": "Peringatan HUT ke-15 Kota Cimahi Berlangsung Meriah",
      "kategori": "bandung",
      "kategori_id": 1,
      "link": "http://www.inilahkoran.com/berita/bandung/58632/peringatan-hut-ke-15-kota-cimahi-berlangsung-meriah",
      "url_id": 58632
    },
    ...
  ],
  "status": "ok",
  "total": 10
}
```

### Fungsi
* list berita

url: ```namadomain/api/v1.0/news?key=APIKEY```

* list berita per kategori

url: ```namadomain/api/v1.0/news/cat/cat_id?key=APIKEY```

* detail berita per id

url: ```namadomain/api/v1.0/news/url_id?key=APIKEY```
