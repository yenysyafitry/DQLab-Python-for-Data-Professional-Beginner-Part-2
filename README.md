<p align="justify"><b>Collections manipulation</b> adalah salah satu teknik yang penting untuk dikuasai setiap programmer. Melalui penguasaan materi collections  manipulation, aku dapat mengolah berbagai tipe data collections dalam Python yang meliputi:</p>
<ol><li>list,</li>
<li>tuple,</li>
<li>set, dan</li>
<li>Dictionary.</li></ol>
<details align="justify"> <summary><b>Mengakses List dan Tuple – Part 1</b></br>Seperti yang telah aku pelajari pada module Python for Data Professional Beginner - Part 1, bab “sequence type”, aku dapat mengakses elemen pada suatu list ataupun tuple dengan menggunakan indeks atau semacam nomor urut dari list atau tuple tersebut. Indeks pada suatu tipe data list atau tuple dimulai dari angka 0.</br></br>
bulan_pembelian = ('januari', 'Februari', 'Maret', 'April', 'Mei', 'Juni', 'Juli', 'Agustus', 'September', 'Oktober', 'November', 'Desember')</br>
print(bulan_pembelian[0])</br>
print(bulan_pembelian[5])</br>
print(bulan_pembelian[-1])</br>
print(bulan_pembelian[-2])</br></br>
</summary><table align="justify"><i>Output : </br>januari</br>
Juni</br>
Desember</br>
November</i></table></details>

<details align="justify"> <summary><b>Mengakses List dan Tuple – Part 2</b></br>Cara collections manipulation pertama yang akan aku pelajari adalah memotong (slicing) list/ tuple dengan menggunakan rentangan nilai indeks (range of index).</br></br>bulan_pembelian = ('januari', 'Februari', 'Maret', 'April', 'Mei', 'Juni', 'Juli', 'Agustus', 'September', 'Oktober', 'November', 'Desember')</br>
pertengahan_tahun = bulan_pembelian [4:8]</br>
print(pertengahan_tahun)</br>
awal_tahun = bulan_pembelian[:5]</br>
print(awal_tahun)</br>
akhir_tahun = bulan_pembelian[8:]</br>
print(akhir_tahun)</br>
print(bulan_pembelian[-4:-1])</br></br>
</summary><table align="justify"><i>Output : </br>('Mei', 'Juni', 'Juli', 'Agustus')</br>
('januari', 'Februari', 'Maret', 'April', 'Mei')</br>
('September', 'Oktober', 'November', 'Desember')</br>
('September', 'Oktober', 'November')</i></table></details>

<details align="justify"> <summary>  <b> Penggabungan Dua atau Lebih List atau Tuple </b>  </br>Selain dapat melakukan pemotongan terhadap tipe data list/ tuple, aku juga dapat menggabungkan isi dari suatu list (ataupun tuple) dengan list lainnya (dengan tuple lainnya) dengan menggunakan operator penambahan (+). </br></br>
list_makanan = ['Gado-Gado', 'Ayam Goreng', 'Rendang']</br>
list_minuman = ['Es Teh', 'Es Jeruk', 'Es Campur']</br>
list_menu = list_makanan + list_minuman</br>
print(list_menu)</br></br>
</summary><table align="justify"><i>Output : </br>['Gado-Gado', 'Ayam Goreng', 'Rendang', 'Es Teh', 'Es Jeruk', 'Es Campur']</i></table></details>

<details align="justify"> <summary><b> List Manipulation – Part 1 </b></br>Untuk memanipulasi tipe data list, aku dapat menggunakan sekumpulan fitur yang telah tersedia dalam bahasa pemrograman Python. Merujuk pada tabel di bawah, aku dapat memahami fitur-fitur untuk melakukan manipulasi data yang terdiri atas append(), clear(), copy(), count() dan extend()</br>
</br># Fitur .append()</br>
print(">>> Fitur .append()")</br>
list_makanan = ['Gado-gado', 'Ayam Goreng', 'Rendang']</br>
list_makanan.append('Ketoprak')</br>
print(list_makanan)</br>
# Fitur .clear()</br>
print(">>> Fitur .clear()")</br>
list_makanan = ['Gado-gado', 'Ayam Goreng', 'Rendang']</br>
list_makanan.clear()</br>
print(list_makanan)</br>
# Fitur .copy()</br>
print(">>> Fitur .copy()")</br>
list_makanan1 = ['Gado-gado', 'Ayam Goreng', 'Rendang']</br>
list_makanan2 = list_makanan1.copy()</br>
list_makanan3 = list_makanan1</br>
list_makanan2.append('Opor')</br>
list_makanan3.append('Ketoprak')</br>
print(list_makanan1)</br>
print(list_makanan2)</br>
# Fitur .count()</br>
print(">>> Fitur .count()")</br>
list_score = ['Budi', 'Sud', 'Budi', 'Budi', 'Budi', 'Sud', 'Sud']</br>
score_budi = list_score.count('Budi')</br>
score_sud = list_score.count('Sud')</br>
print(score_budi) # akan menampilkan output 4</br>
print(score_sud) # akan menampilkan output 3</br>
# Fitur .extend()</br>
print(">>> Fitur .extend()")</br>
list_menu = ['Gado-gado', 'Ayam Goreng', 'Rendang']</br>
list_minuman = ['Es Teh', 'Es Jeruk', 'Es Campur']</br>
list_menu.extend(list_minuman)</br>
print(list_menu)</br></br>
</summary><table align="justify"><i>Output : </br>
  >>> Fitur .append()</br>
['Gado-gado', 'Ayam Goreng', 'Rendang',</br> 'Ketoprak']</br>
>>> Fitur .clear()</br>
[]</br>
>>> Fitur .copy()</br>
['Gado-gado', 'Ayam Goreng', 'Rendang', 'Ketoprak']</br>
['Gado-gado', 'Ayam Goreng', 'Rendang', 'Opor']</br>
>>> Fitur .count()</br>
4</br>
3</br>
>>> Fitur .extend()</br>
['Gado-gado', 'Ayam Goreng', 'Rendang', 'Es Teh', 'Es Jeruk', 'Es Campur']</i></table></details>

