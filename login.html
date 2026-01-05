<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login | Jimpitan Digital</title>
    <style>
        :root { --accent: #00B894; --bg: #0F172A; }
        body { font-family: 'Inter', sans-serif; background: var(--bg); display: flex; justify-content: center; align-items: center; height: 100vh; margin: 0; color: white; }
        .card { background: rgba(30, 41, 59, 0.7); backdrop-filter: blur(10px); padding: 40px 30px; border-radius: 24px; border: 1px solid rgba(255,255,255,0.1); width: 100%; max-width: 320px; text-align: center; }
        input { width: 100%; padding: 15px; margin: 10px 0; border-radius: 12px; border: 1px solid #334155; background: #1E293B; color: white; font-size: 16px; box-sizing: border-box; }
        button { width: 100%; padding: 16px; margin-top: 20px; border-radius: 12px; border: none; background: var(--accent); color: white; font-weight: 700; cursor: pointer; transition: 0.3s; }
        button:disabled { background: #475569; cursor: not-allowed; }
    </style>
</head>
<body>
<div class="card">
    <h2 style="color:var(--accent); margin:0;">RT DIGITAL</h2>
    <p style="color:#94A3B8; font-size:14px;">Silakan login petugas ronda</p>
    <input type="text" id="user" placeholder="Username">
    <input type="password" id="pass" placeholder="Password">
    <button id="btn-login" onclick="login()">Masuk Sekarang</button>
</div>

<script>
    // PASTIKAN URL INI ADALAH URL "EXEC" TERBARU SETELAH DEPLOY
    const scriptURL = 'https://script.google.com/macros/s/AKfycbw6BUZEXc_WxNilOD7tdg5hJ2pmErMltdtDkgmu0vQeL3ATR9lu4XbK2cEPm1DU-nvB/exec';

    function login() {
        const u = document.getElementById('user').value.trim();
        const p = document.getElementById('pass').value.trim();
        const btn = document.getElementById('btn-login');

        if(!u || !p) return alert("Isi Username & Password, Bro!");

        // Ubah tampilan tombol
        btn.innerText = "Mengecek Data...";
        btn.disabled = true;

        // Buat nama callback unik
        const cb = "cb_" + Math.round(Math.random() * 1000000);
        
        // Buat elemen script untuk JSONP
        const s = document.createElement('script');
        
        // Handler respon dari Google Script
        window[cb] = (res) => {
            if (res.status === "success") {
                // Simpan data user ke memori HP
                localStorage.setItem("jimpitan_user", JSON.stringify(res));
                // Pindah ke halaman dashboard
                window.location.href = "dashboard.html";
            } else {
                alert("Login Gagal! Username atau Password salah.");
                btn.innerText = "Masuk Sekarang";
                btn.disabled = false;
            }
            
            // Bersihkan elemen script & window function
            if (s.parentNode) s.parentNode.removeChild(s);
            delete window[cb];
        };

        // Jika dalam 10 detik tidak ada respon, anggap error/timeout
        setTimeout(() => {
            if (btn.disabled && btn.innerText === "Mengecek Data...") {
                alert("Koneksi lambat atau URL Script salah. Cek Deploy ulang!");
                btn.innerText = "Masuk Sekarang";
                btn.disabled = false;
            }
        }, 10000);

        // Eksekusi pemanggilan ke Google Script
        s.src = `${scriptURL}?callback=${cb}&action=login&username=${encodeURIComponent(u)}&password=${encodeURIComponent(p)}`;
        document.body.appendChild(s);
    }
</script>
</body>
</html>
