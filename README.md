# data-manipulation-pandas-python
Diberikan dataset ‘retail_raw_test.csv’
1.	Baca dataset
2.	Tipe data diubah menjadi tipe yang seharusnya
o	customer_id dari string ke int64,
o	quantity dari string ke int64,
o	item_price dari string ke int64
3.	Transform product_value supaya bentuknya seragam dengan format PXXXX, assign ke kolom baru "product_id", dan drop kolom "product_value", jika terdapat nan gantilah dengan "unknown".
4.	Tranform order_date menjadi value dengan format YYYY-MM-DD
5.	Cek data hilang dari tiap kolom dan kemudian isi missing value
o	Di brand dengan "no_brand", dan
o	Cek bagaimana missing value di city & province dengan cara isi missing value di city dan province dengan "unknown"
6.	Create column city/province dari gabungan city & province
7.	Membuat index berdasarkan city_provice, order_date, customer_id, order_id, product_id (cek index)
8.	Membuat kolom "total_price" sebagai hasil perkalian quantity dengan item_price
9.	Slice data hanya untuk Jan 2019
