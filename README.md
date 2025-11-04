<!doctype html>
<html lang="id">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Unban WhatsApp — DenzByteID</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
<style>
  :root{
    --bg1:#05060a;
    --bg2:#0e0f17;
    --card:#0b0b0d;
    --muted:#9aa0a6;
    --accent1:#20f7d6;
    --accent2:#8a61ff;
    --input:#0f1520;
  }
  *{box-sizing:border-box}
  body{
    margin:0;
    min-height:100vh;
    font-family:"Poppins",system-ui,Arial,sans-serif;
    background: radial-gradient(1200px 600px at 10% 10%, #07102a 0%, #08121a 12%, #05060a 70%), linear-gradient(180deg,var(--bg1),var(--bg2));
    color:#e6eef3;
    display:flex;
    align-items:flex-start;
    justify-content:center;
    padding:20px;
  }

  .topbar{
    position:fixed;
    left:18px;
    top:14px;
    display:flex;
    align-items:center;
    gap:12px;
    color:#00e6c7;
    font-weight:600;
    letter-spacing:0.6px;
    z-index:30;
    cursor:pointer;
  }
  .hamb{
    width:26px;height:20px;display:inline-grid;gap:3px;
  }
  .hamb span{display:block;height:3px;background:#00e6c7;border-radius:3px;opacity:.95}

  .dropdown{
    display:none;
    position:fixed;
    top:48px;
    left:16px;
    background:#0e0f17;
    border:1px solid rgba(255,255,255,0.05);
    border-radius:8px;
    box-shadow:0 8px 20px rgba(0,0,0,0.6);
    z-index:40;
    width:160px;
  }
  .dropdown a{
    display:block;
    padding:10px 14px;
    color:#00e6c7;
    text-decoration:none;
    font-size:14px;
  }
  .dropdown a:hover{
    background:rgba(255,255,255,0.05);
  }

  /* Submenu */
  .submenu{
    display:none;
    background:#141622;
    border-top:1px solid rgba(255,255,255,0.05);
  }
  .submenu a{
    font-size:13px;
    color:#7afff3;
    padding-left:28px;
  }
  .submenu a:hover{
    background:rgba(255,255,255,0.04);
  }

  .wrap{
    width:100%;
    max-width:420px;
    margin-top:60px;
    display:flex;
    align-items:center;
    justify-content:center;
  }

  .card{
    width:100%;
    background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
    border-radius:18px;
    padding:28px;
    box-shadow: 0 12px 40px rgba(2,8,20,0.7), inset 0 1px 0 rgba(255,255,255,0.02);
    border: 1px solid rgba(255,255,255,0.02);
    position:relative;
    overflow:hidden;
  }

  .avatar{
    width:70px;height:70px;border-radius:50%;
    background:#0c0c0f;
    display:grid;place-items:center;
    position:relative;
    margin:0 auto 12px;
    border:4px solid rgba(255,255,255,0.03);
    box-shadow:0 6px 18px rgba(0,0,0,0.6);
  }
  .avatar svg{width:44px;height:44px;display:block}
  .check{
    position:absolute;right:-6px;bottom:-6px;width:30px;height:30px;border-radius:50%;
    background:#0d8e5a;border:3px solid #0b0b0d;display:grid;place-items:center;color:#fff;font-size:14px;
    box-shadow:0 6px 10px rgba(13,142,90,0.22);
  }

  h1.title{
    text-align:center;margin:12px 0 18px;font-size:20px;color:#33f3d0;font-weight:700;
  }

  label{
    display:block;color:var(--muted);font-size:13px;margin-bottom:8px;margin-top:8px;
  }
  .field{
    width:100%;
    background:var(--input);
    border-radius:10px;padding:12px 14px;border:1px solid rgba(255,255,255,0.02);
    color:#d9e8ef;font-size:15px;
    outline:none;
  }
  .field::placeholder{color:#67727a}

  .btn{
    margin-top:18px;
    width:100%;
    padding:12px 16px;
    border-radius:10px;
    font-weight:700;
    font-size:15px;
    color:#001;
    background: linear-gradient(90deg,var(--accent1),var(--accent2));
    border:none;
    cursor:pointer;
    box-shadow: 0 8px 18px rgba(10,10,30,0.5);
  }
  .btn:active{transform:translateY(1px)}

  .hint{
    margin-top:16px;font-size:12px;color:var(--muted);line-height:1.4;text-align:center;padding:0 6px;
  }
  footer{margin-top:10px;text-align:center;font-size:12px;color:#9aa0a6}
</style>
</head>
<body>
  <div class="topbar" id="menuBtn">
    <div class="hamb"><span></span><span></span><span></span></div>
    <div>Web OneDev</div>
  </div>

  <div class="dropdown" id="dropdownMenu">
    <a href="#" id="contactBtn">Contact Admin ▾</a>
    <div class="submenu" id="submenu">
      <a href="https://wa.me/628123456789">WhatsApp</a>
      <a href="https://t.me/YourTelegramUsername">Telegram</a>
    </div>
  </div>

  <div class="wrap">
    <div class="card">
      <div class="avatar">
        <svg viewBox="0 0 24 24" fill="none">
          <circle cx="12" cy="8" r="3" stroke="#cfeef0" stroke-width="1.4" fill="rgba(255,255,255,0.02)"/>
          <path d="M4 20c0-2.8 4.5-4 8-4s8 1.2 8 4" stroke="#cfeef0" stroke-width="1.4" stroke-linecap="round"/>
        </svg>
        <div class="check">✓</div>
      </div>

      <h1 class="title">Unban WhatsApp</h1>

      <label for="nomor">Nomor WhatsApp yang diblokir</label>
      <input id="nomor" class="field" type="text" placeholder="+62xxxxxxxxxx">

      <label for="alasan">Pilih Opsi Band</label>
      <select id="alasan" class="field">
        <option value="">-- Pilih alasan --</option>
        <option value="spam">Opsi Spam</option>
        <option value="permanen">Opsi Permanen</option>
      </select>

      <button class="btn" id="sendBtn">KIRIM BANDING</button>

      <div class="hint">
        Saat tombol ditekan: sistem akan membuka Gmail (Android). Silahkan kirim pesannya lalu tunggu balasan WhatsApp.
      </div>

      <footer>© 2025 • Unban WhatsApp — DenzByteID</footer>
    </div>
  </div>

<script>
  const menuBtn = document.getElementById('menuBtn');
  const dropdown = document.getElementById('dropdownMenu');
  const contactBtn = document.getElementById('contactBtn');
  const submenu = document.getElementById('submenu');
  let open = false;
  let subOpen = false;

  menuBtn.addEventListener('click', () => {
    open = !open;
    dropdown.style.display = open ? 'block' : 'none';
  });

  contactBtn.addEventListener('click', (e) => {
    e.preventDefault();
    subOpen = !subOpen;
    submenu.style.display = subOpen ? 'block' : 'none';
  });

  document.addEventListener('click', (e) => {
    if(!menuBtn.contains(e.target) && !dropdown.contains(e.target)){
      dropdown.style.display = 'none';
      submenu.style.display = 'none';
      open = false;
      subOpen = false;
    }
  });

  document.getElementById('sendBtn').addEventListener('click', function(){
    const no = document.getElementById('nomor').value.trim();
    const alasan = document.getElementById('alasan').value;
    if(!no){
      alert('Isi nomor WhatsApp yang diblokir dulu, bro.');
      return;
    }
    if(!alasan){
      alert('Pilih opsi alasan dulu, bro.');
      return;
    }

    const subject = encodeURIComponent('Permintaan Peninjauan Akun WhatsApp yang Diblokir');
    const bodyText = `Halo tim WhatsApp,%0A%0ASaya ingin mengajukan banding untuk akun saya yang diblokir.%0A%0ANomor WhatsApp: ${encodeURIComponent(no)}%0AJenis blokir: ${alasan === 'permanen' ? 'Permanen (Hard Ban)' : 'Spam / Laporan'}%0A%0ASaya yakin tidak melakukan pelanggaran terhadap kebijakan WhatsApp. Mohon agar akun saya dapat ditinjau kembali.%0A%0ATerima kasih.%0A%0AHormat saya,%0A[Nama Anda]`;
    window.location.href = `mailto:support@whatsapp.com?subject=${subject}&body=${bodyText}`;
  });
</script>
</body>
</html>