<details align="justify"> <summary><b>List Manipulation – Part 2</b></br>Selanjutnya aku akan mempelajari fitur index(), insert(), pop(), remove(), reverse(), dan sort() untuk melakukan manipulasi.</br></br># Fitur .index()</br>
print(">>> Fitur .index()")</br>
list_score = ['Budi','Sud','Budi','Budi','Budi','Sud','Sud']</br>
score_pertama_sud = list_score.index('Sud') + 1</br>
print(score_pertama_sud) # akan menampilkan output 2</br>
#Fitur .insert()</br>
print(">>> Fitur .insert()")</br>
list_score = ['Budi','Sud','Budi','Budi','Sud']</br>
list_score.insert(3, 'Sud')</br>
print(list_score)</br>
#Fitur .pop()</br>
print(">>> Fitur .pop()")</br>
list_menu = ['Gado-gado', 'Ayam Goreng', 'Rendang']</br>
list_menu.pop(1)</br>
print(list_menu)</br>
#Fitur .remove()</br>
print(">>> Fitur .remove()")</br>
list_menu = ['Gado-gado', 'Ayam Goreng', 'Rendang', 'Ketoprak']</br>
list_menu.remove('Rendang')</br>
print(list_menu)</br>
#Fitur .reverse()</br>
print(">>> Fitur .reverse()")</br>
list_menu = ['Gado-gado', 'Ayam Goreng', 'Rendang', 'Ketoprak']</br>
list_menu.reverse()</br>
print(list_menu)</br>
#Fitur .sort()</br>
print(">>> Fitur .sort()")</br>
list_menu = ['Gado-gado', 'Ayam Goreng', 'Rendang', 'Ketoprak']</br>
list_menu.sort() #Default: Ascending</br>
print(list_menu) </br>
list_menu.sort(reverse=True)# Descending</br>
print(list_menu) </br></br>
</summary><table align="justify"><i>Output : </br>>>> Fitur .index()</br>
2</br>
>>> Fitur .insert()</br>
['Budi', 'Sud', 'Budi', 'Sud', 'Budi', 'Sud']</br>
>>> Fitur .pop()</br>
['Gado-gado', 'Rendang']</br>
>>> Fitur .remove()</br>
['Gado-gado', 'Ayam Goreng', 'Ketoprak']</br>
>>> Fitur .reverse()</br>
['Ketoprak', 'Rendang', 'Ayam Goreng', 'Gado-gado']</br>
>>> Fitur .sort()</br>
['Ayam Goreng', 'Gado-gado', 'Ketoprak', 'Rendang']</br>
['Rendang', 'Ketoprak', 'Gado-gado', 'Ayam Goreng']</i></table></details>

<details align="justify"> <summary><b>Tuple Manipulation</b></br></br>
#Fitur .count()</br>
print(">>> Fitur .count()")</br>
tuple_score = ('Budi', 'Sud', 'Budi', 'Budi', 'Budi', 'Sud', 'Sud')</br>
score_budi = tuple_score.count('Budi')</br>
score_sud = tuple_score.count('Sud')</br>
print(score_budi) # akan menampilkan output 4</br>
print(score_sud) # akan menampilkan output 3</br>
#Fitur .index()</br>
print(">>> Fitur .index()")</br>
tuple_score = ('Budi','Sud','Budi','Budi','Budi','Sud','Sud')</br>
score_pertama_sud = tuple_score.index('Sud')+1</br>
print(score_pertama_sud) # akan menampilkan output 2</br></br>
</summary><table align="justify"><i>Output : </br>>>> Fitur .count()</br>
4</br>
3</br>
>>> Fitur .index()</br>
2</i></table></details>

<details align="justify"> <summary><b>Set Manipulation – Part 1</b></br>Sedikit berbeda dengan tipe data list dan tuple, pada tipe data set terdapat cukup banyak fitur yang disediakan oleh bahasa Python.</br></br>#Fitur .add()</br>
print(">>> Fitur .add()")</br>
set_buah = {'Jeruk','Apel','Anggur'}</br>
set_buah.add('Melon')</br>
print(set_buah)</br>
#Fitur .clear()</br>
print(">>> Fitur .clear()")</br>
set_buah = {'Jeruk','Apel','Anggur'}</br>
set_buah.clear()</br>
print(set_buah)</br>
#Fitur .copy()</br>
print(">>> Fitur .copy()")</br>
set_buah1 = {'Jeruk','Apel','Anggur'}</br>
set_buah2 = set_buah1</br>
set_buah3 = set_buah1.copy()</br>
set_buah2.add('Melon')</br>
set_buah3.add('Kiwi')</br>
print(set_buah1)</br>
print(set_buah2)
#Fitur .update()</br>
print(">>> Fitur .update()")</br>
parcel1 = {'Anggur','Apel','Jeruk'}</br>
parcel2 = {'Apel','Kiwi','Melon'}</br>
parcel1.update(parcel2)</br>
print(parcel1)</br>
#Fitur .pop()</br>
print(">>> Fitur .pop()")</br>
parcel = {'Anggur','Apel','Jeruk'}</br>
buah = parcel.pop()</br>
print(buah)</br>
print(parcel)</br>
#Fitur .remove()</br>
print(">>> Fitur .remove()")</br>
parcel = {'Anggur','Apel','Jeruk'}</br>
parcel.remove('Apel')</br>
print(parcel)</br></br>
</summary><table align="justify"><i>Output : </br>>>> Fitur .add()</br>
{'Jeruk', 'Anggur', 'Melon', 'Apel'}</br>
>>> Fitur .clear()</br>
set()</br>
>>> Fitur .copy()</br>
{'Jeruk', 'Anggur', 'Melon', 'Apel'}</br>
{'Jeruk', 'Anggur', 'Melon', 'Apel'}</br>
>>> Fitur .update()</br>
{'Kiwi', 'Melon', 'Jeruk', 'Anggur', 'Apel'}</br>
>>> Fitur .pop()</br>
Jeruk</br>
{'Anggur', 'Apel'}</br>
>>> Fitur .remove()</br>
{'Jeruk', 'Anggur'}</br>
  </i></table></details>

