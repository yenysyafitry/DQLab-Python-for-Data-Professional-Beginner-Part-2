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

<details align="justify"> <summary><b> List Manipulation – Part 1 </b></br>Untuk memanipulasi tipe data list, aku dapat menggunakan sekumpulan fitur yang telah tersedia dalam bahasa pemrograman Python. Merujuk pada tabel di bawah, aku dapat memahami fitur-fitur untuk melakukan manipulasi data yang terdiri atas append(), clear(), copy(), count() dan extend()</br><img src="https://github.com/yenysyafitry/DQLab-Python-for-Data-Professional-Beginner-Part-2/blob/main/download.png">
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

<details align="justify"> <summary><b>  </b></br>
</summary><table align="justify"><i>Output : </br>H</i></table></details>

<details align="justify"> <summary><b>  </b></br>
</summary><table align="justify"><i>Output : </br>H</i></table></details>


<details align="justify"> <summary></br>
</summary><table align="justify"><i>Output : </br>H</i></table></details>

<details align="justify"> <summary></br>
</summary><table align="justify"><i>Output : </br>H</i></table></details>

<details align="justify"> <summary></br>
</summary><table align="justify"><i>Output : </br>H</i></table></details>
