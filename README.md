**Stakewars** adalah program yang membantu komunitas menjadi terbiasa dengan apa artinya menjadi validator near dan memberi mereka kesempatan awal untuk mendapatkan akses ke produser khusus Chunk. Hadiah yang ditawarkan oleh program Stakewars mendukung anggota baru yang ingin bergabung dengan jaringan utama sebagai validator mulai akhir September 2022

**bagaimana cara memulainya?**
1.  Pelajari lebih lanjut tentang [stakewars](https://near.org/stakewars/)
2.  Lihat [Produser khusus Chunk](https://near.org/decentralize/)
3.  Isi [formulir](https://nearprotocol1001.typeform.com/to/Z39N7cU9) untuk mendaftar Produser Chunk-Only

Selanjutnya dalam artikel ini kita akan membuat dompet, menyewa vps dan menjalankan node

**Persyaratan Server untuk Produser Khusus Chunk:**
-   CPU: CPU 4-Core dengan dukungan AVX
-   RAM: 8GB DDR4
-   Penyimpanan: 500GB SSD

# Membeli vps
VPS di [contabo](https://contabo.com/en/) , tambahkan 400GB SSD ke dalamnya seharga €1,5 per bulan (500GB dinyatakan dalam persyaratan, dalam praktiknya 400GB sudah cukup).

![enter image description here](https://miro.medium.com/max/1400/1*XtewoLn07kdCKFPDjl3eBA.png)
# Buat Dompet Shardnet
Kami menyarankan Anda menggunakan browser yang tidak berbasis Chromium: Opera, Mozilla, IE

Buka [ [https://wallet.shardnet.near.org/](https://wallet.shardnet.near.org/) ] dan buat dompet, pilih nama Anda dan simpan frasa awal. Dinding ini akan digunakan untuk menyimpan token NEAR.

# Install NEAR CLI Dan dev tools
Menghubungkan ke server Anda

Sebelum memulai, Anda mungkin ingin memastikan bahwa mesin Anda memiliki fitur CPU yang tepat.

```
lscpu | grep -P '(?=.*avx )(?=.*sse4.2 )(?=.*cx16 )(?=.*popcnt )' > /dev/null \
  && echo "Supported" \
  || echo "Not supported"
```
> Input
To operate with NEAR Protocol network we need a tool. It’s called NEAR-CLI.

  