<details align="justify"> <summary><b>Set Manipulation – Part 2</b></br>Sedikit berbeda dengan tipe data list dan tuple, pada tipe data set terdapat cukup banyak fitur manipulasi yang bisa aku gunakan.</br></br>
#Fitur .union()</br>
print(">>> Fitur .union()")</br>
parcel1 = {'Anggur','Apel','Jeruk'}</br>
parcel2 = {'Apel','Kiwi','Melon'}</br>
parcel3 = parcel1.union(parcel2)</br>
print(parcel1)</br>
print(parcel3)</br>
#Fitur .isdisjoint()</br>
print(">>> Fitur .isdisjoint()")</br>
parcel1 = {'Anggur','Apel','Jeruk'}</br>
parcel2 = {'Kiwi','Melon','Pisang'}</br>
parcel3 = {'Apel','Srikaya','Semangka'}</br>
parcel1_parcel2_disjoint = parcel1.isdisjoint(parcel2)</br>
print(parcel1_parcel2_disjoint)</br>
parcel1_parcel3_disjoint = parcel1.isdisjoint(parcel3)</br>
print(parcel1_parcel3_disjoint)</br>
#Fitur .issubset()</br>
print(">>> Fitur .issubset()")</br>
parcel_A = {'Anggur', 'Apel'}</br>
parcel_B = {'Durian','Semangka','Apel'}</br>
parcel_C = {'Anggur', 'Kiwi', 'Apel', 'Jeruk', 'Melon'}</br>
parcel_A_dalam_C = parcel_A.issubset(parcel_C)</br>
parcel_B_dalam_C = parcel_B.issubset(parcel_C)</br>
print(parcel_A_dalam_C)</br>
print(parcel_B_dalam_C)</br>
#Fitur .issuperset()</br>
print(">>> Fitur .issuperset()")</br>
parcel_C_mengandung_A = parcel_C.issuperset(parcel_A)</br>
parcel_C_mengandung_B = parcel_C.issuperset(parcel_B)</br>
print(parcel_C_mengandung_A)</br>
print(parcel_C_mengandung_B)</br>
#Fitur .intersection()</br>
print(">>> Fitur .intersection()")</br>
parcel_A = {'Anggur', 'Kiwi', 'Apel', 'Jeruk', 'Melon'}</br>
parcel_B = {'Apel', 'Jeruk', 'Semangka', 'Durian', 'Tomat'}</br>
parcel_C = parcel_A.intersection(parcel_B)</br>
print(parcel_C)</br>
#Fitur .difference()</br>
print(">>> Fitur .difference()")</br>
parcel_C = parcel_A.difference(parcel_B)</br>
print(parcel_C)</br>
#Fitur .symmetric_difference()</br>
print(">>> Fitur .symmetric_difference()")</br>
parcel_A = {'Anggur', 'Apel', 'Jeruk', 'Melon'}</br>
parcel_B = {'Apel','Jeruk','Semangka','Leci'}</br>
parcel_C = parcel_A.symmetric_difference(parcel_B)</br>
print(parcel_C)</br></br>
</summary><table align="justify"><i>Output : </br>>>> Fitur .union()</br>
{'Anggur', 'Apel', 'Jeruk'}</br>
{'Anggur', 'Melon', 'Kiwi', 'Jeruk', 'Apel'}</br>
>>> Fitur .isdisjoint()</br>
True</br>
False</br>
>>> Fitur .issubset()</br>
True</br>
False</br>
>>> Fitur .issuperset()</br>
True</br>
False</br>
>>> Fitur .intersection()</br>
{'Jeruk', 'Apel'}</br>
>>> Fitur .difference()</br>
{'Anggur', 'Melon', 'Kiwi'}</br>
>>> Fitur .symmetric_difference()</br>
{'Anggur', 'Melon', 'Leci', 'Semangka'}</i></table></details>

<details align="justify"> <summary><b>Dictionary Manipulation</b></br>#Fitur .clear()</br>
print(">>> Fitur .clear()")</br>
info_karyawan = {'nama' : 'Aksara','nik' : '1211011','pekerjaan' : 'Data Analyst'}</br>
info_karyawan.clear()</br>
print(info_karyawan)</br>
#Fitur .copy()</br>
print(">>> Fitur .copy()")</br>
info_karyawan1 = {'nama' : 'Aksara','nik' : '1211011','pekerjaan' : 'Data Analyst'}</br>
info_karyawan2 = info_karyawan1.copy()</br>
info_karyawan2['nama'] = 'Senja'</br>
info_karyawan2['nik'] = '1211056'</br>
print(info_karyawan1)</br>
print(info_karyawan2)</br>
#Fitur .keys()</br>
print(">>> Fitur .keys()")</br>
info_karyawan = {'nama' : 'Aksara',</br>
'nik' : '1211011','pekerjaan' : 'Data Analyst'}</br>
kunci_akses = list(info_karyawan.keys())</br>
print(kunci_akses)</br>
#Fitur .values()</br>
print(">>> Fitur .values()")</br>
value_dict = list(info_karyawan.values())</br>
print(value_dict)</br>
#Fitur .update()</br>
print(">>> Fitur .update()")</br>
info_karyawan.update({'skillset':['Python', 'R']})</br>
print(info_karyawan)</br></br>

</summary><table align="justify"><i>Output : </br>>>> Fitur .clear()</br>
{}</br>
>>> Fitur .copy()</br>
{'pekerjaan': 'Data Analyst', 'nama': 'Aksara', 'nik': '1211011'}</br>
{'pekerjaan': 'Data Analyst', 'nama': 'Senja', 'nik': '1211056'}</br>
>>> Fitur .keys()</br>
['pekerjaan', 'nama', 'nik']</br>
>>> Fitur .values()</br>
['Data Analyst', 'Aksara', '1211011']</br>
>>> Fitur .update()</br>
{'pekerjaan': 'Data Analyst', 'skillset': ['Python', 'R'], 'nama': 'Aksara', 'nik': '1211011'} </i></table></details>

<details align="justify"> <summary><b>Useful Tips and Tricks</b></br>Untuk menentukan berapa jumlah data yang tersimpan di setiap elemen pada tuple/list, aku dapat menggunakan fungsi buit-in len(). </br></br>#Tuple</br>
print(">>> Tuple")</br>
tuple_menu = ('Gado-gado','Ayam Goreng','Rendang','Ketoprak')</br>
jumlah_menu = len(tuple_menu)</br>
print(jumlah_menu)</br>
#List</br>
print(">>> List")</br>
list_menu = ['Gado-gado','Ayam Goreng','Rendang','Ketoprak']</br>
jumlah_menu = len(list_menu)</br>
print(jumlah_menu)</br>
#Konversi tipe data</br>
print(">>> Konversi tipe data")</br>
list_buah = ['Apel', 'Apel', 'Jeruk', 'Markisa', 'Jeruk', 'Markisa', 'Apel']</br>
set_buah = set(list_buah)</br>
print(set_buah)</br>
list_buah = list(set_buah)</br>
list_buah.sort()</br>
print(list_buah)</br></br>
</summary><table align="justify"><i>Output : </br>>>> Tuple</br>
4</br>
>>> List</br>
4</br>
>>> Konversi tipe data</br>
{'Markisa', 'Jeruk', 'Apel'}</br>
['Apel', 'Jeruk', 'Markisa'] </br></i></table></details>


<details align="justify"> <summary><b>Tugas Praktek</b></br>#Data keuangan</br>
keuangan = {</br>
'pengeluaran': [2, 2.5, 2.25, 2.5, 3.2, 2.5, 3.5, 4, 3],</br>
'pemasukan': [7.8, 7.5, 9, 7.6, 7.2, 7.5, 7, 10, 7.5]</br>
}</br>
#Perhitungan rata-rata pemasukan dan rata-rata pengeluaran</br>
total_pengeluaran = 0</br>
total_pemasukan = 0</br>
for biaya in keuangan['pengeluaran']: </br>
    total_pengeluaran += biaya</br>
for biaya in keuangan['pemasukan']: </br>
    total_pemasukan += biaya</br>
rata_rata_pengeluaran = total_pengeluaran / len(keuangan['pengeluaran'])</br>
rata_rata_pemasukan = total_pemasukan / len(keuangan['pemasukan'])</br>
print(rata_rata_pengeluaran) </br>
print(rata_rata_pemasukan)</br></br>
</summary><table align="justify"><i>Output : </br>2.8277777777777775</br>
7.8999999999999995 </i></table></details>

