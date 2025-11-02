
# STUDI KASUS 3 : SISTEM GAJI KARYAWAN DENGAN SIMULASI PROYEK DAN JAM KERJA DINAMIS DENGAN BAHASA JAVA PADA VISUAL CODE   

# Kelompok 5
Nama Anggota :
1. Alicia Khairunnisya      (G1A025025)
2. Zora Ghaziyah Wanie      (G1A025027)
3. Andrian Revaldo          (G1A025113)
# Overview
Proyek ini merupakan sistem gaji karyawan dengan simulasi proyek dan jam kerja dinamis dengan menggunakan bahasa Java. Sistem menghitung gaji bersih setiap karyawan dengan mempertimbangkan jam kerja total, bonus proyek, dan pajak progresif. Setiap proyek memiliki tingkat kesulitan yang memengaruhi besar bonus, serta status penyelesaian proyek yang berpengaruh terhadap hasil akhir gaji.
# Struktur Program
1. Proyek

Mewakili satu proyek yang dikerjakan karyawan.
Atribut:

-nama (String): nama proyek

-tingkatKesulitan (int): tingkat kesulitan 1–5

-jamKerja (int): jumlah jam kerja yang digunakan

-selesai (boolean): status apakah proyek sudah selesai

2. Karyawan

Menyimpan data dan perhitungan gaji tiap karyawan.
Atribut:

-nama (String)

-daftarProyek (List<Proyek>)

-gajiPerJam (double)

Method utama:

-hitungTotalJam() → menjumlahkan semua jam kerja proyek

-hitungBonus() → 5% × total jam × rata-rata tingkat kesulitan

-hitungPajak() → pajak progresif (< 5 juta → 10%, < 10 juta → 15%,10 juta → 20%

-hitungGajiBersih() → menghitung gaji akhir setelah pajak

3. Departemen

Mengelola tim karyawan dalam satu departemen.
Atribut:

-tim (List<Karyawan>)

Method:

-tampilkanLaporanGaji() → menampilkan ringkasan gaji semua karyawan

-cariKaryawanPalingEfisien() → mencari karyawan dengan efisiensi tertinggi

4. MainGaji

Kelas utama yang menjalankan simulasi.
Fitur:

-Input data proyek untuk tiap karyawan

-Menampilkan gaji bersih dan laporan akhir

-Menggunakan looping, if–else, serta logika numerik kompleks