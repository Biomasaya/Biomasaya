<!-- ─────────────────────────────────────────────
  Biomasaya README – animated, clean & science-y
  All animations are CSS-in-SVG (GitHub OK / no JS needed)
────────────────────────────────────────────── -->

<p align="center">
  <!-- Animated neon / stroke-fill logo (SVG Animated Text Fill) -->
  <svg viewBox="0 0 1200 220" width="100%" height="220" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Biomasaya">
    <defs>
      <linearGradient id="g" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stop-color="#56d9cd"/>
        <stop offset="50%" stop-color="#f2385a"/>
        <stop offset="100%" stop-color="#3aa1bf"/>
      </linearGradient>
      <filter id="glow">
        <feGaussianBlur stdDeviation="3" result="b1"/>
        <feMerge>
          <feMergeNode in="b1"/><feMergeNode in="SourceGraphic"/>
        </feMerge>
      </filter>
      <style>
        .word{
          font: 900 70px/1 "Open Sans", system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial, "Noto Sans JP", "Hiragino Kaku Gothic ProN", "Yu Gothic", sans-serif;
          text-transform: uppercase;
          letter-spacing: .12em;
          fill: none;
          stroke: url(#g);
          stroke-width: 3;
          stroke-linejoin: round;
          stroke-dasharray: 80 340;
          animation: dash 6s linear infinite;
          filter: url(#glow);
        }
        @keyframes dash {
          0%   { stroke-dashoffset:   0; }
          100% { stroke-dashoffset: -420; }
        }
      </style>
    </defs>
    <text class="word" x="50%" y="50%" text-anchor="middle" dy=".35em">Biomasaya</text>
  </svg>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Field-Biomechanics-56d9cd?style=for-the-badge&logoColor=white">
  <img src="https://img.shields.io/badge/OpenSim-EMG%20%2F%20CMC%20%2F%20RRA-3aa1bf?style=for-the-badge">
  <img src="https://img.shields.io/badge/Python-NumPy%20%7C%20pandas%20%7C%20matplotlib-f2385a?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/R-ggplot2-6a9bd8?style=for-the-badge&logo=r&logoColor=white">
</p>

<p align="center">
  <!-- Colorful loading dots (as a tiny ambient separator) -->
  <svg viewBox="0 0 340 28" width="270" height="24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
    <style>
      .d{ transform-origin: center; animation: grow 1.6s ease-in-out infinite; opacity:.95; }
      .d:nth-child(1){ animation-delay:-1.4s; fill:#fff000; filter:url(#s); }
      .d:nth-child(2){ animation-delay:-1.2s; fill:#76ff03; filter:url(#s); }
      .d:nth-child(3){ animation-delay:-1.0s; fill:#f06292; filter:url(#s); }
      .d:nth-child(4){ animation-delay:-0.8s; fill:#4fc3f7; filter:url(#s); }
      .d:nth-child(5){ animation-delay:-0.6s; fill:#ba68c8; filter:url(#s); }
      .d:nth-child(6){ animation-delay:-0.4s; fill:#f57c00; filter:url(#s); }
      .d:nth-child(7){ animation-delay:-0.2s; fill:#673ab7; filter:url(#s); }
      @keyframes grow { 0%,40%,100%{ transform:scale(.35) } 20%{ transform:scale(1) } }
    </style>
    <defs>
      <filter id="s"><feGaussianBlur stdDeviation="1.4"/></filter>
    </defs>
    <g transform="translate(14,14)">
      <circle class="d" r="7" cx="0"/>
      <circle class="d" r="7" cx="48"/>
      <circle class="d" r="7" cx="96"/>
      <circle class="d" r="7" cx="144"/>
      <circle class="d" r="7" cx="192"/>
      <circle class="d" r="7" cx="240"/>
      <circle class="d" r="7" cx="288"/>
    </g>
  </svg>
</p>

# 👋 こんにちは、Biomasaya です！

理系大学院生で、生体医工学や動作解析、筋骨格モデリングに取り組んでいます。  
このリポジトリでは、以下のような研究・プロジェクトを公開していきます。

<!-- Barcode-like divider (CSS Animated Barcode idea) -->
<p align="center">
  <svg viewBox="0 0 800 85" width="88%" height="80" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
    <defs>
      <style>
        .b line{ stroke:#e5f0f2; stroke-width:var(--w,3); opacity:.8 }
        .b text{ font: 400 22px/1.2 "Libre Barcode 128 Text","Open Sans",system-ui,sans-serif; fill:#9fb6c1; letter-spacing:.18em }
        /* subtle scan animation */
        .scan{ stroke:#a7dff0; stroke-width:2; opacity:.35; animation:slide 2.8s ease-out infinite }
        @keyframes slide{ 0%,90%{ transform:translateX(-820px) } 100%{ transform:translateX(0) } }
      </style>
    </defs>
    <g class="b" transform="translate(30,15)">
      <!-- bars -->
      <!-- a handful of varying widths to mimic barcode -->
      <line x1="0" y1="0" x2="0" y2="55" style="--w:5"/>
      <line x1="9" y1="0" x2="9" y2="55"/>
      <line x1="16" y1="0" x2="16" y2="55" style="--w:2"/>
      <line x1="24" y1="0" x2="24" y2="55" style="--w:6"/>
      <line x1="36" y1="0" x2="36" y2="55" style="--w:2"/>
      <line x1="44" y1="0" x2="44" y2="55" style="--w:4"/>
      <line x1="54" y1="0" x2="54" y2="55" style="--w:2"/>
      <line x1="62" y1="0" x2="62" y2="55" style="--w:7"/>
      <line x1="75" y1="0" x2="75" y2="55" style="--w:3"/>
      <line x1="83" y1="0" x2="83" y2="55" style="--w:6"/>
      <line x1="95" y1="0" x2="95" y2="55" style="--w:2"/>
      <line x1="103" y1="0" x2="103" y2="55" style="--w:4"/>
      <line x1="113" y1="0" x2="113" y2="55"/>
      <line x1="121" y1="0" x2="121" y2="55" style="--w:6"/>
      <line x1="133" y1="0" x2="133" y2="55" style="--w:2"/>
      <!-- scanning line -->
      <g transform="translate(740,0)"><line class="scan" x1="0" y1="0" x2="0" y2="55"/></g>
      <text x="300" y="75">c o d e  t h e  w o r l d  .  i o</text>
    </g>
  </svg>
</p>

---

## 🔬 研究テーマ
- 💪 **リーチング動作における筋張力推定**（OpenSim + EMG）
- 🤖 **強化学習**による人型モデルの制御（Python + Gym）
- 🧠 **逆最適化**による運動戦略推定モデルの構築

<!-- Slim DNA animation (pure SVG 3D-ish wave) -->
<p align="center">
  <svg viewBox="0 0 820 100" width="92%" height="90" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
    <defs>
      <style>
        .d{ fill:#56d9cd }
        .t{ stroke:#b0b0b0; stroke-dasharray:2 6; opacity:.5 }
        @keyframes y { 0%{ transform:translateY(0) } 50%{ transform:translateY(-10px) } 100%{ transform:translateY(0) } }
      </style>
    </defs>
    <!-- dotted stems -->
    <g class="t">
      <!-- 18 stems -->
      <line x1="20" y1="15" x2="20" y2="85"/><line x1="60" y1="15" x2="60" y2="85"/>
      <line x1="100" y1="15" x2="100" y2="85"/><line x1="140" y1="15" x2="140" y2="85"/>
      <line x1="180" y1="15" x2="180" y2="85"/><line x1="220" y1="15" x2="220" y2="85"/>
      <line x1="260" y1="15" x2="260" y2="85"/><line x1="300" y1="15" x2="300" y2="85"/>
      <line x1="340" y1="15" x2="340" y2="85"/><line x1="380" y1="15" x2="380" y2="85"/>
      <line x1="420" y1="15" x2="420" y2="85"/><line x1="460" y1="15" x2="460" y2="85"/>
      <line x1="500" y1="15" x2="500" y2="85"/><line x1="540" y1="15" x2="540" y2="85"/>
      <line x1="580" y1="15" x2="580" y2="85"/><line x1="620" y1="15" x2="620" y2="85"/>
      <line x1="660" y1="15" x2="660" y2="85"/><line x1="700" y1="15" x2="700" y2="85"/>
    </g>
    <!-- beads moving like helix -->
    <g>
      <!-- top row -->
      <g style="animation:y 2s linear infinite">
        <circle class="d" cx="20" r="5" cy="26"/>
        <circle class="d" cx="60" r="5" cy="26"/>
        <circle class="d" cx="100" r="5" cy="26"/>
        <circle class="d" cx="140" r="5" cy="26"/>
        <circle class="d" cx="180" r="5" cy="26"/>
        <circle class="d" cx="220" r="5" cy="26"/>
        <circle class="d" cx="260" r="5" cy="26"/>
        <circle class="d" cx="300" r="5" cy="26"/>
        <circle class="d" cx="340" r="5" cy="26"/>
        <circle class="d" cx="380" r="5" cy="26"/>
        <circle class="d" cx="420" r="5" cy="26"/>
        <circle class="d" cx="460" r="5" cy="26"/>
        <circle class="d" cx="500" r="5" cy="26"/>
        <circle class="d" cx="540" r="5" cy="26"/>
        <circle class="d" cx="580" r="5" cy="26"/>
        <circle class="d" cx="620" r="5" cy="26"/>
        <circle class="d" cx="660" r="5" cy="26"/>
        <circle class="d" cx="700" r="5" cy="26"/>
      </g>
      <!-- bottom row (phase shift) -->
      <g style="animation:y 2s linear infinite; animation-delay:-1s">
        <circle class="d" cx="20" r="5" cy="74"/>
        <circle class="d" cx="60" r="5" cy="74"/>
        <circle class="d" cx="100" r="5" cy="74"/>
        <circle class="d" cx="140" r="5" cy="74"/>
        <circle class="d" cx="180" r="5" cy="74"/>
        <circle class="d" cx="220" r="5" cy="74"/>
        <circle class="d" cx="260" r="5" cy="74"/>
        <circle class="d" cx="300" r="5" cy="74"/>
        <circle class="d" cx="340" r="5" cy="74"/>
        <circle class="d" cx="380" r="5" cy="74"/>
        <circle class="d" cx="420" r="5" cy="74"/>
        <circle class="d" cx="460" r="5" cy="74"/>
        <circle class="d" cx="500" r="5" cy="74"/>
        <circle class="d" cx="540" r="5" cy="74"/>
        <circle class="d" cx="580" r="5" cy="74"/>
        <circle class="d" cx="620" r="5" cy="74"/>
        <circle class="d" cx="660" r="5" cy="74"/>
        <circle class="d" cx="700" r="5" cy="74"/>
      </g>
    </g>
  </svg>
</p>

---

## 🛠️ 使用スキル
**Languages / Tools**

| Python | OpenSim | Git & GitHub | R |
|:--:|:--:|:--:|:--:|
| PyQt / NumPy / pandas / matplotlib | 動作解析 / 最適化 / CMC / RRA | 研究記録・コード管理 | 統計 / ggplot2 |

---

## 📂 他のリポジトリ
- <a href="https://github.com/Biomasaya/trc-analyzer-gui"><b>trc-opemsim-gui</b></a>：TRCファイルを OpenSim で解析できるようにする GUI ツール

---

## 📝 Contact
- Mail: <am25057@g.kogakuin.jp>  
- GitHub: [@Biomasaya](https://github.com/Biomasaya)

<p align="center">
  <!-- Tiny footer glow -->
  <svg viewBox="0 0 600 18" width="60%" height="16" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
    <defs>
      <radialGradient id="f" cx="50%" cy="50%">
        <stop offset="0%" stop-color="#8feaff" stop-opacity=".8"/>
        <stop offset="60%" stop-color="#8feaff" stop-opacity=".15"/>
        <stop offset="100%" stop-color="transparent" stop-opacity="0"/>
      </radialGradient>
    </defs>
    <ellipse cx="300" cy="9" rx="280" ry="8" fill="url(#f)"/>
  </svg>
</p>