<details align="justify"> <summary><b>Apa itu String Manipulation</b></br>String manipulation adalah teknik yang digunakan dalam memanipulasi data yang disimpan dalam tipe data str. Pada bahasa Python, untuk mempermudah proses pengolahan data, tipe data string dapat diperlakukan layaknya seperti tipe data list.</br></br>nama_produk = "Sepatu Niko"</br>
nama_produk = nama_produk[:2] + "P" + nama_produk[3:9] + "K" + nama_produk[-1]</br>
print(nama_produk)</br>
print(nama_produk[:7])</br>
print(nama_produk[7:])</br>
print(len(nama_produk))</br></br>
</summary><table align="justify"><i>Output : </br>SePatu NiKo</br>
SePatu </br>
NiKo</br>
11</i></table></details>

<details align="justify"> <summary><b>Operator “+” untuk Tipe Data String</b></br>Setelah aku mempelajari String Manipulation, sekarang aku beralih ke Operator “+”. Operator + pada dua string akan secara otomatis menggabungkan kedua string tersebut. Operator + juga dapat digunakan untuk menambahkan beberapa string secara  sekaligus.
Aku mengikuti contoh yang diberikan dengan mengetik syntax pada live code editor untuk memahami bagaimana Operation “+” bekerja pada Python.</br></br>nama_depan = 'John'
nama_belakang = 'Doee'</br>
nama_lengkap = nama_depan + ' ' + nama_belakang</br>
print(nama_lengkap)</br>
umur = '27 tahun'</br>
alamat = 'Jl. Anggrek No. 100'</br>
nama_umur_alamat = 'Hi, saya ' + nama_lengkap + 'umur' + umur + ',tinggal di' + alamat + '.'</br>
print(nama_umur_alamat)</br>
</summary><table align="justify"><i>Output : </br></br>John Doee</br>
Hi, saya John Doeeumur27 tahun,tinggal diJl. Anggrek No. 100.</i></table></details>

<details align="justify"> <summary><b>Menghilangkan Spasi di Awal dan/atau di Akhir</b></br>#Fitur .strip()</br>
print(">>> Fitur .strip()")</br>
kata_sambutan = ' halo, selamat siang!  </br> '
kata_sambutan = kata_sambutan.strip()</br>
print(kata_sambutan)</br>
#Fitur .lstrip()</br>
print(">>> Fitur .lstrip()")</br>
kata_sambutan = ' halo, selamat siang!  </br> '
kata_sambutan = kata_sambutan.lstrip()</br>
print(kata_sambutan)</br>
#Fitur .rstrip()</br>
print(">>> Fitur .rstrip()")</br>
kata_sambutan = ' halo, selamat siang!   </br>'
kata_sambutan = kata_sambutan.rstrip()</br>
print(kata_sambutan)</br>
</summary><table align="justify"><i>Output :</br>>>> Fitur .strip()</br>
halo, selamat siang!</br>
>>> Fitur .lstrip()</br>
halo, selamat siang!   </br>
>>> Fitur .rstrip()</br>
 halo, selamat siang!  </i></table></details>


<details align="justify"> <summary><b>Merubah Caps pada String</b></br>Pada bagian ini, aku akan mempelajari cara merubah caps (penggunaan huruf besar dan kecil). Jika diawal kalimat pada suatu string yang dimiliki belum berupa huruf kapital maka dengan menggunakan fitur .capitalize() kita dengan mudah merubah string tersebut menjadi kalimat yang benar secara bahasa.</br></br>#Fitur .capitalize()</br>
print(">>> Fitur .capitalize()")</br>
judul_buku = 'belajar bahasa Python'</br>
print(judul_buku.capitalize())</br>
#Fitur .lower()</br>
print(">>> Fitur .lower()")</br>
judul_buku = 'Belajar Bahasa PYTHON.'</br>
print(judul_buku.lower())</br>
#Fitur .upper()</br>
print(">>> Fitur .upper()")</br>
judul_buku = 'Belajar Bahasa PYTHON.'</br>
print(judul_buku.upper())</br>
</summary><table align="justify"><i>Output : </br> >>> Fitur .capitalize()</br>
Belajar bahasa python</br>
>>> Fitur .lower()</br>
belajar bahasa python.</br>
>>> Fitur .upper()</br>
BELAJAR BAHASA PYTHON. </i></table></details>

<details align="justify"> <summary><b>Pemecahan, Penggabungan, dan Penggantian String</b></br>aku akan mempelajari bagaimana cara memecah suatu string dengan kondisi tertentu sehingga menghasilkan list of string. Kemudian, akan dipelajari bagaimana cara menggabungkan beberapa list of string menjadi string saja. Akhirnya, aku akan mengganti sub-string tertentu dengan sub-string lainnya sehingga merubah string awalnya.</br></br>#Fitur .split()</br>
print(">>> Fitur .split()")</br>
bilangan = "ani dan budi dan wati dan johan"</br>
karakter = bilangan.split("dan")</br>
print(karakter)</br>
kata = bilangan.split(" ")</br>
print(kata)</br>
#Fitur .join()</br>
print(">>> Fitur .join()")</br>
pemisah = " dan "</br>
karakter = ["Ricky", "Peter", "Jordan"]</br>
kalimat = pemisah.join(karakter)</br>
print(kalimat)</br>
#Fitur .replace()</br>
print(">>> Fitur .replace()")</br>
kalimat = "apel malang apel yang paling segar, apel sehat, apel nikmat"</br>
kalimat = kalimat.replace("apel", "jeruk")</br>
print(kalimat)</br>
</summary><table align="justify"><i>Output : </br>>>> Fitur .split()</br>
['ani ', ' budi ', ' wati ', ' johan']</br>
['ani', 'dan', 'budi', 'dan', 'wati', 'dan', 'johan']</br>
>>> Fitur .join()</br>
Ricky dan Peter dan Jordan</br>
>>> Fitur .replace()</br>
jeruk malang jeruk yang paling segar, jeruk sehat, jeruk nikmat</i></table></details>

<details align="justify"> <summary><b>Menentukan Posisi dan Jumlah Sub-string pada String</b></br>aku akan mempelajari bagaimana cara menentukan posisi awal suatu sub-string dan jumlah kemunculan sub-string tersebut pada suatu string. Agar lebih memahami bagaimana penerapannya pada Python.</br></br>teks = "Apel malang adalah apel termanis dibanding apel-apel lainnya"</br>
#Fitur .find()</br>
print(">>> Fitur .find()")</br>
print(teks.find("Apel"))</br>
print(teks.find("malang"))</br>
#Fitur .count()</br>
print(">>> Fitur .count()")</br>
kemunculan_kata_apel = teks.count("apel")</br>
print(kemunculan_kata_apel)</br>
</summary><table align="justify"><i>Output : </br>H</i></table></details>

