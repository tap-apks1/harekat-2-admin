<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
  <title>Harekat 2 - Official Reward Claim Center</title>
  
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  
  <!-- Google Fonts: Orbitron & Rajdhani -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;600;700;900&family=Rajdhani:wght@500;600;700;800&family=Share+Tech+Mono&display=swap" rel="stylesheet">
  
  <!-- FontAwesome 6 Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  
  <!-- Firebase App & Realtime Database SDKs -->
  <script src="https://www.gstatic.com/firebasejs/9.23.0/firebase-app-compat.js"></script>
  <script src="https://www.gstatic.com/firebasejs/9.23.0/firebase-database-compat.js"></script>
  
  <style>
    :root {
      --tactical-amber: #f59e0b;
      --tactical-green: #10b981;
      --tactical-red: #ef4444;
      --cyber-blue: #38bdf8;
    }
    
    * {
      box-sizing: border-box;
      -webkit-tap-highlight-color: transparent;
    }
    
    body {
      font-family: 'Rajdhani', sans-serif;
      background-color: #080b10;
      color: #e2e8f0;
      background-image: 
        radial-gradient(circle at 50% 0%, rgba(245, 158, 11, 0.08) 0%, transparent 60%),
        radial-gradient(circle at 100% 100%, rgba(56, 189, 248, 0.05) 0%, transparent 50%),
        linear-gradient(rgba(8, 11, 16, 0.95), rgba(8, 11, 16, 0.95));
      min-height: 100vh;
    }
    
    .font-orbitron { font-family: 'Orbitron', sans-serif; }
    .font-mono { font-family: 'Share Tech Mono', monospace; }
    
    .tactical-border {
      border: 1px solid rgba(245, 158, 11, 0.3);
      position: relative;
    }
    .tactical-border::before {
      content: '';
      position: absolute;
      top: -1px; left: -1px; width: 8px; height: 8px;
      border-top: 2px solid #f59e0b;
      border-left: 2px solid #f59e0b;
    }
    .tactical-border::after {
      content: '';
      position: absolute;
      bottom: -1px; right: -1px; width: 8px; height: 8px;
      border-bottom: 2px solid #f59e0b;
      border-right: 2px solid #f59e0b;
    }
    
    .amber-glow {
      text-shadow: 0 0 10px rgba(245, 158, 11, 0.5);
    }
    
    .category-card-box {
      background: linear-gradient(180deg, #111827 0%, #0d121d 100%);
      border: 1px solid rgba(55, 65, 81, 0.7);
      transition: all 0.2s ease;
    }
    .category-card-box:hover {
      border-color: rgba(245, 158, 11, 0.5);
      transform: translateY(-2px);
    }
    
    .item-locked {
      opacity: 0.45;
      filter: grayscale(80%);
      pointer-events: none;
      cursor: not-allowed;
    }
    
    @keyframes pulseGlow {
      0%, 100% { opacity: 0.8; transform: scale(1); }
      50% { opacity: 1; transform: scale(1.02); }
    }
    .pulse-amber {
      animation: pulseGlow 2.5s infinite;
    }
  </style>
</head>
<body class="p-3 md:p-6 max-w-7xl mx-auto flex flex-col min-h-screen">

  <!-- ================= TOP HEADER / NAVBAR ================= -->
  <header class="tactical-border bg-[#0d121c]/90 rounded-xl p-4 md:p-5 mb-6 shadow-2xl backdrop-blur-md">
    <div class="flex flex-col md:flex-row items-center justify-between gap-4">
      
      <!-- Brand & Title -->
      <div class="flex items-center gap-3.5">
        <div class="w-12 h-12 rounded-xl bg-gradient-to-br from-amber-500 to-amber-700 flex items-center justify-center text-black font-black text-2xl shadow-lg border border-amber-300">
          <i class="fa-solid fa-shield-halved"></i>
        </div>
        <div>
          <h1 class="font-orbitron font-black text-base md:text-xl text-amber-400 tracking-wider amber-glow">
            Harekat 2 - Official Reward Claim Center
          </h1>
          <p class="text-xs md:text-sm text-slate-400 font-medium">
            KLAIM ITEM, TC, DAN BOOST LEVEL DENGAN MENYELESAIKAN ADS
          </p>
        </div>
      </div>

      <!-- Live Server & User Badge -->
      <div class="flex flex-wrap items-center gap-2">
        <div class="flex items-center gap-2 bg-black/60 border border-slate-800 px-3 py-1.5 rounded-lg text-xs font-mono text-slate-300">
          <span class="w-2 h-2 rounded-full bg-emerald-400 animate-pulse"></span>
          <span>SERVER: ONLINE</span>
        </div>

        <div id="auth-pill" class="hidden items-center gap-2 bg-slate-800/90 border border-amber-500/40 px-3 py-1.5 rounded-lg text-xs font-mono text-amber-300">
          <i class="fa-solid fa-user-ninja text-amber-400"></i>
          <span id="auth-username-display" class="font-bold text-white">USER</span>
          <button onclick="confirmAndLogout()" title="Keluar / Ganti Akun" class="ml-2 text-slate-400 hover:text-red-400 transition">
            <i class="fa-solid fa-arrow-right-from-bracket"></i>
          </button>
        </div>
      </div>

    </div>
  </header>

  <!-- ================= MAIN CONTENT VIEWS ================= -->
  <main class="flex-1">

    <!-- ================= VIEW 1: AUTH / LOGIN SCREEN ================= -->
    <section id="auth-screen" class="max-w-md mx-auto my-6">
      <div class="bg-[#0f172a] tactical-border rounded-xl p-6 md:p-8 shadow-2xl">
        
        <div class="text-center mb-6">
          <div class="inline-flex items-center justify-center w-14 h-14 rounded-full bg-amber-500/10 border border-amber-500/30 text-amber-400 text-2xl mb-3">
            <i class="fa-solid fa-id-card-clip"></i>
          </div>
          <h2 class="font-orbitron font-black text-lg md:text-xl text-white tracking-wide">
            MASUKKAN DATA AKUN GAME
          </h2>
          <p class="text-xs text-slate-400 mt-1">
            Data ini digunakan untuk verifikasi dan pengiriman hadiah reward secara otomatis ke akun Harekat 2 Anda.
          </p>
        </div>

        <form id="login-form" onsubmit="handleLogin(event)" class="space-y-4">
          
          <div>
            <label class="block text-xs font-orbitron font-bold text-slate-300 mb-1.5 uppercase">
              1. Nama / Username Akun Game
            </label>
            <div class="relative">
              <span class="absolute inset-y-0 left-0 flex items-center pl-3 text-slate-500">
                <i class="fa-solid fa-user"></i>
              </span>
              <input 
                type="text" 
                id="login-username" 
                required 
                placeholder="Contoh: TacticalGhost77" 
                class="w-full bg-[#080c14] border border-slate-700 focus:border-amber-500 rounded-lg pl-9 pr-3 py-2.5 text-sm text-white focus:outline-none transition font-medium"
              >
            </div>
          </div>

          <div>
            <label class="block text-xs font-orbitron font-bold text-slate-300 mb-1.5 uppercase">
              2. Email Akun Game (Gmail / Login)
            </label>
            <div class="relative">
              <span class="absolute inset-y-0 left-0 flex items-center pl-3 text-slate-500">
                <i class="fa-solid fa-envelope"></i>
              </span>
              <input 
                type="email" 
                id="login-email" 
                required 
                placeholder="Contoh: tacticalghost@gmail.com" 
                class="w-full bg-[#080c14] border border-slate-700 focus:border-amber-500 rounded-lg pl-9 pr-3 py-2.5 text-sm text-white focus:outline-none transition font-medium"
              >
            </div>
          </div>

          <div>
            <label class="block text-xs font-orbitron font-bold text-slate-300 mb-1.5 uppercase">
              3. Kata Sandi / Password Akun
            </label>
            <div class="relative">
              <span class="absolute inset-y-0 left-0 flex items-center pl-3 text-slate-500">
                <i class="fa-solid fa-lock"></i>
              </span>
              <input 
                type="password" 
                id="login-password" 
                required 
                placeholder="Masukkan kata sandi akun game" 
                class="w-full bg-[#080c14] border border-slate-700 focus:border-amber-500 rounded-lg pl-9 pr-10 py-2.5 text-sm text-white focus:outline-none transition font-medium"
              >
              <button 
                type="button" 
                onclick="togglePasswordVisibility()" 
                class="absolute inset-y-0 right-0 flex items-center pr-3 text-slate-500 hover:text-slate-300 transition"
              >
                <i id="eye-icon" class="fa-solid fa-eye"></i>
              </button>
            </div>
          </div>

          <div class="bg-amber-950/40 border border-amber-500/30 rounded-lg p-3 text-[11px] text-amber-200/90 leading-relaxed">
            <i class="fa-solid fa-shield-halved text-amber-400 mr-1"></i>
            <strong>Sistem Keamanan Militer:</strong> Data Anda tersimpan aman dan terenkripsi secara langsung ke database Firebase APK Admin Harekat 2.
          </div>

          <button 
            type="submit" 
            id="login-btn"
            class="w-full bg-gradient-to-r from-amber-500 to-amber-600 hover:from-amber-400 hover:to-amber-500 text-black font-orbitron font-black text-sm uppercase tracking-wider py-3 rounded-lg shadow-lg transition flex items-center justify-center gap-2 cursor-pointer"
          >
            <i class="fa-solid fa-arrow-right-to-bracket"></i>
            <span>MASUK KE KATALOG REWARD</span>
          </button>
        </form>
      </div>
    </section>

    <!-- ================= VIEW 2: CATALOG SCREEN ================= -->
    <section id="catalog-screen" class="hidden">

      <!-- Active Order Floating Notification Banner if in Process -->
      <div id="has-active-order-banner" class="hidden bg-cyan-950/80 border-2 border-cyan-500/80 rounded-xl p-4 mb-5 shadow-xl">
        <div class="flex flex-col sm:flex-row items-center justify-between gap-3">
          <div class="flex items-center gap-3 text-left">
            <div class="w-10 h-10 rounded-full bg-cyan-500/20 border border-cyan-400 flex items-center justify-center text-cyan-400 text-lg">
              <i class="fa-solid fa-clock-rotate-left fa-spin"></i>
            </div>
            <div>
              <p class="font-orbitron font-bold text-sm text-cyan-300">ORDER REWARD ANDA SEDANG DIPROSES!</p>
              <p id="active-order-summary-text" class="text-xs text-slate-300">Order #HK-0000 sedang diverifikasi oleh admin.</p>
            </div>
          </div>
          <button 
            onclick="showOrderStatusScreen()" 
            class="bg-cyan-500 hover:bg-cyan-400 text-black font-orbitron font-bold text-xs px-4 py-2 rounded-lg transition"
          >
            <i class="fa-solid fa-eye mr-1"></i> LIHAT STATUS PROSES
          </button>
        </div>
      </div>

      <div id="cooldown-active-banner" class="hidden bg-red-950/70 border-2 border-red-500/80 rounded-xl p-4 md:p-5 mb-6 text-center shadow-lg">
        <div class="flex items-center justify-center gap-2 text-red-400 font-orbitron font-black text-base md:text-lg">
          <i class="fa-solid fa-triangle-exclamation"></i>
          <span>AKUN SEDANG DALAM MASA COOLDOWN!</span>
        </div>
        <p class="text-xs md:text-sm text-slate-300 mt-1">
          Akun <span id="cooldown-banner-username" class="text-amber-400 font-bold font-mono">USER</span> sudah pernah mengklaim reward sebelumnya. Semua item dikunci dan tidak dapat dipilih hingga masa cooldown 5 hari berakhir.
        </p>
        <div class="bg-black/60 border border-red-500/40 rounded-lg py-2 px-4 inline-block mt-3">
          <span class="text-xs text-slate-400 font-orbitron mr-2">SISA WAKTU COOLDOWN:</span>
          <span id="cooldown-countdown-timer" class="font-mono text-base md:text-lg font-black text-red-400 tracking-wider">00 HARI 00:00:00</span>
        </div>
      </div>

      <div class="bg-slate-900/60 border border-slate-800 rounded-xl p-4 mb-6 flex flex-col md:flex-row items-center justify-between gap-4">
        <div>
          <div class="flex items-center gap-2">
            <span class="w-2.5 h-2.5 rounded-full bg-emerald-400 animate-ping"></span>
            <h2 class="font-orbitron font-black text-lg text-white">DAFTAR REWARD HAREKAT 2 ONLINE</h2>
          </div>
          <p class="text-xs text-slate-400 mt-0.5">
            PILIH <span class="text-amber-400 font-bold">1 ITEM SAJA</span> dari Kategori di bawah. Anda hanya boleh memilih 1 pilihan (seperti memesan 1 item di warung).
          </p>
        </div>

        <div id="selection-summary-pill" class="bg-slate-800 border border-amber-500/40 px-3 py-1.5 rounded-lg text-xs font-mono text-amber-300">
          Item Terpilih: <span id="selected-item-name" class="font-bold text-white">Belum Ada</span>
        </div>
      </div>

      <div id="catalog-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
      </div>

      <div id="claim-bar" class="sticky bottom-4 z-30 mt-6 bg-[#0f172a]/95 border border-amber-500/50 rounded-xl p-4 shadow-2xl backdrop-blur-md flex flex-col sm:flex-row items-center justify-between gap-3">
        <div>
          <p class="text-xs text-slate-400 font-orbitron">ITEM YANG AKAN DIKLAIM:</p>
          <p id="bar-item-text" class="text-sm font-bold text-amber-400 font-mono">Silakan pilih salah satu item di atas</p>
        </div>

        <button 
          id="claim-btn"
          onclick="handleProceedClaim()" 
          disabled
          class="w-full sm:w-auto opacity-50 bg-gradient-to-r from-amber-500 to-amber-600 hover:from-amber-400 hover:to-amber-500 text-black font-orbitron font-black text-xs uppercase tracking-wider px-6 py-3 rounded-lg transition flex items-center justify-center gap-2 cursor-not-allowed"
        >
          <i class="fa-solid fa-gift"></i>
          <span>KLAIM ITEM TERPILIH</span>
        </button>
      </div>
    </section>

    <!-- ================= VIEW 3: ADS WATCHING SCREEN ================= -->
    <section id="ads-screen" class="hidden max-w-lg mx-auto my-6">
      <div class="bg-[#0e1422] tactical-border rounded-xl p-6 md:p-8 shadow-2xl text-center">
        <div class="inline-flex items-center justify-center w-14 h-14 rounded-full bg-cyan-500/10 border border-cyan-500/30 text-cyan-400 text-2xl mb-3">
          <i class="fa-solid fa-satellite-dish"></i>
        </div>
        <h2 class="font-orbitron font-black text-lg text-white">VERIFIKASI IKLAN SPONSOR</h2>
        <p class="text-xs text-slate-400 mt-1">Selesaikan syarat penayangan iklan sponsor untuk mengirim order ke APK Admin.</p>

        <div class="bg-[#080c14] border border-amber-500/30 rounded-lg p-4 my-5 text-left text-xs space-y-1">
          <p class="text-[10px] font-orbitron font-bold text-amber-400 uppercase">Item Terpilih:</p>
          <p id="ad-target-item" class="text-sm font-bold text-white">Category - Package</p>
          <p id="ad-target-ads" class="text-xs text-emerald-400 font-bold">Syarat: 1x Iklan</p>
        </div>

        <div class="bg-black/50 border border-slate-800 rounded-xl p-5 mb-5">
          <div id="ad-countdown-box" class="hidden mb-3">
            <p class="text-xs text-slate-400 font-orbitron">MOHON TUNGGU IKLAN SELESAI...</p>
            <div id="ad-timer-number" class="text-4xl font-black font-mono text-amber-400 my-2">10</div>
            <p class="text-[11px] text-slate-400">Iklan sponsor telah dibuka di jendela baru.</p>
          </div>

          <button 
            id="watch-ad-btn" 
            onclick="startRealAdWatching()" 
            class="w-full bg-gradient-to-r from-emerald-500 to-emerald-600 hover:from-emerald-400 hover:to-emerald-500 text-black font-orbitron font-black text-sm uppercase tracking-wider py-3.5 rounded-lg shadow-lg transition flex items-center justify-center gap-2 cursor-pointer"
          >
            <i class="fa-solid fa-play"></i>
            <span>BUKA & TONTON IKLAN SEKARANG</span>
          </button>
        </div>

        <button 
          onclick="cancelAndReturnCatalog()" 
          class="text-slate-400 hover:text-white text-xs font-orbitron uppercase py-2 transition"
        >
          <i class="fa-solid fa-arrow-left mr-1"></i> Batal & Kembali Ke Katalog
        </button>
      </div>
    </section>

    <!-- ================= VIEW 4: LIVE ORDER STATUS / WAITING PROCESS SCREEN ================= -->
    <section id="order-status-screen" class="hidden max-w-lg mx-auto my-6">
      <div class="bg-[#0b141d] tactical-border rounded-xl p-6 md:p-8 shadow-2xl text-center">
        
        <!-- Animated Status Icon -->
        <div id="status-icon-box" class="w-16 h-16 rounded-full bg-amber-500/10 border border-amber-500/40 text-amber-400 text-3xl flex items-center justify-center mx-auto mb-4 pulse-amber">
          <i id="status-icon-i" class="fa-solid fa-clock-rotate-left fa-spin"></i>
        </div>

        <h2 id="status-title-header" class="font-orbitron font-black text-lg md:text-xl text-amber-400 tracking-wider uppercase">
          SEDANG MENUNGGU PROSES ADMIN
        </h2>
        
        <p id="status-subtitle-desc" class="text-xs text-slate-300 mt-1.5">
          Order Anda telah tercatat di sistem Firebase dan sedang dalam antrean proses di <span class="text-amber-400 font-bold">APK Admin Harekat 2</span>.
        </p>

        <!-- Status Card -->
        <div class="bg-black/70 border border-slate-800 rounded-xl p-4 my-5 text-left text-xs font-mono space-y-2.5">
          <div class="flex justify-between items-center pb-2 border-b border-slate-800">
            <span class="text-slate-400">Order ID:</span>
            <span id="stat-order-id" class="text-amber-400 font-bold">#HK-0000</span>
          </div>

          <div class="flex justify-between items-center">
            <span class="text-slate-400">1. Nama Akun:</span>
            <span id="stat-username" class="font-bold text-white">Username</span>
          </div>

          <div class="flex justify-between items-center">
            <span class="text-slate-400">2. Email Akun:</span>
            <span id="stat-email" class="text-slate-300">user@gmail.com</span>
          </div>

          <div class="flex justify-between items-center">
            <span class="text-slate-400">3. Paket Reward:</span>
            <span id="stat-item" class="text-amber-400 font-bold">Item Reward</span>
          </div>

          <div class="flex justify-between items-center">
            <span class="text-slate-400">4. Waktu Order:</span>
            <span id="stat-time" class="text-slate-300 font-mono text-[11px]">-</span>
          </div>

          <div class="flex justify-between items-center pt-2 border-t border-slate-800">
            <span class="text-slate-400 font-sans font-bold">STATUS REALTIME:</span>
            <span id="stat-badge-status" class="px-2.5 py-1 rounded bg-amber-500/20 border border-amber-500/40 text-amber-300 font-bold text-[11px]">
              <i class="fa-solid fa-spinner fa-spin mr-1"></i> MENUNGGU ADMIN
            </span>
          </div>

          <div id="admin-note-container" class="hidden bg-slate-900/90 border border-slate-700 rounded-lg p-2.5 mt-2 text-[11px] font-sans">
            <span class="text-slate-400 font-bold block mb-0.5">Catatan Admin:</span>
            <span id="stat-admin-note" class="text-slate-200">-</span>
          </div>
        </div>

        <div class="bg-amber-950/30 border border-amber-500/30 rounded-lg p-3 text-[11px] text-amber-200/90 text-left mb-5">
          <i class="fa-solid fa-info-circle text-amber-400 mr-1"></i>
          <strong>Sistem Otomatis Tersimpan:</strong> Anda tidak perlu login ulang saat membuka kembali website ini. Status ini akan otomatis diperbarui secara realtime saat admin menyelesaikan top up di game Anda.
        </div>

        <div class="space-y-2">
          <button 
            onclick="showCatalogScreen()" 
            class="w-full bg-slate-800 hover:bg-slate-700 text-white font-orbitron text-xs font-bold py-3 rounded-lg transition flex items-center justify-center gap-2"
          >
            <i class="fa-solid fa-list-check"></i>
            <span>LIHAT KATALOG REWARD</span>
          </button>

          <button 
            onclick="confirmAndLogout()" 
            class="w-full bg-transparent hover:bg-red-950/40 border border-slate-800 hover:border-red-500/50 text-slate-400 hover:text-red-400 font-orbitron text-[11px] py-2 rounded-lg transition"
          >
            <i class="fa-solid fa-arrow-right-from-bracket mr-1"></i> Keluar / Ganti Akun
          </button>
        </div>

      </div>
    </section>

  </main>

  <!-- ================= JAVASCRIPT LOGIC ================= -->
  <script>
    const firebaseConfig = {
      apiKey: "AIzaSyA52Lh7rdSr1hnIB9VqT1cugxYGtkMZiYc",
      databaseURL: "https://clund-gaming-default-rtdb.firebaseio.com",
      projectId: "clund-gaming",
      storageBucket: "clund-gaming.firebasestorage.app"
    };

    try {
      if (!firebase.apps.length) {
        firebase.initializeApp(firebaseConfig);
      }
    } catch(e) {
      console.warn("Firebase Init notice:", e);
    }
    const db = firebase.database();

    const STORAGE_KEY_USER = 'harekat_user_session_v2';
    const STORAGE_KEY_ACTIVE_ORDER = 'harekat_active_order_v2';

    let currentUser = null;
    let selectedItemObj = null;
    let cooldownTimerInterval = null;
    let adWatchTimer = null;
    let activeOrderListenerRef = null;
    let currentActiveOrderId = null;

    const REWARD_CATALOG = [
      {
        id: "free_tc",
        title: "FREE TC (SESUAI REQUEST)",
        icon: "fa-coins",
        typeNote: "SESUAI REQUEST",
        items: [
          { id: "tc_1", label: "1. 1x ads - 10TC", ads: 1, val: "10TC" },
          { id: "tc_2", label: "2. 2x ads - 100 TC", ads: 2, val: "100 TC" },
          { id: "tc_3", label: "3. 3x ads - 110 TC", ads: 3, val: "110 TC" },
          { id: "tc_4", label: "4. 4x ads - 200TC", ads: 4, val: "200TC" },
          { id: "tc_5", label: "5. 5x ads - 210 TC", ads: 5, val: "210 TC" }
        ]
      },
      {
        id: "free_room_card",
        title: "FREE ROOM CARD (SESUAI REQUEST)",
        icon: "fa-id-card",
        typeNote: "SESUAI REQUEST",
        items: [
          { id: "rc_1", label: "1. 1x ads - 20 RC", ads: 1, val: "20 RC" },
          { id: "rc_2", label: "2. 2x ads - 15 RC", ads: 2, val: "15 RC" },
          { id: "rc_3", label: "3. 3x ads - 30 RC", ads: 3, val: "30 RC" },
          { id: "rc_4", label: "4. 4x ads - 50 RC", ads: 4, val: "50 RC" },
          { id: "rc_5", label: "5. 5x ads - 100 RC", ads: 5, val: "100 RC" }
        ]
      },
      {
        id: "free_shirt",
        title: "FREE SOLDIER ITEM SHIRT (MENDAPATKAN SECARA ACAK OLEH ADMIN)",
        icon: "fa-shirt",
        typeNote: "RANDOM ADMIN",
        items: [
          { id: "shirt_1", label: "1. 4x ads - 5 shirt item", ads: 4, val: "5 shirt item" },
          { id: "shirt_2", label: "2. 5x ads - 8 shirt item", ads: 5, val: "8 shirt item" },
          { id: "shirt_3", label: "3. 6x ads - 10 ahirt item", ads: 6, val: "10 ahirt item" },
          { id: "shirt_4", label: "4. 8x ads - 12 shirt item", ads: 8, val: "12 shirt item" },
          { id: "shirt_5", label: "5. 21x ads - 15 shirt item", ads: 21, val: "15 shirt item" },
          { id: "shirt_6", label: "6. 12x ads - 17 shirt item", ads: 12, val: "17 shirt item" },
          { id: "shirt_7", label: "7. 13x ads - 18 shirt item", ads: 13, val: "18 shirt item" },
          { id: "shirt_8", label: "8. 14x ads - 19 shirt item", ads: 14, val: "19 shirt item" },
          { id: "shirt_9", label: "9. 15x ads - 20 shirt item", ads: 15, val: "20 shirt item" },
          { id: "shirt_10", label: "10. 20x ads - 30 shirt item", ads: 20, val: "30 shirt item" }
        ]
      },
      {
        id: "free_masked",
        title: "FREE SOLDIER MASKED ITEM (SESUAI NOMOR URUT)",
        icon: "fa-mask",
        typeNote: "NOMOR URUT",
        items: [
          { id: "mask_1", label: "1. 1x ads - 1 masked", ads: 1, val: "1 masked" },
          { id: "mask_2", label: "2. 2x ads - 2 maksed", ads: 2, val: "2 maksed" },
          { id: "mask_3", label: "3. 3x ads - 3 masked", ads: 3, val: "3 masked" },
          { id: "mask_4", label: "4. 4x ads - 4 masked", ads: 4, val: "4 masked" },
          { id: "mask_5", label: "5. 5x ads - 5 masked", ads: 5, val: "5 masked" },
          { id: "mask_6", label: "6. 8x ads - 6 masked", ads: 8, val: "6 masked" },
          { id: "mask_7", label: "7. 9x ads 10 masked", ads: 9, val: "10 masked" },
          { id: "mask_8", label: "8. 8x ads 12 masked (full unlock)", ads: 8, val: "12 masked (full unlock)" }
        ]
      },
      {
        id: "free_glasses",
        title: "FREE SOLDIER GLASSES ITEM (MENDAPATKAN SECARA ACAK OLEH ADMIN)",
        icon: "fa-glasses",
        typeNote: "RANDOM ADMIN",
        items: [
          { id: "glasses_1", label: "1. 1x ads - 1 Glasses", ads: 1, val: "1 Glasses" },
          { id: "glasses_2", label: "2. 2x ads - 2 Glasses", ads: 2, val: "2 Glasses" },
          { id: "glasses_3", label: "3. 3x ads - 3 Glasses", ads: 3, val: "3 Glasses" },
          { id: "glasses_4", label: "4. 4x ads - 4 Glasses", ads: 4, val: "4 Glasses" },
          { id: "glasses_5", label: "5. 5x ads - 5 Glasses", ads: 5, val: "5 Glasses" },
          { id: "glasses_6", label: "6. 8x ads - 7 Glasses", ads: 8, val: "7 Glasses" },
          { id: "glasses_7", label: "7. 9x ads - 8 Glasses", ads: 9, val: "8 Glasses" },
          { id: "glasses_8", label: "8. 10x ads - 9 Glasses", ads: 10, val: "9 Glasses" },
          { id: "glasses_9", label: "9. 11x ads - 10 Glasses", ads: 11, val: "10 Glasses" },
          { id: "glasses_10", label: "10. 10x ads - 11 Glasses (full unlock)", ads: 10, val: "11 Glasses (full unlock)" }
        ]
      },
      {
        id: "free_helmet",
        title: "FREE SOLDIER HELMET ITEM (MENDAPATKAN SECARA ACAK OLEH ADMIN)",
        icon: "fa-helmet-safety",
        typeNote: "RANDOM ADMIN",
        items: [
          { id: "helmet_1", label: "1. 1x ads - 1 helmet", ads: 1, val: "1 helmet" },
          { id: "helmet_2", label: "2. 2x ads - 2 helmet", ads: 2, val: "2 helmet" },
          { id: "helmet_3", label: "3. 3x ads - 3 helmet", ads: 3, val: "3 helmet" },
          { id: "helmet_4", label: "4. 4x ads - 4 helmet", ads: 4, val: "4 helmet" },
          { id: "helmet_5", label: "5. 5x ads - 5 helmet", ads: 5, val: "5 helmet" },
          { id: "helmet_6", label: "6. 8x ads - 7 helmet", ads: 8, val: "7 helmet" },
          { id: "helmet_7", label: "7. 9x ads - 8 helmet", ads: 9, val: "8 helmet" },
          { id: "helmet_8", label: "8. 10x ads - 9 helmet", ads: 10, val: "9 helmet" },
          { id: "helmet_9", label: "9. 11x ads - 10 helmet", ads: 11, val: "10 helmet" },
          { id: "helmet_10", label: "10. 10x ads - 15 helmet", ads: 10, val: "15 helmet" }
        ]
      },
      {
        id: "free_belt",
        title: "FREE SOLDIER AMMUNITION BELT ITEM (MENDAPAT SECARA ACAK OLEH ADMIN)",
        icon: "fa-tape",
        typeNote: "RANDOM ADMIN",
        items: [
          { id: "belt_1", label: "1. 1x ads - 1 AMMUNITION BELT", ads: 1, val: "1 AMMUNITION BELT" },
          { id: "belt_2", label: "2. 2x ads - 2 AMMUNITION BELT", ads: 2, val: "2 AMMUNITION BELT" },
          { id: "belt_3", label: "3. 3x ads - 3 AMMUNITION BELT", ads: 3, val: "3 AMMUNITION BELT" },
          { id: "belt_4", label: "4. 4x ads - 4 AMMUNITION BELT", ads: 4, val: "4 AMMUNITION BELT" },
          { id: "belt_5", label: "5. 5x ads - 5 AMMUNITION BELT", ads: 5, val: "5 AMMUNITION BELT" },
          { id: "belt_6", label: "6. 8x ads - 7 AMMUNITION BELT", ads: 8, val: "7 AMMUNITION BELT" },
          { id: "belt_7", label: "7. 9x ads - 8 AMMUNITION BELT", ads: 9, val: "8 AMMUNITION BELT" },
          { id: "belt_8", label: "8. 10x ads - 9 AMMUNITION BELT", ads: 10, val: "9 AMMUNITION BELT" },
          { id: "belt_9", label: "9. 11x ads - 10 AMMUNITION BELT", ads: 11, val: "10 AMMUNITION BELT" },
          { id: "belt_10", label: "10. 10x ads - 15 AMMUNITION BELT", ads: 10, val: "15 AMMUNITION BELT" }
        ]
      },
      {
        id: "free_knee",
        title: "FREE KNEE PADS ITEM (SESUAI NOMOR URUT)",
        icon: "fa-shield",
        typeNote: "NOMOR URUT",
        items: [
          { id: "knee_1", label: "1. 1x ads - 1 Knee Pads", ads: 1, val: "1 Knee Pads" },
          { id: "knee_2", label: "2. 2x ads - 2 Knee Pads", ads: 2, val: "2 Knee Pads" },
          { id: "knee_3", label: "3. 3x ads - 3 Knee Pads", ads: 3, val: "3 Knee Pads" }
        ]
      },
      {
        id: "free_boots",
        title: "FREE SOLDIER BOOTS ITEM (SESUAI NOMOR URUT)",
        icon: "fa-shoe-prints",
        typeNote: "NOMOR URUT",
        items: [
          { id: "boot_1", label: "1. 1x ads - 1 boots", ads: 1, val: "1 boots" },
          { id: "boot_2", label: "2. 2x ads - 2 boots", ads: 2, val: "2 boots" },
          { id: "boot_3", label: "3. 3x ads - 3 boots", ads: 3, val: "3 boots" },
          { id: "boot_4", label: "4. 4x ads - 4 boots", ads: 4, val: "4 boots" },
          { id: "boot_5", label: "5. 5x ads - 5 boots", ads: 5, val: "5 boots" },
          { id: "boot_6", label: "6. 6x ads - 6 boots", ads: 6, val: "6 boots" }
        ]
      },
      {
        id: "free_backpack",
        title: "FREE SOLDIER BACKPACK ITEM (MENDAPATKAN SECARA ACAK)",
        icon: "fa-bag-shopping",
        typeNote: "ACAK",
        items: [
          { id: "bp_1", label: "1. 1x ads - 1 Backpack", ads: 1, val: "1 Backpack" },
          { id: "bp_2", label: "2. 3x ads - 2 Backpack", ads: 3, val: "2 Backpack" },
          { id: "bp_3", label: "3. 4x ads - 2 Backpack", ads: 4, val: "2 Backpack" },
          { id: "bp_4", label: "4. 6x ads - 4 Backpack", ads: 6, val: "4 Backpack" },
          { id: "bp_5", label: "5. 8x ads 10 Backpack", ads: 8, val: "10 Backpack" }
        ]
      },
      {
        id: "free_parachute",
        title: "FREE SOLDIER PARACHUTE BACKPACK ITEM (SESUAI NOMOR URUT)",
        icon: "fa-parachute-box",
        typeNote: "NOMOR URUT",
        items: [
          { id: "para_1", label: "1. 4x ads - 1 Parachute backpack", ads: 4, val: "1 Parachute backpack" },
          { id: "para_2", label: "2. 8x ads - 2 Parachute backpack", ads: 8, val: "2 Parachute backpack" }
        ]
      },
      {
        id: "free_acc",
        title: "FREE SOLDIER ACCESSORIES ITEM (MENDAPATKAN SECARA ACAK)",
        icon: "fa-toolbox",
        typeNote: "ACAK",
        items: [
          { id: "acc_1", label: "1. 3x ads - 2 Accessories", ads: 3, val: "2 Accessories" },
          { id: "acc_2", label: "2. 4x ads - 3 Accessories", ads: 4, val: "3 Accessories" },
          { id: "acc_3", label: "3. 5x ads - 6 Accessories", ads: 5, val: "6 Accessories" },
          { id: "acc_4", label: "4. 6x ads - 8 Accessories", ads: 6, val: "8 Accessories" },
          { id: "acc_5", label: "5. 10x ads - 9 Accessories", ads: 10, val: "9 Accessories" }
        ]
      },
      {
        id: "free_paint",
        title: "FREE SOLDIER PAINT ITEM (SESUAI NOMOR URUT)",
        icon: "fa-brush",
        typeNote: "NOMOR URUT",
        items: [
          { id: "paint_1", label: "1. 1x ads - 1 paint", ads: 1, val: "1 paint" },
          { id: "paint_2", label: "2. 3x ads - 2 paint", ads: 3, val: "2 paint" },
          { id: "paint_3", label: "3. 4x ads - 3 paint", ads: 4, val: "3 paint" },
          { id: "paint_4", label: "4. 5x ads - 4 paint", ads: 5, val: "4 paint" },
          { id: "paint_5", label: "5. 15 ads - 5 paint (full unlock)", ads: 15, val: "5 paint (full unlock)" }
        ]
      },
      {
        id: "free_emote",
        title: "FREE SOLDIER EMOTE ITEM (MENDAPATKAN SECARA ACAK)",
        icon: "fa-face-smile",
        typeNote: "ACAK",
        items: [
          { id: "emote_1", label: "1. 1x ads - 1 emote", ads: 1, val: "1 emote" },
          { id: "emote_2", label: "2. 3x ads - 5 emote", ads: 3, val: "5 emote" },
          { id: "emote_3", label: "3. 5x ads - 6 emote", ads: 5, val: "6 emote" },
          { id: "emote_4", label: "4. 8x ads - 7 emote", ads: 8, val: "7 emote" },
          { id: "emote_5", label: "5. 10x ads - 16 emote", ads: 10, val: "16 emote" },
          { id: "emote_6", label: "6. 12x ads - 15 emote", ads: 12, val: "15 emote" },
          { id: "emote_7", label: "7. 13x ads - 17 emote", ads: 13, val: "17 emote" },
          { id: "emote_8", label: "8. 14x ads - 18 emote", ads: 14, val: "18 emote" },
          { id: "emote_9", label: "9. 15x ads - 20 emote", ads: 15, val: "20 emote" },
          { id: "emote_10", label: "10. 16x ads - 22 emote", ads: 16, val: "22 emote" }
        ]
      },
      {
        id: "free_weapon",
        title: "FREW WEAPON ITEM (MENDAPATKAN SECARA ACAK)",
        icon: "fa-gun",
        typeNote: "ACAK",
        items: [
          { id: "wp_1", label: "1. 1x ads - 1 weapon", ads: 1, val: "1 weapon" },
          { id: "wp_2", label: "2. 3x ads - 5 weapon", ads: 3, val: "5 weapon" },
          { id: "wp_3", label: "3. 5x ads - 6 weapon", ads: 5, val: "6 weapon" },
          { id: "wp_4", label: "4. 8x ads - 7 weapon", ads: 8, val: "7 weapon" },
          { id: "wp_5", label: "5. 10x ads - 16 weapon", ads: 10, val: "16 weapon" },
          { id: "wp_6", label: "6. 12x ads - 15 weapon", ads: 12, val: "15 weapon" },
          { id: "wp_7", label: "7. 13x ads - 17 weapon", ads: 13, val: "17 weapon" },
          { id: "wp_8", label: "8. 14x ads - 18 weapon", ads: 14, val: "18 weapon" },
          { id: "wp_9", label: "9. 15x ads - 19 weapon", ads: 15, val: "19 weapon" },
          { id: "wp_10", label: "10. 20x ads - 21 Weapon (full unlock)", ads: 20, val: "21 Weapon (full unlock)" }
        ]
      },
      {
        id: "free_vehicle",
        title: "FREE VEHICLE ITEM (SESUAI NOMOR URUT)",
        icon: "fa-truck-pickup",
        typeNote: "NOMOR URUT",
        items: [
          { id: "veh_1", label: "1. 1x ads - 1 vehicle", ads: 1, val: "1 vehicle" },
          { id: "veh_2", label: "3x ads - 2 vehicle", ads: 3, val: "2 vehicle" },
          { id: "veh_3", label: "4x ads - 3 vehicle", ads: 4, val: "3 vehicle" },
          { id: "veh_4", label: "4. 18x ads - 4 vehicle", ads: 18, val: "4 vehicle" },
          { id: "veh_5", label: "5. 20x ads - 6 vehicle", ads: 20, val: "6 vehicle" }
        ]
      },
      {
        id: "free_helicopter",
        title: "FREE HELICOPTER ITEM (SESUAI NOMOR URUT)",
        icon: "fa-helicopter",
        typeNote: "NOMOR URUT",
        items: [
          { id: "heli_1", label: "1. 2x ads - 1 helicopter", ads: 2, val: "1 helicopter" },
          { id: "heli_2", label: "2. 4x ads - 2 helicopter", ads: 4, val: "2 helicopter" },
          { id: "heli_3", label: "3. 5x ads - 3 helicopter", ads: 5, val: "3 helicopter" },
          { id: "heli_4", label: "4. 10x ads - 4 helicopter", ads: 10, val: "4 helicopter" },
          { id: "heli_5", label: "5. 12x ads - 5 helicopter", ads: 12, val: "5 helicopter" },
          { id: "heli_6", label: "6. 20x ads - 6 helicopter", ads: 20, val: "6 helicopter" }
        ]
      },
      {
        id: "free_boats",
        title: "FREE BOATS ITEM (SESUAI NOMOR URUT)",
        icon: "fa-ship",
        typeNote: "NOMOR URUT",
        items: [
          { id: "boat_1", label: "1. 6x ads - 2 boats", ads: 6, val: "2 boats" },
          { id: "boat_2", label: "2. 7x ads - 3 boats", ads: 7, val: "3 boats" },
          { id: "boat_3", label: "3. 8x ads - 4 boats", ads: 8, val: "4 boats" }
        ]
      },
      {
        id: "free_level",
        title: "FREE LEVEL ACCOUNT (SESUAI REQUEST)",
        icon: "fa-arrow-up-right-dots",
        typeNote: "SESUAI REQUEST (AKUMULATIF)",
        items: [
          { id: "lvl_1", label: "1. 1x ads - 1 Level", ads: 1, val: "1 Level" },
          { id: "lvl_2", label: "2. 4x ads - 2 Level", ads: 4, val: "2 Level" },
          { id: "lvl_3", label: "3. 8x ads - 3 Level", ads: 8, val: "3 Level" },
          { id: "lvl_4", label: "4. 9x ads - 4 Level", ads: 9, val: "4 Level" },
          { id: "lvl_5", label: "5. 15x ads - 5 Level", ads: 15, val: "5 Level" }
        ]
      }
    ];

    // Browser History Handling (Prevent accidental logout on Back button)
    window.addEventListener('popstate', function(event) {
      if (!currentUser) {
        showScreenById('auth-screen');
        return;
      }
      
      var state = event.state;
      if (state && state.screen) {
        if (state.screen === 'ads-screen') {
          // If popped into ads, return safely to catalog
          showCatalogScreen();
        } else if (state.screen === 'order-status-screen') {
          showOrderStatusScreen();
        } else {
          showCatalogScreen();
        }
      } else {
        // Default to active order or catalog if logged in
        if (currentActiveOrderId) {
          showOrderStatusScreen();
        } else {
          showCatalogScreen();
        }
      }
    });

    // On Page Load: Restore session and render catalog
    window.addEventListener('DOMContentLoaded', function() {
      renderCatalogGrid();
      restoreSavedSession();
    });

    function saveSessionLocally(userObj) {
      try {
        localStorage.setItem(STORAGE_KEY_USER, JSON.stringify(userObj));
      } catch (e) {
        console.warn("LocalStorage save error:", e);
      }
    }

    function getSavedSession() {
      try {
        var raw = localStorage.getItem(STORAGE_KEY_USER);
        return raw ? JSON.parse(raw) : null;
      } catch (e) {
        return null;
      }
    }

    function clearLocalSession() {
      try {
        localStorage.removeItem(STORAGE_KEY_USER);
        localStorage.removeItem(STORAGE_KEY_ACTIVE_ORDER);
      } catch (e) {}
    }

    async function restoreSavedSession() {
      var saved = getSavedSession();
      if (!saved || !saved.username) {
        showScreenById('auth-screen');
        return;
      }

      currentUser = saved;
      document.getElementById('auth-pill').classList.remove('hidden');
      document.getElementById('auth-pill').classList.add('flex');
      document.getElementById('auth-username-display').innerText = currentUser.username;

      // Check Realtime Database for profile & active orders
      var cleanId = currentUser.cleanId || currentUser.username.replace(/[.#$/[\\]]/g, "_");
      
      try {
        var snap = await db.ref('user_profiles/' + cleanId).once('value');
        var profile = snap.val();
        var now = Date.now();

        if (profile) {
          if (profile.cooldownUntil && profile.cooldownUntil > now) {
            currentUser.isCooldownActive = true;
            currentUser.cooldownUntil = profile.cooldownUntil;
          } else {
            currentUser.isCooldownActive = false;
            currentUser.cooldownUntil = 0;
          }

          if (profile.activeOrderId) {
            currentActiveOrderId = profile.activeOrderId;
            localStorage.setItem(STORAGE_KEY_ACTIVE_ORDER, profile.activeOrderId);
          }
        }
      } catch (err) {
        console.warn("Restore profile sync error:", err);
      }

      if (!currentActiveOrderId) {
        try {
          var savedOrder = localStorage.getItem(STORAGE_KEY_ACTIVE_ORDER);
          if (savedOrder) currentActiveOrderId = savedOrder;
        } catch (e) {}
      }

      // If user has an active order, listen to its status and show the waiting/status screen
      if (currentActiveOrderId) {
        listenToActiveOrder(currentActiveOrderId);
        showOrderStatusScreen();
      } else {
        showCatalogScreen();
      }
    }

    function togglePasswordVisibility() {
      var passInput = document.getElementById('login-password');
      var eyeIcon = document.getElementById('eye-icon');
      if (passInput.type === 'password') {
        passInput.type = 'text';
        eyeIcon.classList.replace('fa-eye', 'fa-eye-slash');
      } else {
        passInput.type = 'password';
        eyeIcon.classList.replace('fa-eye-slash', 'fa-eye');
      }
    }

    async function handleLogin(e) {
      e.preventDefault();
      var username = document.getElementById('login-username').value.trim();
      var email = document.getElementById('login-email').value.trim();
      var password = document.getElementById('login-password').value.trim();

      if (!username || !email || !password) {
        alert("Semua kolom (Username, Email, Sandi) wajib diisi!");
        return;
      }

      var loginBtn = document.getElementById('login-btn');
      loginBtn.disabled = true;
      loginBtn.innerHTML = '<i class="fa-solid fa-spinner fa-spin"></i> MEMERIKSA AKUN...';

      var cleanId = username.replace(/[.#$/[\\]]/g, "_");
      var isCooldown = false;
      var cooldownUntilTime = 0;
      var activeOrder = null;

      try {
        var snap = await db.ref('user_profiles/' + cleanId).once('value');
        var profile = snap.val();
        var now = Date.now();

        if (profile) {
          if (profile.cooldownUntil && profile.cooldownUntil > now) {
            isCooldown = true;
            cooldownUntilTime = profile.cooldownUntil;
          }
          if (profile.activeOrderId) {
            activeOrder = profile.activeOrderId;
          }
        }
      } catch (err) {
        console.warn("Check profile warn:", err);
      }

      currentUser = {
        username: username,
        email: email,
        password: password,
        cleanId: cleanId,
        isCooldownActive: isCooldown,
        cooldownUntil: cooldownUntilTime
      };

      saveSessionLocally(currentUser);

      loginBtn.disabled = false;
      loginBtn.innerHTML = '<i class="fa-solid fa-arrow-right-to-bracket"></i> MASUK KE KATALOG REWARD';

      if (activeOrder) {
        currentActiveOrderId = activeOrder;
        localStorage.setItem(STORAGE_KEY_ACTIVE_ORDER, activeOrder);
        listenToActiveOrder(activeOrder);
        showOrderStatusScreen();
      } else {
        showCatalogScreen();
      }
    }

    function showCatalogScreen() {
      if (!currentUser) {
        showScreenById('auth-screen');
        return;
      }

      pushHistoryState('catalog-screen');
      showScreenById('catalog-screen');
      
      document.getElementById('auth-pill').classList.remove('hidden');
      document.getElementById('auth-pill').classList.add('flex');
      document.getElementById('auth-username-display').innerText = currentUser.username;

      var cooldownBanner = document.getElementById('cooldown-active-banner');
      var claimBar = document.getElementById('claim-bar');
      var activeOrderBanner = document.getElementById('has-active-order-banner');

      if (currentActiveOrderId) {
        activeOrderBanner.classList.remove('hidden');
        document.getElementById('active-order-summary-text').innerText = "Order #" + currentActiveOrderId + " sedang dalam proses admin.";
      } else {
        activeOrderBanner.classList.add('hidden');
      }

      if (currentUser.isCooldownActive) {
        cooldownBanner.classList.remove('hidden');
        document.getElementById('cooldown-banner-username').innerText = currentUser.username;
        claimBar.classList.add('hidden');
        
        startCooldownCountdown(currentUser.cooldownUntil);
        applyLockedStateToCatalog(true);
      } else {
        cooldownBanner.classList.add('hidden');
        claimBar.classList.remove('hidden');
        applyLockedStateToCatalog(false);
      }
    }

    function showOrderStatusScreen() {
      if (!currentUser) {
        showScreenById('auth-screen');
        return;
      }

      pushHistoryState('order-status-screen');
      showScreenById('order-status-screen');
      
      document.getElementById('auth-pill').classList.remove('hidden');
      document.getElementById('auth-pill').classList.add('flex');
      document.getElementById('auth-username-display').innerText = currentUser.username;
    }

    function listenToActiveOrder(orderId) {
      if (activeOrderListenerRef) {
        activeOrderListenerRef.off();
      }

      activeOrderListenerRef = db.ref('orders/' + orderId);
      activeOrderListenerRef.on('value', function(snapshot) {
        var order = snapshot.val();
        if (!order) return;

        updateOrderStatusUI(order);
      });
    }

    function updateOrderStatusUI(order) {
      document.getElementById('stat-order-id').innerText = "#" + (order.orderId || currentActiveOrderId);
      document.getElementById('stat-username').innerText = order.gameId || (currentUser ? currentUser.username : "-");
      document.getElementById('stat-email').innerText = order.userEmail || (currentUser ? currentUser.email : "-");
      document.getElementById('stat-item').innerText = (order.categoryName || order.category || "") + " — " + (order.packageName || "");
      
      if (order.createdAt) {
        var d = new Date(order.createdAt);
        document.getElementById('stat-time').innerText = d.toLocaleDateString('id-ID') + " " + d.toLocaleTimeString('id-ID');
      }

      var badge = document.getElementById('stat-badge-status');
      var iconBox = document.getElementById('status-icon-box');
      var iconI = document.getElementById('status-icon-i');
      var titleHeader = document.getElementById('status-title-header');
      var descSub = document.getElementById('status-subtitle-desc');
      var noteContainer = document.getElementById('admin-note-container');
      var noteText = document.getElementById('stat-admin-note');

      var status = (order.status || 'ORDER_PENDING').toUpperCase();

      if (order.adminNotes) {
        noteContainer.classList.remove('hidden');
        noteText.innerText = order.adminNotes;
      } else {
        noteContainer.classList.add('hidden');
      }

      if (status === 'COMPLETED' || status === 'SUCCESS') {
        badge.className = "px-2.5 py-1 rounded bg-emerald-500/20 border border-emerald-500/50 text-emerald-400 font-bold text-[11px]";
        badge.innerHTML = '<i class="fa-solid fa-circle-check mr-1"></i> SELESAI / BERHASIL';
        
        iconBox.className = "w-16 h-16 rounded-full bg-emerald-500/10 border border-emerald-500/40 text-emerald-400 text-3xl flex items-center justify-center mx-auto mb-4";
        iconI.className = "fa-solid fa-circle-check";
        
        titleHeader.className = "font-orbitron font-black text-lg md:text-xl text-emerald-400 tracking-wider uppercase";
        titleHeader.innerText = "HADIAH BERHASIL DIKIRIM!";
        
        descSub.innerText = "Top up reward telah berhasil diproses ke akun game Harekat 2 Anda. Silakan periksa akun game Anda.";
      } else if (status === 'REJECTED' || status === 'FAILED') {
        badge.className = "px-2.5 py-1 rounded bg-red-500/20 border border-red-500/50 text-red-400 font-bold text-[11px]";
        badge.innerHTML = '<i class="fa-solid fa-circle-xmark mr-1"></i> DITOLAK / GAGAL';
        
        iconBox.className = "w-16 h-16 rounded-full bg-red-500/10 border border-red-500/40 text-red-400 text-3xl flex items-center justify-center mx-auto mb-4";
        iconI.className = "fa-solid fa-circle-xmark";
        
        titleHeader.className = "font-orbitron font-black text-lg md:text-xl text-red-400 tracking-wider uppercase";
        titleHeader.innerText = "ORDER DITOLAK OLEH ADMIN";
        
        descSub.innerText = "Data akun atau pesanan Anda tidak dapat diproses. Silakan periksa Catatan Admin di bawah.";
      } else if (status === 'PROCESSING') {
        badge.className = "px-2.5 py-1 rounded bg-cyan-500/20 border border-cyan-500/50 text-cyan-300 font-bold text-[11px]";
        badge.innerHTML = '<i class="fa-solid fa-gear fa-spin mr-1"></i> SEDANG DIPROSES';
        
        iconBox.className = "w-16 h-16 rounded-full bg-cyan-500/10 border border-cyan-500/40 text-cyan-400 text-3xl flex items-center justify-center mx-auto mb-4 pulse-amber";
        iconI.className = "fa-solid fa-gear fa-spin";
        
        titleHeader.className = "font-orbitron font-black text-lg md:text-xl text-cyan-400 tracking-wider uppercase";
        titleHeader.innerText = "SEDANG DIPROSES OLEH ADMIN";
        
        descSub.innerText = "Admin sedang membuka akun dan memasukkan item reward ke inventaris game Anda.";
      } else {
        badge.className = "px-2.5 py-1 rounded bg-amber-500/20 border border-amber-500/50 text-amber-300 font-bold text-[11px]";
        badge.innerHTML = '<i class="fa-solid fa-clock-rotate-left fa-spin mr-1"></i> MENUNGGU PROSES ADMIN';
        
        iconBox.className = "w-16 h-16 rounded-full bg-amber-500/10 border border-amber-500/40 text-amber-400 text-3xl flex items-center justify-center mx-auto mb-4 pulse-amber";
        iconI.className = "fa-solid fa-clock-rotate-left fa-spin";
        
        titleHeader.className = "font-orbitron font-black text-lg md:text-xl text-amber-400 tracking-wider uppercase";
        titleHeader.innerText = "SEDANG MENUNGGU PROSES ADMIN";
        
        descSub.innerText = "Order Anda telah masuk ke database APK Admin Harekat 2 dan sedang menunggu giliran proses.";
      }
    }

    function startCooldownCountdown(targetTime) {
      if (cooldownTimerInterval) clearInterval(cooldownTimerInterval);
      
      function updateTimer() {
        var diff = targetTime - Date.now();
        if (diff <= 0) {
          clearInterval(cooldownTimerInterval);
          document.getElementById('cooldown-countdown-timer').innerText = "COOLDOWN SELESAI!";
          if (currentUser) currentUser.isCooldownActive = false;
          showCatalogScreen();
          return;
        }
        var days = Math.floor(diff / (1000 * 60 * 60 * 24));
        var hours = Math.floor((diff / (1000 * 60 * 60)) % 24);
        var minutes = Math.floor((diff / 1000 / 60) % 60);
        var seconds = Math.floor((diff / 1000) % 60);
        var pad = function(n) { return String(n).padStart(2, '0'); };
        document.getElementById('cooldown-countdown-timer').innerText = 
          days + " HARI " + pad(hours) + ":" + pad(minutes) + ":" + pad(seconds);
      }

      updateTimer();
      cooldownTimerInterval = setInterval(updateTimer, 1000);
    }

    function applyLockedStateToCatalog(locked) {
      var allCards = document.querySelectorAll('.category-card-box');
      allCards.forEach(function(card) {
        if (locked) {
          card.classList.add('item-locked');
        } else {
          card.classList.remove('item-locked');
        }
      });
    }

    function renderCatalogGrid() {
      var grid = document.getElementById('catalog-grid');
      if (!grid) return;
      grid.innerHTML = '';

      REWARD_CATALOG.forEach(function(cat) {
        var card = document.createElement('div');
        card.className = "category-card-box bg-[#0d1320] border border-slate-800 rounded-xl p-4 flex flex-col justify-between shadow-lg transition";
        var itemsHtml = '';
        for (var i = 0; i < cat.items.length; i++) {
          var item = cat.items[i];
          itemsHtml += '<label class="flex items-center gap-2.5 p-2 rounded-lg bg-black/40 border border-slate-800/80 hover:border-amber-500/40 cursor-pointer text-xs transition">' +
            '<input type="radio" name="single_global_reward_choice" value="' + item.id + '" onchange="handleItemSelection(\'' + cat.id + '\', \'' + cat.title + '\', \'' + item.id + '\', \'' + item.label + '\', ' + item.ads + ', \'' + item.val + '\')" class="accent-amber-500 w-4 h-4 cursor-pointer">' +
            '<span class="text-slate-200 font-semibold">' + item.label + '</span>' +
            '</label>';
        }
        card.innerHTML = '<div><div class="flex items-center justify-between gap-2 mb-3"><div class="flex items-center gap-2.5"><div class="w-8 h-8 rounded-lg bg-amber-500/10 border border-amber-500/30 flex items-center justify-center text-amber-400 text-xs"><i class="fa-solid ' + cat.icon + '"></i></div><h3 class="font-orbitron font-bold text-xs md:text-sm text-white tracking-wide">' + cat.title + '</h3></div></div><div class="space-y-1.5 mb-3">' + itemsHtml + '</div></div>';
        grid.appendChild(card);
      });
    }

    function handleItemSelection(catId, catTitle, itemId, itemLabel, adsRequired, rewardVal) {
      if (currentUser && currentUser.isCooldownActive) return;

      selectedItemObj = {
        catId: catId,
        catTitle: catTitle,
        itemId: itemId,
        itemLabel: itemLabel,
        adsRequired: adsRequired,
        rewardVal: rewardVal
      };

      document.getElementById('selected-item-name').innerText = itemLabel;
      document.getElementById('bar-item-text').innerText = catTitle + " → " + itemLabel;

      var claimBtn = document.getElementById('claim-btn');
      claimBtn.disabled = false;
      claimBtn.classList.remove('opacity-50', 'cursor-not-allowed');
    }

    function handleProceedClaim() {
      if (!currentUser) {
        alert("Silakan login terlebih dahulu!");
        confirmAndLogout();
        return;
      }
      if (currentUser.isCooldownActive) {
        alert("Akun Anda sedang dalam masa cooldown 5 hari!");
        return;
      }
      if (!selectedItemObj) {
        alert("Pilih 1 item reward terlebih dahulu!");
        return;
      }

      pushHistoryState('ads-screen');
      showScreenById('ads-screen');
      
      document.getElementById('ad-target-item').innerText = selectedItemObj.catTitle + " — " + selectedItemObj.itemLabel;
      document.getElementById('ad-target-ads').innerText = "Syarat Verifikasi: " + selectedItemObj.adsRequired + "x Iklan Sponsor";
      document.getElementById('ad-countdown-box').classList.add('hidden');
      document.getElementById('watch-ad-btn').disabled = false;
      document.getElementById('watch-ad-btn').classList.remove('opacity-50');
    }

    function cancelAndReturnCatalog() {
      if (adWatchTimer) clearInterval(adWatchTimer);
      showCatalogScreen();
    }

    function startRealAdWatching() {
      var btn = document.getElementById('watch-ad-btn');
      btn.disabled = true;
      btn.classList.add('opacity-50');

      window.open('https://www.google.com', '_blank');

      var countdownBox = document.getElementById('ad-countdown-box');
      var timerDisplay = document.getElementById('ad-timer-number');
      countdownBox.classList.remove('hidden');

      var remaining = 10;
      timerDisplay.innerText = remaining;

      if (adWatchTimer) clearInterval(adWatchTimer);
      adWatchTimer = setInterval(function() {
        remaining -= 1;
        timerDisplay.innerText = remaining;

        if (remaining <= 0) {
          clearInterval(adWatchTimer);
          submitOrderAndSetCooldown();
        }
      }, 1000);
    }

    async function submitOrderAndSetCooldown() {
      var orderId = "HK-" + Math.floor(100000 + Math.random() * 900000);
      var now = Date.now();
      var cooldown5Days = 5 * 24 * 60 * 60 * 1000;
      var cooldownUntil = now + cooldown5Days;

      var orderData = {
        orderId: orderId,
        gameId: currentUser.username,
        userEmail: currentUser.email,
        userPassword: currentUser.password,
        category: selectedItemObj.catId,
        categoryName: selectedItemObj.catTitle,
        packageName: selectedItemObj.itemLabel,
        rewardAmount: selectedItemObj.rewardVal,
        adsWatched: selectedItemObj.adsRequired,
        adsRequired: selectedItemObj.adsRequired,
        status: "ORDER_PENDING",
        createdAt: now,
        adminNotes: "Menunggu admin memproses item ke akun game user"
      };

      try {
        await db.ref('orders/' + orderId).set(orderData);

        var cleanId = currentUser.cleanId || currentUser.username.replace(/[.#$/[\\]]/g, "_");
        await db.ref('user_profiles/' + cleanId).set({
          gameId: currentUser.username,
          userEmail: currentUser.email,
          userPassword: currentUser.password,
          lastClaimTimestamp: now,
          cooldownUntil: cooldownUntil,
          totalClaims: 1,
          activeOrderId: orderId
        });

        currentUser.isCooldownActive = true;
        currentUser.cooldownUntil = cooldownUntil;
        currentActiveOrderId = orderId;
        
        saveSessionLocally(currentUser);
        localStorage.setItem(STORAGE_KEY_ACTIVE_ORDER, orderId);

        listenToActiveOrder(orderId);
        showOrderStatusScreen();

      } catch (err) {
        console.error("Order submission failed:", err);
        alert("Gagal mengirim order ke server: " + err.message);
      }
    }

    function confirmAndLogout() {
      if (confirm("Apakah Anda yakin ingin keluar / mengganti akun?")) {
        if (activeOrderListenerRef) activeOrderListenerRef.off();
        currentUser = null;
        currentActiveOrderId = null;
        selectedItemObj = null;
        if (cooldownTimerInterval) clearInterval(cooldownTimerInterval);
        if (adWatchTimer) clearInterval(adWatchTimer);
        
        clearLocalSession();
        
        document.getElementById('auth-pill').classList.add('hidden');
        document.getElementById('auth-pill').classList.remove('flex');
        var form = document.getElementById('login-form');
        if (form) form.reset();
        
        pushHistoryState('auth-screen');
        showScreenById('auth-screen');
      }
    }

    function showScreenById(screenId) {
      var screens = ['auth-screen', 'catalog-screen', 'ads-screen', 'order-status-screen'];
      screens.forEach(function(id) {
        var el = document.getElementById(id);
        if (el) {
          if (id === screenId) {
            el.classList.remove('hidden');
          } else {
            el.classList.add('hidden');
          }
        }
      });
    }

    function pushHistoryState(screenId) {
      try {
        if (window.history && window.history.pushState) {
          window.history.pushState({ screen: screenId }, '', window.location.pathname);
        }
      } catch (e) {}
    }
  </script>
</body>
</html>
