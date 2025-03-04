# Hasil Belajar Prefix SQL dari Bootcamp DQLab

Repositori ini berisi hasil belajar saya mengenai prefix SQL selama mengikuti bootcamp di DQLab.

## Deskripsi

Dalam repositori ini, Anda akan menemukan berbagai contoh kode SQL yang menunjukkan penggunaan prefix dalam kueri SQL. 
Prefix digunakan untuk menghindari ambiguitas ketika mengakses kolom dari beberapa tabel yang memiliki nama kolom yang sama.

## Pengenalan Prefix SQL

Prefix SQL adalah cara untuk menentukan tabel asal kolom dalam kueri SQL. 
Ini sangat penting ketika Anda menggabungkan beberapa tabel dan ada kolom dengan nama yang sama di tabel-tabel tersebut.

## Contoh Penggunaan Prefix

Berikut adalah contoh sederhana penggunaan prefix:

```sql
SELECT
    customers.customer_id,
    orders.order_date
FROM
    customers
JOIN
    orders ON customers.customer_id = orders.customer_id;