<details align="justify"> <summary><b>Menentukan String Apakah Diawali/Diakhiri oleh Sub-string</b></br>Pada bagian ini, aku akan mempelajari bagaimana menentukan apakah suatu string diawali atau diakhiri dengan suatu substring (teks) tertentu.</br>
  
  </br>#Fitur .startswith()</br>
print(">>> Fitur .startswith()")</br>
teks = "Apel malang adalah apel termanis dibanding apel-apel lainnya"</br>
print(teks.startswith("Apel"))</br>
print(teks.startswith("apel"))</br>
#Fitur .endswith()</br>
print(">>> Fitur .endswith()")</br>
print(teks.endswith("lainnya"))</br>
print(teks.endswith("apel"))</br></br>
</summary><table align="justify"><i>Output : </br>>>> Fitur .startswith()</br>
True</br>
False</br>
>>> Fitur .endswith()</br>
True</br>
False</i></table></details>


<details align="justify"> <summary><b>Tugas Praktek</b></br>Aku mengeklik dokumen PENGOLAHAN DATA TEKS. Di dalamnya aku diminta untuk meneliti popularitas antara buah salak dan buah jeruk berdasarkan judul artikel yang muncul di majalah Buah Sehat. Aku mulai menyiapkan susunan kodeku:</br></br>judul_artikel = [
"Buah Salak Baik untuk Mata", "Buah Salak Kaya Potasium", 
"Buah Jeruk Kaya Vitamin C", "Buah Salak Kaya Manfaat", 
"Salak Baik untuk Jantung", "Jeruk dapat Memperkuat Tulang", 
"Jeruk Mencegah Penyakit Asma", "Jeruk Memperkuat Gigi", 
"Jeruk Mencegah Kolesterol Jahat", "Salak Mencegah Diabetes", 
"Salak Memperkuat Dinding Usus", "Salak Baik untuk Darah",
"Jeruk Kaya Manfaat untuk Jantung", "Salak si Kecil yang Baik", 
"Jeruk dan Salak Buah Kaya Manfaat", "Buah Jeruk Enak",
"Tips Panen Jeruk Ribuan Kilo", "Tips Bertanam Salak", 
"Salak Manis untuk Berbuka", "Jeruk Baik untuk Wajah"
]</br>
jumlah_artikel_jeruk = 0</br>
jumlah_artikel_salak = 0</br>
for judul in judul_artikel:</br>
    if judul.count("Jeruk") > 0: </br>
        jumlah_artikel_jeruk += 1</br>
    if judul.count("Salak") > 0:</br>
        jumlah_artikel_salak += 1</br>
print(jumlah_artikel_jeruk) </br>
print(jumlah_artikel_salak)</br></br>
</summary><table align="justify"><i>Output : </br>10</br>
11 </i></table></details>

<details align="justify"> <summary><b>Tugas Praktek</b></br>Dengan cepat, aku mendeklarasikan daftar bernama kata_positif yang berisi nuansa kata positif untuk menghitung jumlah kemunculan kata_positif bagi tiap artikel jeruk dan salak</br></br>judul_artikel = [
"Buah Salak Baik untuk Mata", "Buah Salak Kaya Potasium", 
"Buah Jeruk Kaya Vitamin C", "Buah Salak Kaya Manfaat", 
"Salak Baik untuk Jantung", "Jeruk dapat Memperkuat Tulang", 
"Jeruk Mencegah Penyakit Asma", "Jeruk Memperkuat Gigi", 
"Jeruk Mencegah Kolesterol Jahat", "Salak Mencegah Diabetes", 
"Salak Memperkuat Dinding Usus", "Salak Baik untuk Darah",
"Jeruk Kaya Manfaat untuk Jantung", "Salak si Kecil yang Baik", 
"Jeruk dan Salak Buah Kaya Manfaat", "Buah Jeruk Enak",
"Tips Panen Jeruk Ribuan Kilo", "Tips Bertanam Salak", 
"Salak Manis untuk Berbuka", "Jeruk Baik untuk Wajah"
]</br>
kata_positif = ["Kaya", "Baik", "Mencegah", "Memperkuat"]</br>
kata_positif_jeruk = 0</br>
kata_positif_salak = 0</br>
for judul in judul_artikel: </br>
    for kata in kata_positif:</br>
        if judul.count("Jeruk") > 0 and judul.count(kata) > 0: </br>
            kata_positif_jeruk += 1</br>
        if judul.count("Salak") > 0 and judul.count(kata) > 0:</br>
            kata_positif_salak += 1</br>
print(kata_positif_jeruk) </br>
print(kata_positif_salak)</br></br>
</summary><table align="justify"><i>Output : </br>8</br>
9</i></table></details>

<p align="justify"><b>Function </b>adalah sebuah blok statemen yang hanya akan dijalankan saat ia dipanggil. Secara tidak sadar, selama proses belajar ini, aku telah mencoba menggunakan fungsi-fungsi dalam bahasa pemrograman Python.Fungsi len() untuk mengukur jumlah elemen dalam sebuah list dan fungsi print() untuk menampilkan pesan pada layar konsol merupakan contoh dari bentuk fungsi yang telah disediakan oleh bahasa pemrograman Python atau dengan kata lain built-in functions. Selain fungsi yang telah disediakan oleh Python, Python mengizinkan aku untuk mendeklarasikan fungsi dalam kode yang aku tuliskan yang dikenal dengan user defined function.</br></br><i>
  def nama_fungsi(argument):</br>
    statement_1</br>
    …</br>
    statement_n</br>
    return returned_value</br></i></p>
 
 Aku menuliskan dalam catatanku:
<ol><li>nama_fungsi adalah nama untuk fungsi yang Anda definisikan, memiliki aturan seperti penamaan variabel</li>
<li>argument adalah variabel masukan ke fungsi, bisa tanpa variabel, satu variabel atau lebih</li>
<li>statement_1 … statement_n adalah algoritma yang telah Anda transfer dalam bahasa Python yang merupakan inti dari fungsi yang Anda definisikan. Seluruh statement adalah menjorok (indent) ke dalam seperti yang pernah Anda pelajari pada conditioning dan looping</li>
<li>return_value adalah variabel output dari fungsi Anda, bisa tanpa variabel, satu variabel atau lebih.</li></ol>

<details align="justify"> <summary><b>Fungsi Pertama</b></br>contoh_fungsi merupakan nama dari fungsi yang aku deklarasikan dan statemen-statemen di dalamnya disebut sebagai isi (body) dari fungsi.</br></br>#Definisikan fungsi</br>
def contoh_fungsi():</br>
    print("Halo Dunia")</br>
    print("Aku sedang belajar bahasa Python")</br>
#Panggil fungsi yang telah didefinisikan</br>
contoh_fungsi()</br></br>
</summary><table align="justify"><i>Output : </br>Halo Dunia</br>
Aku sedang belajar bahasa Python</i></table></details>


