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
