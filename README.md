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

<details align="justify"> <summary><b>  </b></br>
</summary><table align="justify"><i>Output : </br>H</i></table></details>

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