<details align="justify"> <summary><b>Fungsi Kedua</b></br>fungsi_dengan_argumen membutuhkan dua argumen (nama_depan, nama_belakang).
Python akan menjalankan sebuah fungsi hanya ketika aku telah mensuplai jumlah argumen yang sesuai saat fungsi didefinisikan.</br></br>
#Definsikan fungsi </br>
def fungsi_dengan_argumen(nama_depan, nama_belakang):</br>
    print(nama_depan+" "+nama_belakang)</br>
#Panggil fungsi dengan memasukkan argumen</br>
#nama_depan yaitu "John" dan nama_belakang "Doe"</br>
fungsi_dengan_argumen("John", "Doe")</br></br>
</summary><table align="justify"><i>Output : </br>John Doe</i></table></details>

<details align="justify"> <summary><b>Fungsi Ketiga</b></br>Argumen nama_belakang menjadi bersifat opsional, saat fungsi dipanggil, jika argumen kedua tidak disuplai Python akan secara otomatis menset argumen nama_belakang menjadi string kosong - empty string ("").</br></br> #Definsikan fungsi dengan nilai default argument kedua adalah "".</br>
def fungsi_dengan_argumen(nama_depan, nama_belakang = ""):</br>
	print(nama_depan+" "+nama_belakang)</br>
#Panggil fungsi dengan memasukkan argumen nama_depan "John"</br>
fungsi_dengan_argumen("John")</br>
#Panggil fungsi dengan memasukkan argumen</br>
#nama_depan yaitu "John" dan nama_belakang "Doe"</br>
fungsi_dengan_argumen("John", "Doe")</br></br>
</summary><table align="justify"><i>Output : </br>John </br>
John Doe</i></table></details>


<details align="justify"> <summary><b>Tugas Praktek</b></br><i>#Dua buah data yang tersimpan dalam tipe list</br>
data1 = [70, 70, 70, 100, 100, 100, 120, 120, 150, 150]</br>
data2 = [50, 60, 60, 50, 70, 70, 100, 80, 100, 90]</br>
#Definisikan fungsi hitng_rata_rata</br>
def hitung_rata_rata(data):</br>
    jumlah = 0</br>
    for item in data:</br>
        jumlah += item</br>
    rata_rata = jumlah/len(data)</br>
    return rata_rata</br>
#Hitung nilai rata-rata dari kedua data yang dimiliki</br>
print('Rata-rata data1:')</br>
print(hitung_rata_rata(data1))</br>
print('Rata-rata data2:')</br>
print(hitung_rata_rata(data2))</br></i>
</summary><table align="justify"><i>Output : </br>Rata-rata data1:</br>
105.0</br>
Rata-rata data2:</br>
73.0 </i></table></details>

<details align="justify"> <summary><b>Tugas Praktek</b></br>fungsi untuk menghitung standar deviasi data dari data yang sudah saya berikan tadi (data dalam list of numeric bertipe int atau float).</br></br>#Dua buah data yang tersimpan dalam tipe list</br>
data1 = [70, 70, 70, 100, 100, 100, 120, 120, 150, 150]</br>
data2 = [50, 60, 60, 50, 70, 70, 100, 80, 100, 90]</br>
#Fungsi rata-rata data</br>
def hitung_rata_rata(data):</br>
    jumlah = 0</br>
    for item in data:</br>
        jumlah += item</br>
    rata_rata = jumlah/len(data)</br>
    return rata_rata</br>
#Definisikan fungsi hitung_standar_deviasi</br>
def hitung_standar_deviasi(data):</br>
    rata_rata_data = hitung_rata_rata(data)</br>
    varians = 0</br>
    for item in data:</br>
        varians += (item - rata_rata_data)**2</br>
        varians /= len(data)</br>
    standar_deviasi = varians ** (1/2)</br>
    return standar_deviasi</br>
#Hitung nilai standar deviasi dari kedua data yang dimiliki</br>
print('Standar deviasi data1:')</br>
print(hitung_standar_deviasi(data1))</br>
print('Standar deviasi data2:')</br>
print(hitung_standar_deviasi(data2))</br></br>
</summary><table align="justify"><i>Output : </br>Standar deviasi data1:</br>
14.93311056335886</br>
Standar deviasi data2:</br>
6.025948374480153</i></table></details>

<details align="justify"> <summary><b>Tugas Praktek</b></br><i># Data properti</br>
tabel_properti = {</br>
'luas_tanah': [70, 70, 70, 100, 100, 100, 120, 120, 150, 150],</br>
'luas_bangunan': [50, 60, 60, 50, 70, 70, 100, 80, 100, 90],</br>
'jarak': [15, 30, 55, 30, 25, 50, 20, 50, 50, 15],</br>
'harga': [500, 400, 300, 700, 1000, 650, 2000, 1200, 1800, 3000]</br>
}</br>
#Fungsi rata-rata data</br>
def hitung_rata_rata(data):</br>
    jumlah = 0</br>
    for item in data:</br>
        jumlah += item</br>
    rata_rata = jumlah/len(data)</br>
    return rata_rata</br>
#Fungsi hitung_standar_deviasi</br>
def hitung_standar_deviasi(data):</br>
    rata_rata_data = hitung_rata_rata(data)</br>
    varians = 0</br>
    for item in data:</br>
        varians += (item - rata_rata_data) ** 2</br>
        varians /= len(data)</br>
    standar_deviasi = varians ** (1/2)</br>
    return standar_deviasi</br>
#Definisikan fungsi untuk menghitung rata-rata dan standar deviasi</br>
#setiap kolom pada tabel_properti yang diberikan oleh key dict.</br>
def deskripsi_properti(tabel):</br>
    for key in tabel.keys():</br>
        print('Rata-rata ' + key + ':')</br>
        print(hitung_rata_rata(tabel[key])) </br>
        print('Standar deviasi ' + key + ':')</br>
        print(hitung_standar_deviasi(tabel[key]))</br>
        print('')</br>
#Panggil fungsi deskripsi_properti untuk menghitung rata-rata </br>
#dan standar deviasi setiap kolom pada tabel_properti</br>
deskripsi_properti(tabel_properti)</i></br></br>
</summary><table align="justify"><i>Output : </br>Rata-rata luas_bangunan:</br>
73.0</br>
Standar deviasi luas_bangunan:</br>
6.025948374480153</br>
Rata-rata luas_tanah:</br>
105.0</br>
Standar deviasi luas_tanah:</br>
14.93311056335886</br>
Rata-rata harga:</br>
1155.0</br>
Standar deviasi harga:</br>
587.0594351517378</br>
Rata-rata jarak:</br>
34.0</br>
Standar deviasi jarak:</br>
6.24005184770928</i></table></details>

