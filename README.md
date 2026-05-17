<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Sistem Mandiri Perpustakaan Faith</title>
</head>
<body>

    <!-- JUDUL UTAMA -->
    <h1>PERPUSTAKAAN FAITH</h1>
    <p>Selamat datang di Layanan Mandiri Layar Sentuh.</p>
    <hr>

    <!-- MENU UTAMA PILIHAN -->
    <h3>Silakan pilih layanan:</h3>
    <ul>
        <li><a href="#peminjaman">Pilihan 1: Meminjam Buku</a></li>
        <li><a href="#pengembalian">Pilihan 2: Mengembalikan Buku</a></li>
    </ul>
    
    <hr>

    <!-- JALUR A: FORM PEMINJAMAN -->
    <div id="peminjaman">
        <h2>Form Peminjaman Buku</h2>
        <form action="#" method="get">
            <p>
                <label>Nama Lengkap:</label><br>
                <input type="text" name="nama_peminjam" placeholder="Masukkan nama lengkap" required>
            </p>
            <p>
                <label>Alamat:</label><br>
                <input type="text" name="alamat_peminjam" placeholder="Masukkan alamat lengkap" required>
            </p>
            <p>
                <label>Buku yang Ingin Dipinjam:</label><br>
                <input type="text" name="buku_dipinjam" placeholder="Masukkan judul buku" required>
            </p>
            <p>
                <button type="submit">Konfirmasi Pinjam (Peminjaman Berhasil jika Buku Tersedia)</button>
            </p>
        </form>
        <p><em>*Catatan: Batas waktu peminjaman di Perpustakaan Faith adalah 7 hari.</em></p>
    </div>

    <hr>

    <!-- JALUR B: FORM PENGEMBALIAN -->
    <div id="pengembalian">
        <h2>Form Pengembalian Buku</h2>
        <form action="#" method="get">
            <p>
                <label>Nama Lengkap:</label><br>
                <input type="text" name="nama_pengembali" placeholder="Masukkan nama lengkap" required>
            </p>
            <p>
                <label>Buku yang Dipulangkan:</label><br>
                <input type="text" name="buku_dikembalikan" placeholder="Masukkan judul buku" required>
            </p>
            <p>
                <label>Lama Waktu Peminjaman (Hari):</label><br>
                <input type="number" name="durasi_pinjam" min="1" placeholder="Contoh: 5 atau 10" required>
            </p>
            <p>
                <button type="submit">Konfirmasi Pemulangan Buku</button>
            </p>
        </form>
        
        <h3>Aturan Denda Perpustakaan Faith:</h3>
        <p>Jika pengembalian melewati batas 7 hari, akan dikenakan denda sebesar <strong>Rp 3.000 per hari</strong> dan dianjurkan untuk langsung membayar denda di mesin/kasir. Jika kurang dari atau sama dengan 7 hari, cukup isi nama dan judul buku saja.</p>
    </div>

    <hr>
    <p><a href="#">Kembali ke Menu Utama Atas</a></p>

</body>
</html>
