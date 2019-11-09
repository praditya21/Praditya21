<head>
  <title>Tugas Ibu Novira</title>

  <body>

  <td><h3 align='center'>Data Mahasiswa <br> Kampus Akademi Komunitas </h3> </td><hr>

  <script type="text/javascript">
  function cek(){
    nim=document.getElementById('nim').value;
    nama=document.getElementById('nama').value;
    jenis=document.getElementById('jenis').value;
    agama=document.getElementById('agama').value;
    prodi=document.getElementById('prodi').value;
   komentar=document.getElementById('komentar').value;

   if(nim==''||nim==null){
      document.getElementById('e_nim').innerHTML="Harus diisi";
      return false;
      }

    if(nama==''||nama==null){
      document.getElementById('e_nama').innerHTML="Harus diisi";
      return false;
      }

    if(jenis=='-'||jenis==''||jenis==null){
      document.getElementById('e_jenis').innerHTML="Harus diisi";
      return false;
      }

    if(agama=='-'||agama==''||agama==null){
      document.getElementById('e_agama').innerHTML="Harus diisi";
      return false;
      }

      if(prodi=='-'||prodi==''||prodi==null){
      document.getElementById('e_prodi').innerHTML="Harus diisi";
      return false;
       }

    if(komentar==''||komentar==null){
      document.getElementById('e_komentar').innerHTML="Harus diisi";
      return false;
      }

  if(nim!=''&& nama!=''&& jenis!='-'&&  agama!='-' && prodi!='-'&& komentar!='') {
      document.getElementById('Hasil').innerHTML="Nim="+nim+"<br> Nama="+nama+"<br> Jenis_Kelamin="+jenis+"<br> Agama="+agama+" <br>Prodi="+prodi+"<br> Komentar="+komentar;
      return false;
    }
    }
      </script>
</head>

<body>
 <form id="latihan" onsubmit="return cek();" >
<table align="center">

<tr><td>Nim</td>
  <td><input type="text" id="nim"></td>
  <td> <div id="e_nim"></div> </td>  </tr><br>

<tr>
  <td> Nama </td>
  <td> <input type="text" id="nama"></td> 
  <td> <div id="e_nama"></div></td></tr><br>    

<tr><td>Jenis Kelamin </td>
  <td><select id="jenis">
  <option value="-">-pilih-</option>
  <option value="L">Laki-laki</option>
  <option value="P">Perempuan</option></td>
  </select> 
  <td><div id="e_jenis"></div></td></tr><br>

<tr>
  <td> Agama</td> 
  <td> <select id="agama">
  <option value = "-pilih-" /> pilih 
  <option value = "Islam" /> Islam 
  <option value = "Kristen" /> Kristen
  <option value = "Katolik" /> Katolik 
  <option value = "Budha" /> Budha
  <option value = "Hindu" /> Hindu </select>
  <div id="e_agama"></div></td></tr><br>

<tr> <td>Prodi </td>
  <td> <select id="prodi">
  <option value="-">-Pilih Prodi-</option>
  <option value="1">Sistem Informasi</option>
  <option value="Teknik Informatika">Teknik Informatika</option>
  <option value="3">Manajemen Informatika</option>
  <option value="4">Sistem Informatika</option>
  <option value="5">Teknik Komputer</option></td>
  </select>
  <td><div id="e_prodi"></div></td> </tr><br>

<tr><td>Komentar</td>
  <td> <textarea id="komentar" cols="15" rows="5"></textarea></td>
  <td> <div id="e_komentar"></div> </td></tr> <br>

 <tr>
<td><input type="submit" value="Ok"></td></tr>
<tr><td> <p id="Hasil">Silahkan diisi Form di atas</p></td> </tr> 
 </form>

</table>
</body>
</html>