<details align="justify"> <summary><b>Membaca Berkas Teks – Part 1</b></br>Setelah mempelajari bagaimana membuka/ membuat sebuah berkas teks dalam Python, aku akan mempelajari sintaks untuk dapat membaca isi dari sebuah berkas. Untuk membaca isi dari sebuah teks aku dapat menggunakan potongan kode berikut.</br></br>#Membaca file hello.txt dengan fungsi read()</br>
print(">>> Membaca file hello.txt dengan fungsi read()")</br>
file = open("hello.txt", "r")</br>
content = file.read()</br>
file.close()</br>
print(content)</br>
#Membaca file hello.txt dengan fungsi readline()</br>
print(">>> Membaca file hello.txt dengan fungsi readline()")</br>
file = open("hello.txt", "r")</br>
first_line = file.readline()</br>
second_line = file.readline()</br>
file.close()</br>
print(first_line)</br>
print(second_line)</br>
</summary><table align="justify"><i>Output : </br>>>> Membaca file hello.txt dengan fungsi read()</br>
Sekarang kita belajar menulis dengan menggunakan PythonMenulis konten file dengan mode w(write).Sekarang kita belajar menulis dengan menggunakan PythonMenulis konten file dengan mode a (append).</br>
>>> Membaca file hello.txt dengan fungsi readline()</br>
Sekarang kita belajar menulis dengan menggunakan PythonMenulis konten file dengan mode w(write).Sekarang kita belajar menulis dengan menggunakan PythonMenulis konten file dengan mode a (append).</i></table></details>


