<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sistem Mandiri Perpustakaan Faith</title>
    <style>
        * {
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        body {
            background-color: #f4f6f9;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
        }
        .container {
            background-color: #ffffff;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 8px 24px rgba(0,0,0,0.1);
            width: 100%;
            max-width: 500px;
            text-align: center;
            border-top: 6px solid #2c3e50;
        }
        h2 {
            color: #2c3e50;
            margin-bottom: 5px;
            text-transform: uppercase;
        }
        .sub-title {
            color: #7f8c8d;
            font-size: 14px;
            margin-bottom: 25px;
        }
        
        /* Navigasi Menu Utama Menggunakan Sistem Anchor HTML */
        .menu-utama {
            display: flex;
            gap: 15px;
            margin-bottom: 25px;
        }
        .tombol-menu {
            flex: 1;
            padding: 12px;
            font-size: 15px;
            font-weight: bold;
            color: white;
            text-decoration: none;
            border-radius: 8px;
            transition: 0.2s;
        }
        .bg-biru { background-color: #3498db; }
        .bg-biru:hover { background-color: #2980b9; }
        .bg-hijau { background-color: #2ecc71; }
        .bg-hijau:hover { background-color: #27ae60; }

        /* Mengatur tampilan form agar berganti sesuai target ID HTML */
        .form-section {
            display: none; /* Tersembunyi di awal */
            text-align: left;
            background: #fdfdfd;
            padding: 20px;
            border: 1px solid #e2e8f0;
            border-radius: 8px;
            margin-top: 15px;
        }
        /* Logika murni HTML (:target) untuk memunculkan form tanpa JavaScript */
        .form-section:target {
            display: block;
        }
        
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: 600;
            color: #4a5568;
        }
        input[type="text"], input[type="number"] {
            width: 100%;
            padding: 10px;
            border: 1px solid #cbd5e1;
            border-radius: 6px;
            font-size: 14px;
        }
        .btn-submit {
            background-color: #2c3e50;
            color: white;
            width: 100%;
            padding: 12px;
            font-size: 16px;
            font-weight: bold;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            margin-top: 10px;
        }
        .btn-submit:hover {
            background-color: #1a252f;
        }
        
        .info-box {
            background-color: #eff6ff;
            border-left: 4px solid #3b82f6;
            padding: 12px;
            font-size: 13px;
            color: #1e3a8a;
            margin-top: 15px;
            border-radius: 0 6px 6px 0;
        }
        .info-box ul {
            margin: 5px 0 0 0;
            padding-left: 20px;
        }
    </style>
</head>
<body>

<div class="container">
    <h2>Perpustakaan Faith</h2>
    <div class="sub-title">Layanan Mandiri Layar Sentuh</div>
    <p>Silakan klik layanan di bawah ini:</p>
    
    <!-- MENU UTAMA MURNI LINK HTML -->
    <div class="menu-utama">
        <a href="#layanan-peminjaman" class="tombol-menu bg-biru">Meminjam Buku</a>
        <a href="#layanan-pengembalian" class="tombol-menu bg-hijau">Mengembalikan Buku</a>
    </div>

    <!-- JALUR A: FORM PEMINJAMAN MURNI HTML -->
    <div id="layanan-peminjaman" class="form-section">
        <h3>Form Peminjaman Buku</h3>
        <form action="#" method="get">
            <div class="form-group">
                <label>Nama Lengkap</label>
                <input type="text" placeholder="Masukkan nama lengkap Anda" required>
            </div>
            <div class="form-group">
                <label>Alamat</label>
                <input type="text" placeholder="Masukkan alamat tinggal" required>
            </div>
            <div class="form-group">
                <label>Judul Buku</label>
                <input type="text" placeholder="Masukkan judul buku yang ingin dipinjam" required>
            </div>
            <button type="submit" class="btn-submit">Proses Peminjaman Berhasil</button>
        </form>
        <div class="info-box">
            *Ketentuan: Jika buku tersedia di rak, peminjaman sukses (Maksimal 7 hari).
        </div>
    </div>

    <!-- JALUR B: FORM PENGEMBALIAN MURNI HTML -->
    <div id="layanan-pengembalian" class="form-section">
        <h3>Form Pengembalian Buku</h3>
        <form action="#" method="get">
            <div class="form-group">
                <label>Nama Lengkap</label>
                <input type="text" placeholder="Masukkan nama Anda" required>
            </div>
            <div class="form-group">
                <label>Judul Buku</label>
                <input type="text" placeholder="Judul buku yang dipulangkan" required>
            </div>
            <div class="form-group">
                <label>Lama Pinjam (Hari)</label>
                <input type="number" min="1" placeholder="Contoh: 5 atau 10" required>
            </div>
            <button type="submit" class="btn-submit">Proses Pengembalian Berhasil</button>
        </form>
        <div class="info-box">
            <strong>Aturan Denda Perpustakaan Faith:</strong>
            <ul>
                <li>≤ 7 Hari = Bebas denda (Cukup masukkan Nama & Judul).</li>
                <li>> 7 Hari = Denda Rp3.000 / hari keterlambatan.</li>
            </ul>
        </div>
    </div>
</div>

</body>
</html>
            text-align: center;
            border-top: 6px solid #2c3e50;
        }
        h2 {
            color: #2c3e50;
            margin-bottom: 5px;
        }
        .sub-title {
            color: #7f8c8d;
            font-size: 14px;
            margin-bottom: 25px;
        }
        .btn-group {
            display: flex;
            gap: 15px;
            margin-bottom: 25px;
        }
        button {
            flex: 1;
            padding: 12px;
            font-size: 16px;
            font-weight: bold;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: 0.2s;
        }
        .btn-primary { background-color: #3498db; color: white; }
        .btn-primary:hover { background-color: #2980b9; }
        .btn-success { background-color: #2ecc71; color: white; }
        .btn-success:hover { background-color: #27ae60; }
        .btn-submit { background-color: #2c3e50; color: white; width: 100%; margin-top: 15px; }
        .btn-submit:hover { background-color: #1a252f; }
        
        .form-section {
            display: none;
            text-align: left;
            background: #fdfdfd;
            padding: 20px;
            border: 1px solid #e2e8f0;
            border-radius: 8px;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: 600;
            color: #4a5568;
        }
        input[type="text"], input[type="number"] {
            width: 100%;
            padding: 10px;
            border: 1px solid #cbd5e1;
            border-radius: 6px;
            font-size: 14px;
        }
        .result {
            margin-top: 20px;
            padding: 15px;
            border-radius: 8px;
            font-weight: bold;
            display: none;
            text-align: left;
            line-height: 1.5;
        }
        .success { background-color: #def7ec; color: #03543f; border: 1px solid #84e1bc; }
        .error { background-color: #fde8e8; color: #9b1c1c; border: 1px solid #f8b4b4; }
        .warning { background-color: #fef3c7; color: #92400e; border: 1px solid #fde68a; }
    </style>
</head>
<body>

<div class="container">
    <h2>PERPUSTAKAAN FAITH</h2>
    <div class="sub-title">Layanan Mandiri Layar Sentuh</div>
    <p>Silakan pilih layanan di bawah ini:</p>
    
    <div class="btn-group">
        <button class="btn-primary" onclick="tampilkanForm('pinjam')">Meminjam Buku</button>
        <button class="btn-success" onclick="tampilkanForm('kembali')">Mengembalikan Buku</button>
    </div>

    <!-- FORM PEMINJAMAN -->
    <div id="formPinjam" class="form-section">
        <h3>Form Peminjaman Buku</h3>
        <div class="form-group">
            <label>Nama Lengkap</label>
            <input type="text" id="namaPinjam" placeholder="Masukkan nama Anda">
        </div>
        <div class="form-group">
            <label>Alamat</label>
            <input type="text" id="alamatPinjam" placeholder="Masukkan alamat Anda">
        </div>
        <div class="form-group">
            <label>Judul Buku</label>
            <input type="text" id="bukuPinjam" placeholder="Contoh: Laskar Pelangi, Bumi Manusia">
        </div>
        <button class="btn-submit" onclick="prosesPinjam()">Konfirmasi Pinjam</button>
    </div>

    <!-- FORM PENGEMBALIAN -->
    <div id="formKembali" class="form-section">
        <h3>Form Pengembalian Buku</h3>
        <div class="form-group">
            <label>Nama Lengkap</label>
            <input type="text" id="namaKembali" placeholder="Masukkan nama Anda">
        </div>
        <div class="form-group">
            <label>Judul Buku</label>
            <input type="text" id="bukuKembali" placeholder="Judul buku yang dikembalikan">
        </div>
        <div class="form-group">
            <label>Durasi Peminjaman (Hari)</label>
            <input type="number" id="durasiPinjam" min="1" placeholder="Berapa hari buku dipinjam?">
        </div>
        <button class="btn-submit" onclick="prosesKembali()">Konfirmasi Pengembalian</button>
    </div>

    <!-- KOTAK NOTIFIKASI HASIL -->
    <div id="kotakHasil" class="result"></div>
</div>

<script>
    // Database simulasi status buku di Perpustakaan Faith
    let daftarBuku = {
        "laskar pelangi": true,
        "bumi manusia": false, 
        "aljabar linear": true,
        "fisika dasar": true
    };

    function tampilkanForm(jenis) {
        document.getElementById('formPinjam').style.style.display = 'none'; // Error diperbaiki di baris ini
        document.getElementById('formPinjam').style.display = 'none';
        document.getElementById('formKembali').style.display = 'none';
        document.getElementById('kotakHasil').style.display = 'none';

        if (jenis === 'pinjam') {
            document.getElementById('formPinjam').style.display = 'block';
        } else if (jenis === 'kembali') {
            document.getElementById('formKembali').style.display = 'block';
        }
    }

    function prosesPinjam() {
        let nama = document.getElementById('namaPinjam').value.trim();
        let alamat = document.getElementById('alamatPinjam').value.trim();
        let bukuInput = document.getElementById('bukuPinjam').value.trim();
        let bukuKey = bukuInput.toLowerCase();
        let kotakHasil = document.getElementById('kotakHasil');

        if (!nama || !alamat || !bukuInput) {
            alert("Harap isi semua kolom data peminjaman!");
            return;
        }

        kotakHasil.style.display = 'block';

        if (bukuKey in daftarBuku) {
            if (daftarBuku[bukuKey] === true) {
                kotakHasil.className = "result success";
                kotakHasil.innerHTML = `<strong>Peminjaman Berhasil!</strong><br>Halo ${nama}, buku "${bukuInput}" siap diambil. Batas pengembalian Perpustakaan Faith adalah 7 hari.`;
                daftarBuku[bukuKey] = false; 
            } else {
                kotakHasil.className = "result error";
                kotakHasil.innerHTML = `<strong>Peminjaman Gagal.</strong><br>Maaf ${nama}, buku "${bukuInput}" sedang dipinjam atau belum dipulangkan ke Perpustakaan Faith.`;
            }
        } else {
            kotakHasil.className = "result error";
            kotakHasil.innerHTML = `<strong>Peminjaman Gagal.</strong><br>Buku "${bukuInput}" tidak tersedia di koleksi Perpustakaan Faith.`;
        }
    }

    function prosesKembali() {
        let nama = document.getElementById('namaKembali').value.trim();
        let bukuInput = document.getElementById('bukuKembali').value.trim();
        let bukuKey = bukuInput.toLowerCase();
        let durasi = parseInt(document.getElementById('durasiPinjam').value);
        let kotakHasil = document.getElementById('kotakHasil');

        if (!nama || !bukuInput || isNaN(durasi)) {
            alert("Harap isi semua kolom data pengembalian!");
            return;
        }

        kotakHasil.style.display = 'block';
        let batasMaksimal = 7;
        let tarifDenda = 3000;

        if (durasi > batasMaksimal) {
            let hariTerlambat = durasi - batasMaksimal;
            let totalDenda = hariTerlambat * tarifDenda;
            
            kotakHasil.className = "result warning";
            kotakHasil.innerHTML = `<strong>Pemulangan Berhasil dengan Catatan!</strong><br>
                                    Halo ${nama}, Anda terlambat ${hariTerlambat} hari dari batas waktu Perpustakaan Faith.<br>
                                    <strong>Denda Anda: Rp ${totalDenda.toLocaleString('id-ID')}</strong><br>
                                    <em>Anjuran: Silakan lakukan pembayaran denda di mesin/kasir Perpustakaan Faith.</em>`;
        } else {
            kotakHasil.className = "result success";
            kotakHasil.innerHTML = `<strong>Pemulangan Berhasil!</strong><br>Terima kasih ${nama}, Anda telah mengembalikan buku "${bukuInput}" ke Perpustakaan Faith tepat waktu.`;
        }

        daftarBuku[bukuKey] = true;
    }
</script>

</body>
</html>
            text-align: center;
        }
        h2 {
            color: #2c3e50;
            margin-bottom: 20px;
        }
        .btn-group {
            display: flex;
            gap: 15px;
            margin-bottom: 25px;
        }
        button {
            flex: 1;
            padding: 12px;
            font-size: 16px;
            font-weight: bold;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: 0.2s;
        }
        .btn-primary { background-color: #3498db; color: white; }
        .btn-primary:hover { background-color: #2980b9; }
        .btn-success { background-color: #2ecc71; color: white; }
        .btn-success:hover { background-color: #27ae60; }
        .btn-submit { background-color: #2c3e50; color: white; width: 100%; margin-top: 15px; }
        .btn-submit:hover { background-color: #1a252f; }
        
        .form-section {
            display: none;
            text-align: left;
            background: #fdfdfd;
            padding: 20px;
            border: 1px solid #e2e8f0;
            border-radius: 8px;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: 600;
            color: #4a5568;
        }
        input[type="text"], input[type="number"] {
            width: 100%;
            padding: 10px;
            border: 1px solid #cbd5e1;
            border-radius: 6px;
            font-size: 14px;
        }
        .result {
            margin-top: 20px;
            padding: 15px;
            border-radius: 8px;
            font-weight: bold;
            display: none;
        }
        .success { background-color: #def7ec; color: #03543f; border: 1px solid #84e1bc; }
        .error { background-color: #fde8e8; color: #9b1c1c; border: 1px solid #f8b4b4; }
        .warning { background-color: #fef3c7; color: #92400e; border: 1px solid #fde68a; }
    </style>
</head>
<body>

<div class="container">
    <h2>Layar Sentuh Perpustakaan</h2>
    <p>Silakan pilih layanan di bawah ini:</p>
    
    <div class="btn-group">
        <button class="btn-primary" onclick="tampilkanForm('pinjam')">Meminjam Buku</button>
        <button class="btn-success" onclick="tampilkanForm('kembali')">Mengembalikan Buku</button>
    </div>

    <!-- FORM PEMINJAMAN -->
    <div id="formPinjam" class="form-section">
        <h3>Form Peminjaman</h3>
        <div class="form-group">
            <label>Nama Lengkap</label>
            <input type="text" id="namaPinjam" placeholder="Masukkan nama Anda">
        </div>
        <div class="form-group">
            <label>Alamat</label>
            <input type="text" id="alamatPinjam" placeholder="Masukkan alamat Anda">
        </div>
        <div class="form-group">
            <label>Judul Buku</label>
            <input type="text" id="bukuPinjam" placeholder="Contoh: Laskar Pelangi, Bumi Manusia">
        </div>
        <button class="btn-submit" onclick="prosesPinjam()">Konfirmasi Pinjam</button>
    </div>

    <!-- FORM PENGEMBALIAN -->
    <div id="formKembali" class="form-section">
        <h3>Form Pengembalian</h3>
        <div class="form-group">
            <label>Nama Lengkap</label>
            <input type="text" id="namaKembali" placeholder="Masukkan nama Anda">
        </div>
        <div class="form-group">
            <label>Judul Buku</label>
            <input type="text" id="bukuKembali" placeholder="Judul buku yang dikembalikan">
        </div>
        <div class="form-group">
            <label>Durasi Peminjaman (Hari)</label>
            <input type="number" id="durasiPinjam" min="1" placeholder="Berapa hari buku dipinjam?">
        </div>
        <button class="btn-submit" onclick="prosesKembali()">Konfirmasi Pengembalian</button>
    </div>

    <!-- KOTAK NOTIFIKASI HASIL -->
    <div id="kotakHasil" class="result"></div>
</div>

<script>
    // Database simulasi status buku (True = Tersedia, False = Tidak Tersedia)
    let daftarBuku = {
        "laskar pelangi": true,
        "bumi manusia": false, // Anggap sedang dipinjam orang lain
        "aljabar linear": true,
        "fisika dasar": true
    };

    function tampilkanForm(jenis) {
        // Sembunyikan semua form dan kotak hasil terlebih dahulu
        document.getElementById('formPinjam').style.display = 'none';
        document.getElementById('formKembali').style.display = 'none';
        document.getElementById('kotakHasil').style.display = 'none';

        // Tampilkan form yang dipilih
        if (jenis === 'pinjam') {
            document.getElementById('formPinjam').style.display = 'block';
        } else if (jenis === 'kembali') {
            document.getElementById('formKembali').style.display = 'block';
        }
    }

    function prosesPinjam() {
        let nama = document.getElementById('namaPinjam').value.trim();
        let alamat = document.getElementById('alamatPinjam').value.trim();
        let buku = document.getElementById('bukuPinjam').value.trim().toLowerCase();
        let kotakHasil = document.getElementById('kotakHasil');

        if (!nama || !alamat || !buku) {
            alert("Harap isi semua kolom data peminjaman!");
            return;
        }

        kotakHasil.style.display = 'block';

        if (buku in daftarBuku) {
            if (daftarBuku[buku] === true) {
                kotakHasil.className = "result success";
                kotakHasil.innerHTML = `Peminjaman Berhasil!<br>Halo ${nama}, buku siap diambil. Batas pengembalian adalah 7 hari.`;
                daftarBuku[buku] = false; // Status diubah jadi terpinjam
            } else {
                kotakHasil.className = "result error";
                kotakHasil.innerHTML = `Peminjaman Gagal.<br>Maaf ${nama}, buku tersebut sedang dipinjam atau belum dipulangkan.`;
            }
        } else {
            kotakHasil.className = "result error";
            kotakHasil.innerHTML = `Peminjaman Gagal.<br>Buku tidak tersedia di perpustakaan ini.`;
        }
    }

    function prosesKembali() {
        let nama = document.getElementById('namaKembali').value.trim();
        let buku = document.getElementById('bukuKembali').value.trim().toLowerCase();
        let durasi = parseInt(document.getElementById('durasiPinjam').value);
        let kotakHasil = document.getElementById('kotakHasil');

        if (!nama || !buku || isNaN(durasi)) {
            alert("Harap isi semua kolom data pengembalian!");
            return;
        }

        kotakHasil.style.display = 'block';
        let batasMaksimal = 7;
        let tarifDenda = 3000;

        if (durasi > batasMaksimal) {
            let hariTerlambat = durasi - batasMaksimal;
            let totalDenda = hariTerlambat * tarifDenda;
            
            kotakHasil.className = "result warning";
            kotakHasil.innerHTML = `Pemulangan Berhasil dengan Catatan!<br>
                                    Halo ${nama}, Anda terlambat ${hariTerlambat} hari.<br>
                                    <strong>Denda: Rp ${totalDenda.toLocaleString('id-ID')}</strong><br>
                                    <em>Anjuran: Silakan lakukan pembayaran denda di mesin/kasir.</em>`;
        } else {
            kotakHasil.className = "result success";
            kotakHasil.innerHTML = `Pemulangan Berhasil!<br>Terima kasih ${nama}, Anda mengembalikan buku tepat waktu.`;
        }

        // Kembalikan status ketersediaan buku ke sistem
        daftarBuku[buku] = true;
    }
</script>

</body>
</html>
