<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
  <title>KD LIVE - Online Coaching & Batches</title>
  <meta name="description" content="Explore all KD LIVE online batches for competitive exams.">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="">
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800;900&amp;display=swap" rel="stylesheet">
  <style>
    :root {
      --primary: #2563eb;
      --primary-hover: #1d4ed8;
      --navy: #0f172a;
      --card-bg: #ffffff;
      --bg-surface: #f8fafc;
      --border-color: #e2e8f0;
      --text-main: #0f172a;
      --text-muted: #64748b;
      --success: #10b981;
      --danger: #ef4444;
      --radius-lg: 16px;
      --radius-sm: 10px;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; -webkit-tap-highlight-color: transparent; }
    
    body {
      font-family: 'Plus Jakarta Sans', sans-serif;
      background-color: var(--bg-surface);
      color: var(--text-main);
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      line-height: 1.5;
    }

    /* Top Sticky Header */
    .top-header {
      position: sticky;
      top: 0;
      z-index: 50;
      background: rgba(255, 255, 255, 0.9);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--border-color);
    }
    
    .header-container {
      max-width: 1120px;
      margin: 0 auto;
      padding: 12px 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .pw-brand-badge {
      display: flex;
      align-items: center;
      gap: 12px;
      background: #ffffff;
      border: 1px solid var(--border-color);
      padding: 6px 16px 6px 8px;
      border-radius: 999px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.03);
    }

    .pw-header-logo {
      width: 38px;
      height: 38px;
      border-radius: 50%;
      object-fit: cover;
    }

    .brand-text-wrap {
      display: flex;
      flex-direction: column;
      justify-content: center;
    }

    .title-row {
      display: flex;
      align-items: center;
      gap: 6px;
    }

    .pw-title {
      font-size: 16px;
      font-weight: 800;
      color: var(--navy);
      letter-spacing: -0.3px;
      line-height: 1.2;
    }

    .pw-verified {
      width: 15px;
      height: 15px;
      background: var(--primary);
      color: #ffffff;
      border-radius: 50%;
      font-size: 9px;
      display: inline-flex;
      align-items: center;
      justify-content: center;
    }

    .developer-subtext {
      font-size: 11px;
      font-weight: 700;
      color: var(--primary);
      letter-spacing: 0.2px;
      line-height: 1.2;
      margin-top: 2px;
    }

    /* Main Container */
    .main-wrap {
      max-width: 1120px;
      width: 100%;
      margin: 0 auto;
      padding: 24px 20px 80px;
      flex: 1;
    }

    /* Search Bar */
    .search-wrapper {
      margin-bottom: 24px;
      position: relative;
    }

    .search-input {
      width: 100%;
      padding: 14px 48px 14px 48px;
      font-size: 15px;
      font-weight: 500;
      border: 1.5px solid var(--border-color);
      border-radius: var(--radius-lg);
      background: #ffffff;
      color: var(--text-main);
      outline: none;
      transition: all 0.2s ease;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.02);
    }

    .search-input:focus {
      border-color: var(--primary);
      box-shadow: 0 0 0 4px rgba(37, 99, 235, 0.12);
    }

    .search-icon {
      position: absolute;
      left: 16px;
      top: 50%;
      transform: translateY(-50%);
      font-size: 16px;
      color: #94a3b8;
      pointer-events: none;
    }

    .clear-search-btn {
      position: absolute;
      right: 14px;
      top: 50%;
      transform: translateY(-50%);
      width: 26px;
      height: 26px;
      border-radius: 50%;
      border: none;
      background: #f1f5f9;
      color: var(--text-muted);
      display: none;
      place-items: center;
      cursor: pointer;
      font-size: 12px;
      transition: background 0.2s;
    }

    .clear-search-btn:hover { background: #e2e8f0; }
    .clear-search-btn.active { display: grid; }

    /* Heading & Stats */
    .heading-bar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 6px;
    }

    .page-heading {
      font-size: 24px;
      font-weight: 800;
      color: var(--navy);
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .green-board {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      background: linear-gradient(135deg, #059669 0%, #10b981 100%);
      color: #ffffff;
      padding: 3px 12px;
      border-radius: 999px;
      font-size: 13px;
      font-weight: 800;
      box-shadow: 0 2px 8px rgba(16, 185, 129, 0.25);
    }

    .sub-count-text {
      font-size: 14px;
      color: var(--text-muted);
      margin-bottom: 20px;
      font-weight: 500;
    }

    /* Filter Chips */
    .chips-row {
      display: flex;
      align-items: center;
      gap: 10px;
      overflow-x: auto;
      padding-bottom: 20px;
      scrollbar-width: none;
    }

    .chips-row::-webkit-scrollbar { display: none; }

    .filter-chip {
      white-space: nowrap;
      padding: 8px 18px;
      border-radius: 999px;
      border: 1px solid var(--border-color);
      background: #ffffff;
      color: #475569;
      font-size: 13.5px;
      font-weight: 600;
      cursor: pointer;
      transition: all 0.2s ease;
    }

    .filter-chip:hover {
      border-color: #cbd5e1;
      background: #f1f5f9;
    }

    .filter-chip.active {
      background: var(--navy);
      color: #ffffff;
      border-color: var(--navy);
      box-shadow: 0 4px 12px rgba(15, 23, 42, 0.15);
    }

    /* Batch Cards Grid */
    .batches-grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: 24px;
    }

    @media (min-width: 640px) { .batches-grid { grid-template-columns: repeat(2, 1fr); } }
    @media (min-width: 1024px) { .batches-grid { grid-template-columns: repeat(3, 1fr); } }

    .batch-card {
      background: var(--card-bg);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-lg);
      overflow: hidden;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.03);
      display: flex;
      flex-direction: column;
      transition: all 0.25s cubic-bezier(0.4, 0, 0.2, 1);
    }

    .batch-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 12px 28px rgba(0, 0, 0, 0.08);
      border-color: #cbd5e1;
    }

    .card-banner {
      position: relative;
      width: 100%;
      height: 180px;
      background: #f1f5f9;
      overflow: hidden;
      border-bottom: 1px solid var(--border-color);
    }

    .banner-img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      display: block;
      transition: transform 0.3s ease;
    }

    .batch-card:hover .banner-img {
      transform: scale(1.02);
    }

    .card-content {
      padding: 18px;
      display: flex;
      flex-direction: column;
      flex: 1;
    }

    .category-label {
      font-size: 11.5px;
      font-weight: 800;
      color: #ea580c;
      text-transform: uppercase;
      letter-spacing: 0.5px;
    }

    .batch-title {
      font-size: 16px;
      font-weight: 800;
      color: var(--navy);
      margin: 6px 0 12px;
      line-height: 1.4;
      display: -webkit-box;
      -webkit-line-clamp: 2;
      -webkit-box-orient: vertical;
      overflow: hidden;
      height: 44px;
    }

    .details-row, .status-row {
      display: flex;
      align-items: center;
      gap: 8px;
      font-size: 13px;
      color: var(--text-muted);
      font-weight: 500;
      margin-bottom: 8px;
    }

    .status-dot {
      width: 8px;
      height: 8px;
      border-radius: 50%;
    }

    .card-footer {
      margin-top: auto;
      padding-top: 16px;
      border-top: 1px solid #f1f5f9;
    }

    .buy-btn {
      display: block;
      background: var(--navy);
      color: #ffffff;
      border: none;
      padding: 12px 16px;
      border-radius: var(--radius-sm);
      font-size: 14px;
      font-weight: 700;
      text-decoration: none;
      cursor: pointer;
      width: 100%;
      text-align: center;
      transition: all 0.2s ease;
      box-shadow: 0 2px 6px rgba(15, 23, 42, 0.12);
    }

    .buy-btn:hover {
      background: var(--primary);
      box-shadow: 0 4px 12px rgba(37, 99, 235, 0.25);
    }

    .buy-btn.locked {
      background: #f1f5f9;
      color: #94a3b8;
      cursor: not-allowed;
      box-shadow: none;
      border: 1px solid var(--border-color);
    }

    /* Footer & Empty State */
    .developer-footer {
      text-align: center;
      margin-top: 50px;
      font-size: 13px;
      color: var(--text-muted);
      font-weight: 600;
    }

    .empty-state {
      text-align: center;
      padding: 60px 20px;
      background: #ffffff;
      border: 1.5px dashed var(--border-color);
      border-radius: var(--radius-lg);
      display: none;
      grid-column: 1/-1;
    }

    .empty-state h3 { font-size: 18px; color: var(--navy); margin-bottom: 6px; }
    .empty-state p { font-size: 14px; color: var(--text-muted); margin-bottom: 16px; }

    .reset-btn {
      background: var(--primary);
      color: #fff;
      border: none;
      padding: 10px 22px;
      border-radius: var(--radius-sm);
      font-weight: 700;
      font-size: 13.5px;
      cursor: pointer;
      transition: background 0.2s;
    }

    .reset-btn:hover { background: var(--primary-hover); }

    /* =======================================
       Custom Popup Modal CSS
    ======================================= */
    .popup-overlay {
      position: fixed;
      inset: 0;
      background: rgba(15, 23, 42, 0.65);
      backdrop-filter: blur(8px);
      -webkit-backdrop-filter: blur(8px);
      z-index: 9999;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 20px;
      opacity: 0;
      visibility: hidden;
      transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    }

    .popup-overlay.active {
      opacity: 1;
      visibility: visible;
    }

    .popup-card {
      position: relative;
      background: #ffffff;
      width: 100%;
      max-width: 400px;
      border-radius: 20px;
      padding: 28px 22px;
      text-align: center;
      box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
      border: 1px solid rgba(226, 232, 240, 0.8);
      transform: scale(0.9) translateY(20px);
      transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    }

    .popup-overlay.active .popup-card {
      transform: scale(1) translateY(0);
    }

    .popup-close {
      position: absolute;
      top: 14px;
      right: 16px;
      background: #f1f5f9;
      border: none;
      width: 32px;
      height: 32px;
      border-radius: 50%;
      font-size: 20px;
      color: var(--text-muted);
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: center;
      transition: all 0.2s;
    }

    .popup-close:hover {
      background: #e2e8f0;
      color: var(--navy);
    }

    .popup-logo-container {
      width: 72px;
      height: 72px;
      margin: 0 auto 16px;
      border-radius: 50%;
      padding: 4px;
      background: linear-gradient(135deg, #2563eb, #10b981);
      box-shadow: 0 6px 16px rgba(37, 99, 235, 0.25);
    }

    .popup-logo {
      width: 100%;
      height: 100%;
      border-radius: 50%;
      object-fit: cover;
      background: #ffffff;
    }

    .popup-title {
      font-size: 20px;
      font-weight: 800;
      color: var(--navy);
      margin-bottom: 8px;
    }

    .popup-desc {
      font-size: 13.5px;
      color: var(--text-muted);
      line-height: 1.5;
      margin-bottom: 22px;
      padding: 0 8px;
    }

    .popup-btn-group {
      display: flex;
      flex-direction: column;
      gap: 12px;
    }

    .popup-btn {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      padding: 12px 18px;
      border-radius: 12px;
      font-size: 14px;
      font-weight: 700;
      text-decoration: none;
      color: #ffffff;
      transition: all 0.2s ease;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
    }

    .popup-btn svg {
      width: 20px;
      height: 20px;
      fill: currentColor;
    }

    .btn-telegram {
      background: #229ED9;
    }

    .btn-telegram:hover {
      background: #1d8cbd;
      box-shadow: 0 6px 16px rgba(34, 158, 217, 0.35);
    }

    .btn-whatsapp {
      background: #25D366;
    }

    .btn-whatsapp:hover {
      background: #20bd5a;
      box-shadow: 0 6px 16px rgba(37, 211, 102, 0.35);
    }
  </style>
</head>
<body>
  <header class="top-header">
    <div class="header-container">
      <div class="pw-brand-badge">
        <img class="pw-header-logo" src="https://i.postimg.cc/Pqg46Zgt/image-search-1790505464474.jpg" alt="KD LIVE Logo" onerror="this.src='https://via.placeholder.com/38'">
        <div class="brand-text-wrap">
          <div class="title-row">
            <span class="pw-title">KD LIVE</span>
            <span class="pw-verified">✓</span>
          </div>
          <span class="developer-subtext">Developer By MedxrohitBihar</span>
        </div>
      </div>
    </div>
  </header>

  <main class="main-wrap">
    <div class="search-wrapper">
      <span class="search-icon">🔍</span>
      <input type="text" id="searchInput" class="search-input" placeholder="Search batches by title, exam, or topic..." autocomplete="off">
      <button id="clearSearchBtn" class="clear-search-btn">✕</button>
    </div>

    <div class="heading-bar">
      <h1 class="page-heading">
        All Batches
        <span class="green-board" id="greenBoardCount">0</span>
      </h1>
    </div>
    <div class="sub-count-text" id="subCountText">Loading available courses...</div>

    <div class="chips-row" id="chipsRow">
      <button class="filter-chip active" data-filter="all">All</button>
      <button class="filter-chip" data-filter="kd">KD</button>
      <button class="filter-chip" data-filter="maths">Maths</button>
      <button class="filter-chip" data-filter="reasoning">Reasoning</button>
      <button class="filter-chip" data-filter="ssc">SSC</button>
      <button class="filter-chip" data-filter="english">English</button>
    </div>

    <div class="batches-grid" id="batchesGrid"></div>

    <div class="empty-state" id="emptyState">
      <h3>No Batches Found</h3>
      <p>We couldn't find any courses matching your search criteria.</p>
      <button class="reset-btn" id="resetFilterBtn">Reset Filters</button>
    </div>

    <div class="developer-footer">
      Developed with ❤️ by MedxrohitBihar
    </div>
  </main>

  <!-- Custom Popup Modal -->
  <div class="popup-overlay" id="customPopup">
      <div class="popup-card">
          <button class="popup-close" onclick="closePopup()">&times;</button>
          <div class="popup-logo-container">
              <img class="popup-logo" src="https://i.postimg.cc/wMYf41jh/1788716447275.png" alt="Popup Logo">
          </div>
          <div class="popup-title">Join Our Community</div>
          <div class="popup-desc">Get instant updates, direct study links, and premium study materials by joining our official handles.</div>
          <div class="popup-btn-group">
              <a href="https://t.me/+cw7TRotEzcczNThl" target="_blank" class="popup-btn btn-telegram">
                  <svg viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm4.64 6.8c-.15 1.58-.8 5.42-1.13 7.19-.14.75-.42 1-.68 1.03-.58.05-1.02-.38-1.58-.75-.88-.58-1.38-.94-2.23-1.5-.99-.65-.35-1.01.22-1.59.15-.15 2.71-2.48 2.76-2.69.01-.03.01-.14-.07-.2-.08-.06-.19-.04-.27-.02-.12.03-1.99 1.27-5.62 3.72-.53.36-1.01.54-1.44.53-.47-.01-1.38-.27-2.06-.49-.83-.27-1.49-.42-1.43-.89.03-.25.38-.51 1.08-.78 4.23-1.84 7.05-3.05 8.46-3.63 4.03-1.68 4.87-1.98 5.42-1.99.12 0 .38.03.55.17.14.12.18.28.2.45-.02.07-.02.13-.04.2z"/></svg>
                  Join Telegram Channel
              </a>
              <a href="https://whatsapp.com/channel/0029Vb6FhReEquiLz1jNH00o" target="_blank" class="popup-btn btn-whatsapp">
                  <svg viewBox="0 0 24 24"><path d="M17.472 14.382c-.297-.149-1.758-.868-2.031-.967-.272-.099-.47-.149-.669.149-.198.297-.768.967-.941 1.165-.173.198-.347.223-.644.074-.297-.149-1.255-.462-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.297-.347.446-.521.151-.172.2-.296.3-.495.099-.198.05-.372-.025-.521-.075-.148-.669-1.611-.916-2.206-.242-.579-.487-.501-.669-.51l-.57-.01c-.198 0-.52.074-.792.372s-1.04 1.016-1.04 2.479 1.065 2.876 1.213 3.074c.149.198 2.096 3.2 5.077 4.487.709.306 1.263.489 1.694.626.712.226 1.36.194 1.872.118.571-.085 1.758-.719 2.006-1.413.248-.695.248-1.29.173-1.414-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.353z"/></svg>
                  Join WhatsApp Channel
              </a>
          </div>
      </div>
  </div>

  <script>
    const fallbackBatches = [
      { id: "new-1", name: "ENGLISH BY NEETU SINGH 75 BATCH", class: "Foundation", exam: "SSC", photo: "https://i.postimg.cc/13NRSfmC/image-search-1790593787677.jpg", link: "https://madxrohitbihar-app.github.io/NEETU-SINGH-3/", locked: false },
      { id: "new-2", name: "COMPULSORY ENGLISH BATCH BY NEETU SINGH 12 BATCH", class: "Special", exam: "English", photo: "https://i.postimg.cc/cJBS13VM/Picsart-26-09-28-07-51-14-952.png", link: "https://madxrohitbihar-app.github.io/NEETU-SINGH-4/", locked: false },
      { id: "new-3", name: "ENGLISH BY NEETU SINGH 62 VOD", class: "Combo", exam: "Reasoning", photo: "https://i.postimg.cc/XNF3JXTn/image-search-1790594205364.jpg", link: "https://madxrohitbihar-app.github.io/NEETU-SINGH-5/", locked: false },
      { id: "1", name: "ENGLISH SPECIAL NEETU SINGH BASIC TO ADVANCE PRE + MAINS", class: "Foundation", exam: "English", photo: "https://i.postimg.cc/sxybNbkC/image-search-1790510985052.png", link: "https://madxrohitbihar-app.github.io/NEETU-SINGH-1/", locked: false },
      { id: "2", name: "ENGLISH COMBO BATCH BASIC TO ADVANCE PRE + MAINS", class: "Combo", exam: "English", photo: "https://i.postimg.cc/3wv6JK7y/image-search-1790510465789.jpg", link: "https://madxrohitbihar-app.github.io/NEETU-SINGH-2/", locked: false },
      { id: "3", name: "FOUNDATION BATCH FOR SSC & ALL COMPETITIVE EXAMS", class: "Foundation", exam: "SSC", photo: "https://i.postimg.cc/Yqm8cdxL/image-search-1790506552143.jpg", link: "#", locked: true },
      { id: "4", name: "ENGLISH SPECIAL", class: "Special", exam: "English", photo: "https://i.postimg.cc/1RLR5zDY/image-search-1790506572592.jpg", link: "#", locked: true },
      { id: "5", name: "REASONING FOUNDATION BATCH FOR SSC & ALL EXAMS", class: "Foundation", exam: "Reasoning", photo: "https://i.postimg.cc/G2TFG2tZ/image-search-1790506582479.jpg", link: "#", locked: true },
      { id: "6", name: "UPTGT/PGT-2026 LITERATURE & GRAMMAR", class: "State Exam", exam: "KD", photo: "https://i.postimg.cc/fRWY55kk/image-search-1790506599219.jpg", link: "#", locked: true },
      { id: "7", name: "UP TGT PGT-2026 COMPLETE LITERATURE, GRAMMAR + GS", class: "State Exam", exam: "KD", photo: "https://i.postimg.cc/4NP9KtwT/image-search-1790506608549.jpg", link: "#", locked: true },
      { id: "8", name: "FOUNDATION BATCH FOR SSC & ALL OTHER EXAMS COMBO FULL COURSE", class: "Combo", exam: "SSC", photo: "https://i.postimg.cc/hGkzF04d/image-search-1790506620653.jpg", link: "#", locked: true },
      { id: "9", name: "ENGLISH SPECIAL", class: "Special", exam: "English", photo: "https://i.postimg.cc/CMHZtD3k/image-search-1790506642887.jpg", link: "#", locked: true },
      { id: "10", name: "ENGLISH SPECIAL BASIC TO ADVANCE (PRE + MAINS)", class: "Foundation", exam: "English", photo: "https://i.postimg.cc/52Gjvmzc/image-search-1790506649721.jpg", link: "#", locked: true },
      { id: "11", name: "ENGLISH A TO Z VOD BATCH", class: "VOD", exam: "English", photo: "https://i.postimg.cc/zvJf5tsg/image-search-1790506656219.jpg", link: "#", locked: true },
      { id: "12", name: "ENGLISH SPECIAL COMPETITIVE", class: "Special", exam: "English", photo: "https://i.postimg.cc/QN081bLQ/image-search-1790506662943.jpg", link: "#", locked: true },
      { id: "13", name: "SSC GD, UP CONSTABLE DELHI POLICE UP HOME GUARD", class: "Target", exam: "SSC", photo: "https://i.postimg.cc/T14vStGB/image-search-1790506700161.jpg", link: "#", locked: true },
      { id: "14", name: "ALLAHABAD HIGH COURT RO /ARO BATCH", class: "State Exam", exam: "KD", photo: "https://i.postimg.cc/9ML6RL4D/image-search-1790506705465.jpg", link: "#", locked: true },
      { id: "15", name: "ENGLISH A TO Z VOD BATCH", class: "VOD", exam: "English", photo: "https://i.postimg.cc/yYMwZgdB/image-search-1790506712278.jpg", link: "#", locked: true },
      { id: "16", name: "UP SUPER TET 2026 Aadesh Sir Special Batch", class: "Teaching", exam: "KD", photo: "https://i.postimg.cc/7Lmsmfxr/image-search-1790506727865.jpg", link: "#", locked: true },
      { id: "17", name: "FOUNDATION BATCH FOR SSC & ALL COMPETITIVE EXAMS", class: "Foundation", exam: "SSC", photo: "https://i.postimg.cc/SRzgSdcj/image-search-1790506733537.jpg", link: "#", locked: true },
      { id: "18", name: "REASONING 04 SPECIAL BATCH", class: "Special", exam: "Reasoning", photo: "https://i.postimg.cc/28nfTFgL/image-search-1790506738302.jpg", link: "#", locked: true },
      { id: "19", name: "RRB TECHNICIAN & ALP BHARTI 2026", class: "Railway", exam: "KD", photo: "https://i.postimg.cc/7Y8FCJhR/image-search-1790506749844.jpg", link: "#", locked: true },
      { id: "20", name: "ENGLISH COMBO BATCH PRE + MAINS", class: "Combo", exam: "English", photo: "https://i.postimg.cc/W1sx8RM6/image-search-1790506760282.jpg", link: "#", locked: true },
      { id: "21", name: "SPOKEN ENGLISH NEETU MA'AM", class: "Spoken", exam: "English", photo: "https://i.postimg.cc/PqRcdP0b/image-search-1790506772162.jpg", link: "#", locked: true },
      { id: "22", name: "UP SUPERTET 2026 (PRIMARY) ENGLISH SPECIAL", class: "Teaching", exam: "English", photo: "https://i.postimg.cc/j2VFJBx2/image-search-1790506789070.jpg", link: "#", locked: true }
    ];

    let allBatchesData = [];
    let currentSearch = "";
    let currentFilter = "all";

    const batchesGrid = document.getElementById("batchesGrid");
    const searchInput = document.getElementById("searchInput");
    const clearSearchBtn = document.getElementById("clearSearchBtn");
    const greenBoardCount = document.getElementById("greenBoardCount");
    const subCountText = document.getElementById("subCountText");
    const emptyState = document.getElementById("emptyState");
    const chipsRow = document.getElementById("chipsRow");
    const resetFilterBtn = document.getElementById("resetFilterBtn");

    function loadAllData() {
      allBatchesData = fallbackBatches;
      filterAndRender();
    }

    function filterAndRender() {
      let filtered = allBatchesData;

      if (currentFilter !== "all") {
        filtered = filtered.filter(b => `${b.name} ${b.exam} ${b.class}`.toLowerCase().includes(currentFilter));
      }

      if (currentSearch) {
        filtered = filtered.filter(b => `${b.name} ${b.exam} ${b.class}`.toLowerCase().includes(currentSearch.toLowerCase()));
      }

      greenBoardCount.textContent = filtered.length;
      subCountText.textContent = `${filtered.length} ${filtered.length === 1 ? 'course' : 'courses'} available for your preparation`;

      if (filtered.length === 0) {
        batchesGrid.innerHTML = "";
        emptyState.style.display = "block";
        return;
      }

      emptyState.style.display = "none";
      batchesGrid.innerHTML = filtered.map(b => `
        <article class="batch-card">
          <div class="card-banner">
            <img class="banner-img" src="${b.photo}" alt="${b.name}" loading="lazy" onerror="this.onerror=null; this.src='https://via.placeholder.com/400x200?text=KD+LIVE+Batch';">
          </div>
          <div class="card-content">
            <span class="category-label">${b.class || 'KD LIVE'}</span>
            <h2 class="batch-title" title="${b.name}">${b.name}</h2>
            <div class="details-row">
              <span>📖 ${b.exam || 'General'}</span>
            </div>
            <div class="status-row">
              <span class="status-dot" style="background: ${b.locked ? 'var(--danger)' : 'var(--success)'}"></span>
              <span style="color: ${b.locked ? 'var(--danger)' : 'var(--success)'}">${b.locked ? 'Locked Batch' : 'Ongoing Batch'}</span>
            </div>
            <div class="card-footer">
              ${b.locked ? 
                `<button class="buy-btn locked" disabled>🔒 Locked</button>` : 
                `<a href="${b.link}" class="buy-btn" target="_blank" rel="noopener noreferrer">Enroll Now</a>`
              }
            </div>
          </div>
        </article>
      `).join("");
    }

    searchInput.addEventListener("input", (e) => {
      currentSearch = e.target.value.trim();
      clearSearchBtn.classList.toggle("active", currentSearch.length > 0);
      filterAndRender();
    });

    clearSearchBtn.addEventListener("click", () => {
      searchInput.value = "";
      currentSearch = "";
      clearSearchBtn.classList.remove("active");
      filterAndRender();
    });

    chipsRow.addEventListener("click", (e) => {
      const btn = e.target.closest(".filter-chip");
      if (!btn) return;
      document.querySelectorAll(".filter-chip").forEach(c => c.classList.remove("active"));
      btn.classList.add("active");
      currentFilter = btn.dataset.filter;
      filterAndRender();
    });

    resetFilterBtn.addEventListener("click", () => {
      searchInput.value = "";
      currentSearch = "";
      currentFilter = "all";
      document.querySelectorAll(".filter-chip").forEach(c => c.classList.remove("active"));
      document.querySelector('[data-filter="all"]').classList.add("active");
      filterAndRender();
    });

    // =======================================
    // Popup Modal Functions
    // =======================================
    function showPopup() {
      const popup = document.getElementById('customPopup');
      if (popup) {
        popup.classList.add('active');
      }
    }

    function closePopup() {
      const popup = document.getElementById('customPopup');
      if (popup) {
        popup.classList.remove('active');
      }
    }

    // Close popup on overlay background click
    document.getElementById('customPopup')?.addEventListener('click', function(e) {
      if (e.target === this) {
        closePopup();
      }
    });

    // Auto trigger popup on page load after a short delay
    window.addEventListener('DOMContentLoaded', () => {
      loadAllData();
      setTimeout(showPopup, 600);
    });
  </script>
</body>
</html>