<details align="justify"> <summary><b>Membaca Berkas Teks – Part 2(</b></br>https://academy.dqlab.id/main/livecode/160/299/1382)</br>
#Membaca file hello.txt dengan fungsi readlines()</br>
print(">>> Membaca file hello.txt dengan fungsi readlines()")</br>
file = open("hello.txt", "r")</br>
all_lines = file.readlines()</br>
file.close()</br>
print(all_lines)</br>
#Membaca file hello.txt dengan menerapkan looping</br>
print(">>> Membaca file hello.txt dengan menerapkan looping")</br>
file = open("hello.txt", "r")</br>
for line in file:</br>
    print(line)</br></br>
  </summary><table align="justify"><i>Output : </br>
>>> Membaca file hello.txt dengan fungsi readlines()</br>
['Sekarang kita belajar menulis dengan menggunakan PythonMenulis konten file dengan mode w(write).Sekarang kita belajar menulis dengan menggunakan PythonMenulis konten file dengan mode a (append).']</br>
>>> Membaca file hello.txt dengan menerapkan looping</br>
Sekarang kita belajar menulis dengan menggunakan PythonMenulis konten file dengan mode w(write).Sekarang kita belajar menulis dengan menggunakan PythonMenulis konten file dengan mode a (append).</i></table></details>

<details align="justify"> <summary><b>Menulis Berkas Teks – Part 1</b></br>(https://academy.dqlab.id/main/livecode/160/299/1383)</br>Untuk menuliskan isi dari suatu berkas, aku dapat menggunakan fungsi write() atau writelines() yang telah disediakan oleh Python. Sebelum masuk ke dalam contoh penggunaan fungsi write() atau writelines(), penting bagiku untuk mengingat bahwa mode yang aku spesifikasikan pada fungsi open() akan mempengaruhi bagaimana Python menuliskan isi ke dalam berkas teks. Jika aku menggunakan mode "w", maka Python akan menghapus seluruh isi dalam berkas sebelum menuliskan konten yang aku spesifikasikan.</br></br>
#Menulis ke file hello_write.txt</br>
file = open("hello.txt", "w")</br>
file.write("Sekarang kita belajar menulis dengan menggunakan Python")</br>
file.write("Menulis konten file dengan mode w (write).")</br>
file.close()</br></summary><table align="justify"><i>Output : </br>Sekarang kita belajar menulis dengan menggunakan Python</br>
Menulis konten file dengan mode w (write).</br></i>
</table></details>

<details align="justify"> <summary><b>Menulis Berkas Teks – Part 2</b></br>https://academy.dqlab.id/main/livecode/160/299/1384)</br>Ketika aku menulis pada berkas teks menggunakan mode "a", Python tidak akan menghapus isi dalam berkas dan hanya akan menambahkan konten. Aku mempelajari contoh berikut untuk memahami penggunaan fungsi write() dan writelines()</br>Untuk membuka/membuat sebuah berkas teks dengan menggunakan mode “a”, untuk menambahkan beberapa baris pada berkas teks setelah isi dari berkas awalnya</br></br>
#Menulis ke file dengan mode append</br>
file = open("hello.txt", "a")</br>
file.writelines([</br>
"Sekarang kita belajar menulis dengan menggunakan Python", </br>
"Menulis konten file dengan mode a (append)."</br>
])</br>
file.close()</br>
</summary><table align="justify"><i>Output : </br>
In [1]: # Menulis ke file dengan mode append</br>
        file = open("hello.txt", "a")</br>
        file.writelines([</br>
        "Sekarang kita belajar menulis dengan menggunakan Python",</br> 
        "Menulis konten file dengan mode a (append)."])</br>
        file.close()</i></table></details>


<details align="justify"> <summary><b>Fungsi dalam Library Matematika – Part 1]</b></br>(https://academy.dqlab.id/main/livecode/160/299/1388)
#Import library math</br>
import math</br>
#Fungsi math.ceil()</br>
print(">>> Fungsi math.ceil()")</br>
x = 10.32</br>
y = 13.87</br>
x_ceil = math.ceil(x)</br>
y_ceil = math.ceil(y)</br>
print(x_ceil)</br>
print(y_ceil)</br>
#Fungsi math.floor()</br>
print(">>> Fungsi math.floor()")</br>
x_floor = math.floor(x)</br>
y_floor = math.floor(y)</br>
print(x_floor)</br>
print(y_floor)</br>
#Fungsi math.fabs()</br>
print(">>> Fungsi math.fabs()")</br>
x = 10.32</br>
y = -13.87</br>
x = math.fabs(x)</br>
y = math.fabs(y)</br>
print(x)</br>
print(y)</br>
#Fungsi math.factorial()</br>
print(">>> Fungsi math.factorial()")</br>
x_factorial = math.factorial(5)</br>
print(x_factorial)</br>
#Fungsi math.fsum()</br>
print(">>> Fungsi math.fsum()")</br>
x = [1, 2, 3, 4, 5, 6, -6, -5, -4]</br>
total = math.fsum(x)</br>
print(total)</br>
</summary><table align="justify"><i>Output : </br>
>>> Fungsi math.ceil()</br>
11</br>
14</br>
>>> Fungsi math.floor()</br>
10</br>
13</br>
>>> Fungsi math.fabs()</br>
10.32</br>
13.87</br>
>>> Fungsi math.factorial()</br>
120</br>
>>> Fungsi math.fsum()</br>
6.0</i></table></details>

<details align="justify"> <summary><b>Fungsi dalam Library Matematika – Part 2</b></br>https://academy.dqlab.id/main/livecode/160/299/1389</br>
import math</br>
x = [2.22,-3.33,4.44,-5.55]</br>
total = 0</br>
for i in x:</br>
    total += math.ceil(i)</br>
print(total)</br>
</summary><table align="justify"><i>Output : </br>>>> Fungsi math.log()</br>
3.0</br>
4.0</br>
4.0</br>
>>> Fungsi math.sqrt()</br>
10.0</br>
1.4142135623730951</br>
>>> Fungsi math.copysign()</br>
-10.32</br>
-13.87</br>
15.0</i></table></details>

<details align="justify"> <summary><b>Harga Rumah di Tangerang</b></br>https://academy.dqlab.id/main/livecode/160/303/1392</brKita diminta untuk mengembangkan model prediksi harga rumah di di Tangerang berdasarkan luas tanah, luas bangunan serta kedekatan lokasi dengan pusat kota.</br></br>
#STEP 1: </br>
#Baca file "harga_rumah.txt"</br>
file_harga_rumah = open("harga_rumah.txt", "r")</br>
data_harga_rumah = file_harga_rumah.readlines()</br>
file_harga_rumah.close()</br>
#Buat list of dict dengan nama harga rumah</br>
key_harga_rumah = data_harga_rumah[0].replace("\n","").split(",")</br>
harga_rumah = []</br>
for baris in data_harga_rumah[1:]:</br>
	baris_harga_rumah = baris.replace("\n","").split(",")</br>
	dict_harga_rumah = dict()</br>
	for i in range(len(baris_harga_rumah)):</br>
		dict_harga_rumah[key_harga_rumah[i]] = baris_harga_rumah[i]</br>
	harga_rumah.append(dict_harga_rumah)</br>
print(harga_rumah)</br>
#STEP 2:
#Buat fungsi  get_all_specified_attribute yang menerima parameter list_of_dictionary </br>
#(tipe data list yang berisikan sekumpulan tipe data dictionary) dan specified_key </br>
#(tipe data string). Fungsi akan mengembalikan sebuah list yang berisikan seluruh </br>
#atribut dengan kunci (key) specified_key. </br>
def get_all_specified_attributes(list_of_dictionary, specified_key):</br>
	list_attributes = []</br>
	for data in list_of_dictionary:</br>
		attribute = data[specified_key]</br>
		list_attributes.append(attribute)</br>
	return list_attributes</br>
#STEP 3: </br>
#Buat fungsi fungsi min_value yang menerima parameter list_attributes (berupa </br>
#tipe data list) dan mengembalikan nilai terkecil dalam list_attributes </br>
def min_value(list_attributes):</br>
	min_attribute = 9999</br>
	for attr in list_attributes:</br>
		if int(attr) < min_attribute:</br>
			min_attribute = int(attr)</br>
	return min_attribute</br>
#Buat fungsi dan max_value yang menerima parameter list_attribute dan </br>
#mengembalikan nilai terbesar dalam list_attributes.	</br>
def max_value(list_attributes):</br>
	max_attribute = -9999</br>
	for attr in list_attributes:</br>
		if int(attr) > max_attribute:</br>
			max_attribute = int(attr)</br>
	return max_attribute</br>
#STEP 4: </br>
#Buat fungsi transform_attribute yang menerima parameter attr (sebuah </br>
#bilangan), max_attr (sebuah bilangan) dan min_attr (sebuah bilangan) </br>
#yang mengembalikan nilai transformasi dari sebuah attribute.</br>
def transform_attribute(attr, max_attr, min_attr):</br>
	nilai_transformasi = (attr - min_attr) / (max_attr - min_attr)</br>
	return nilai_transformasi</br>
#STEP 5:</br>
#Buat fungsi data_transformation yang menerima parameter list_of_dictionary </br>
#(sebuah list yang berisikan tipe data dictionary) dan list_attribute_names </br>
#(sebuah list yang berisikan tipe data string) mengembalikan hasil </br>
#transformasi data dari list_of_dictionary berdasarkan list_attribute_names </br>
#dan attr_info telah dispesifikasikan.</br>
def data_transformation(list_of_dictionary, list_attribute_names):</br>
	attr_info = {}</br>
	for attr_name in list_attribute_names:</br>
		specified_attributes = get_all_specified_attributes(list_of_dictionary, attr_name)</br>
		max_attr = max_value(specified_attributes)</br>
		min_attr = min_value(specified_attributes)</br>
		attr_info[attr_name] = {'max': max_attr, 'min': min_attr}</br>
		data_idx = 0</br>
		while(data_idx < len(list_of_dictionary)):</br>
			list_of_dictionary[data_idx][attr_name] = transform_attribute(int(list_of_dictionary[data_idx][attr_name]), max_attr, min_attr)</br>
			data_idx += 1</br>
	return list_of_dictionary, attr_info</br>
#STEP 6:</br>
#Berdasarkan data baru dan attr_info ini, buat fungsi transform_data yang</br>
#menerima parameter data dan attr_info dan mengembalikan nilai atribut </br>
#dari data baru yang telah ditransformasikan.</br>
def transform_data(data, attr_info):</br>
	for key_name in data.keys():</br>
		data[key_name] = (data[key_name] - attr_info[key_name]['min']) / (</br>
		                  attr_info[key_name]['max'] - attr_info[key_name]['min'])</br>
	return data</br>
#STEP 7:</br>
#Buat fungsi yang digunakan untuk sistem prediksi harga berdasarkan </br>
#nilai kemiripan atribut, yaitu argument input data dan list_of_data!</br>
def abs_value(value):</br>
	if value < 0:</br>
		return -value</br>
	else:</br>
		return value</br>
def price_based_on_similarity(data, list_of_data):</br>
	prediksi_harga = 0</br>
	perbedaan_terkecil = 999</br>
	for data_point in list_of_data:</br>
		perbedaan= abs_value(data['tanah'] - data_point['tanah'])</br>
		perbedaan+= abs_value(data['bangunan'] - data_point['bangunan'])</br>
		perbedaan+= abs_value(data['jarak_ke_pusat'] - data_point['jarak_ke_pusat'])</br>
		if perbedaan < perbedaan_terkecil:</br>
			prediksi_harga = data_point['harga']</br>
			perbedaan_terkecil = perbedaan</br>
	return prediksi_harga</br>
#STEP 8:</br>
#Hitung harga rumah yang telah ditransformasikan ke dalam variabel </br>
#harga_rumah berikut dengan atributnya attr_info</br>
harga_rumah, attr_info = data_transformation(harga_rumah,['tanah','bangunan','jarak_ke_pusat'])</br>
#Gunakan variabel data untuk memprediksi harga rumah</br>
data = {'tanah': 110, 'bangunan': 80, 'jarak_ke_pusat': 35}</br>
#Transformasikan data tersebut dengan dengan menggunakan attr_info yang telah </br>
#diperoleh yang kembali disimpan ke variabel data.</br>
data = transform_data(data, attr_info)</br>
#Hitunglah prediksi harga dari variabel data tersebut.</br>
harga = price_based_on_similarity(data, harga_rumah)</br>
print("Prediksi harga rumah: ", harga)</br>
