<!doctype html>
<html lang="pt-br">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Papel & Arte Brasil | Papelaria, Organização e Livros Infantis</title>
  <meta name="description" content="Loja online de papelaria, produtos de organização e livros infantis. Produtos de qualidade com entrega rápida via Mercado Livre." />
  <meta name="theme-color" content="#0b1220" />

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      background: #f4f6fb;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
      color: #111;
      line-height: 1.6;
    }

    /* ====== HEADER/NAVBAR ====== */
    .header {
      background: linear-gradient(135deg, #0b1220, #1e293b);
      padding: 12px 20px;
      position: sticky;
      top: 0;
      z-index: 100;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
    }

    .logo-mini {
      max-width: 40px;
      height: auto;
      color: #fff;
      font-weight: bold;
      font-size: 18px;
      display: flex;
      align-items: center;
    }

    .header-nav {
      display: flex;
      gap: 15px;
      align-items: center;
    }

    .header-nav a {
      color: #fff;
      text-decoration: none;
      font-size: 13px;
      padding: 8px 12px;
      border-radius: 6px;
      transition: 0.2s;
    }

    .header-nav a:hover {
      background: rgba(255, 255, 255, 0.1);
    }

    /* ====== BANNER TOPO ====== */
    .banner-topo {
      background: linear-gradient(135deg, #0b1220, #1e293b);
      padding: 50px 20px;
      text-align: center;
      color: #fff;
    }

    .banner-topo img {
      max-width: 220px;
      width: 100%;
      margin-bottom: 14px;
      border-radius: 12px;
    }

    .banner-topo h1 {
      font-size: clamp(28px, 6vw, 42px);
      margin: 10px 0 8px;
      font-weight: 700;
    }

    .banner-topo p {
      font-size: clamp(14px, 3vw, 18px);
      opacity: 0.95;
      margin: 0 0 6px;
    }

    .banner-sub {
      font-size: 13px;
      opacity: 0.8;
      margin: 8px 0 0;
    }

    .banner-btn {
      display: inline-block;
      margin-top: 20px;
      padding: 14px 32px;
      background: #ff6a00;
      color: #fff;
      text-decoration: none;
      border-radius: 12px;
      font-weight: 700;
      font-size: 15px;
      border: none;
      cursor: pointer;
      transition: 0.3s ease;
      box-shadow: 0 4px 15px rgba(255, 106, 0, 0.3);
    }

    .banner-btn:hover {
      background: #ff5500;
      transform: translateY(-2px);
      box-shadow: 0 6px 20px rgba(255, 106, 0, 0.4);
    }

    /* ====== TRUST SECTION ====== */
    .trust-section {
      background: #fff;
      padding: 25px 20px;
      display: flex;
      justify-content: center;
      gap: 30px;
      flex-wrap: wrap;
      font-size: 13px;
      color: #444;
      border-bottom: 1px solid rgba(0, 0, 0, 0.06);
    }

    .trust-item {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .trust-item-icon {
      font-size: 24px;
    }

    /* ====== VITRINE ====== */
    .store-wrap {
      max-width: 1100px;
      margin: 35px auto;
      padding: 0 15px;
    }

    .store-header {
      display: flex;
      gap: 15px;
      flex-wrap: wrap;
      align-items: flex-end;
      justify-content: space-between;
      margin-bottom: 20px;
    }

    .store-header > div:first-child {
      flex: 1;
      min-width: 200px;
    }

    .store-title {
      margin: 0;
      font-size: clamp(24px, 5vw, 32px);
      color: #0b1220;
      font-weight: 700;
    }

    .store-sub {
      margin: 6px 0 0;
      color: #666;
      font-size: 14px;
    }

    .controls {
      display: flex;
      gap: 10px;
      flex-wrap: wrap;
      min-width: 100%;
    }

    @media (min-width: 768px) {
      .controls {
        min-width: auto;
        flex-wrap: nowrap;
      }
    }

    .inp,
    .sel {
      padding: 12px 14px;
      border-radius: 10px;
      border: 1px solid rgba(0, 0, 0, 0.12);
      outline: none;
      background: #fff;
      font-family: inherit;
      font-size: 14px;
      transition: 0.2s;
      flex: 1;
      min-width: 180px;
    }

    .inp:focus,
    .sel:focus {
      border-color: #ff6a00;
      box-shadow: 0 0 0 3px rgba(255, 106, 0, 0.1);
    }

    .pillbar {
      display: flex;
      gap: 10px;
      flex-wrap: wrap;
      margin: 16px 0 20px;
    }

    .pill {
      background: #fff;
      border: 1px solid rgba(0, 0, 0, 0.08);
      border-radius: 999px;
      padding: 8px 14px;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
      font-size: 12px;
      color: #333;
      font-weight: 500;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
      gap: 16px;
      margin-bottom: 30px;
    }

    @media (max-width: 600px) {
      .grid {
        grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
        gap: 12px;
      }
    }

    .card {
      background: #fff;
      border-radius: 14px;
      overflow: hidden;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.06);
      border: 1px solid rgba(0, 0, 0, 0.05);
      display: flex;
      flex-direction: column;
      transition: 0.3s ease;
      position: relative;
    }

    .card:hover {
      transform: translateY(-6px);
      box-shadow: 0 12px 24px rgba(0, 0, 0, 0.1);
    }

    .img-wrapper {
      position: relative;
      width: 100%;
      height: 160px;
      overflow: hidden;
      background: linear-gradient(135deg, #f3f4f6, #e5e7eb);
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      display: block;
      transition: 0.3s ease;
    }

    .img.loaded {
      animation: fadeIn 0.3s ease-in;
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    .card:hover .img {
      transform: scale(1.05);
    }

    .img-placeholder {
      font-size: 48px;
      color: #999;
    }

    .loading-spinner {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 30px;
      height: 30px;
      border: 3px solid #f3f3f3;
      border-top: 3px solid #ff6a00;
      border-radius: 50%;
      animation: spin 0.8s linear infinite;
    }

    @keyframes spin {
      0% { transform: translate(-50%, -50%) rotate(0deg); }
      100% { transform: translate(-50%, -50%) rotate(360deg); }
    }

    .badge {
      position: absolute;
      top: 10px;
      right: 10px;
      background: #ff6a00;
      color: #fff;
      padding: 4px 10px;
      border-radius: 6px;
      font-size: 11px;
      font-weight: 700;
      text-transform: uppercase;
      z-index: 2;
    }

    .content {
      padding: 12px;
      flex: 1;
      display: flex;
      flex-direction: column;
    }

    .tag {
      display: inline-block;
      font-size: 11px;
      font-weight: 700;
      padding: 4px 8px;
      border-radius: 6px;
      background: #eef2ff;
      color: #1e293b;
      margin-bottom: 6px;
      width: fit-content;
    }

    .name {
      margin: 0 0 4px;
      font-size: 14px;
      font-weight: 600;
      color: #0b1220;
      line-height: 1.3;
      min-height: 2.6em;
      display: -webkit-box;
      -webkit-line-clamp: 2;
      -webkit-box-orient: vertical;
      overflow: hidden;
    }

    .meta {
      margin: 0;
      color: #666;
      font-size: 12px;
      line-height: 1.4;
    }

    .actions {
      padding: 10px;
      border-top: 1px solid rgba(0, 0, 0, 0.04);
      display: flex;
      gap: 8px;
      flex-wrap: wrap;
    }

    .btn {
      flex: 1;
      min-width: 90px;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 10px 12px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: 700;
      font-size: 12px;
      border: none;
      cursor: pointer;
      transition: 0.2s ease;
      text-align: center;
    }

    .buy {
      background: #ff6a00;
      color: #fff;
    }

    .buy:hover {
      background: #ff5500;
      transform: translateY(-1px);
    }

    .view {
      background: #f0f0f0;
      color: #0b1220;
      border: 1px solid #ddd;
    }

    .view:hover {
      background: #e0e0e0;
    }

    /* ====== EMPTY STATE ====== */
    .empty {
      padding: 40px 20px;
      background: #fff;
      border: 2px dashed rgba(0, 0, 0, 0.12);
      border-radius: 14px;
      color: #666;
      text-align: center;
      font-size: 14px;
      margin-bottom: 30px;
      display: none;
    }

    .empty-icon {
      font-size: 48px;
      margin-bottom: 12px;
    }

    /* ====== CTA SECTION ====== */
    .cta-section {
      background: linear-gradient(135deg, #0b1220, #1e293b);
      color: #fff;
      padding: 40px 20px;
      text-align: center;
      border-radius: 14px;
      margin: 40px auto;
      max-width: 800px;
    }

    .cta-section h2 {
      margin: 0 0 10px;
      font-size: 24px;
      font-weight: 700;
    }

    .cta-section p {
      margin: 0 0 20px;
      font-size: 15px;
      opacity: 0.9;
    }

    .cta-btn {
      display: inline-block;
      padding: 12px 28px;
      background: #ff6a00;
      color: #fff;
      text-decoration: none;
      border-radius: 10px;
      font-weight: 700;
      transition: 0.3s ease;
    }

    .cta-btn:hover {
      background: #ff5500;
      transform: translateY(-2px);
    }

    /* ====== FOOTER ====== */
    footer {
      background: #0b1220;
      color: #aaa;
      padding: 30px 20px;
      text-align: center;
      font-size: 13px;
      margin-top: 40px;
      border-top: 1px solid rgba(255, 255, 255, 0.1);
    }

    footer a {
      color: #ff6a00;
      text-decoration: none;
      transition: 0.2s;
    }

    footer a:hover {
      text-decoration: underline;
    }

    .footer-content {
      max-width: 1100px;
      margin: 0 auto;
    }

    .social-links {
      margin: 15px 0;
      font-size: 14px;
    }

    .social-links a {
      margin: 0 12px;
      display: inline-block;
    }

    /* ====== RESPONSIVE ====== */
    @media (max-width: 600px) {
      .store-header {
        flex-direction: column;
        align-items: stretch;
      }

      .store-header > div:first-child {
        min-width: auto;
      }

      .controls {
        flex-direction: column;
      }

      .inp,
      .sel {
        min-width: 100%;
      }

      .banner-topo {
        padding: 35px 15px;
      }

      .header {
        flex-direction: column;
        gap: 10px;
      }

      .trust-section {
        gap: 15px;
      }

      .pill {
        font-size: 11px;
      }
    }

    /* ====== ACCESSIBILITY ====== */
    a:focus,
    button:focus {
      outline: 2px solid #ff6a00;
      outline-offset: 2px;
    }

    @media (prefers-reduced-motion: reduce) {
      * {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
      }
    }
  </style>
</head>

<body>

  <!-- ====== STICKY HEADER ====== -->
  <header class="header">
    <div class="logo-mini">📦 Papel & Arte</div>
    <nav class="header-nav">
      <a href="#vitrine">Produtos</a>
      <a href="#contato">Contato</a>
    </nav>
  </header>

  <!-- ====== BANNER COM LOGO ====== -->
  <section class="banner-topo">
    <img src="logo.jpg" alt="Papel & Arte Brasil - Papelaria, Organização e Livros Infantis">
    <h1>Papel & Arte Brasil</h1>
    <p>Sua vitrine online de papelaria, organização e livros infantis</p>
    <p class="banner-sub">📦 Produtos selecionados com entrega rápida via Mercado Livre</p>
    <a href="#vitrine" class="banner-btn">🛍️ Ver Produtos</a>
  </section>

  <!-- ====== TRUST SIGNALS ====== -->
  <section class="trust-section">
    <div class="trust-item">
      <span class="trust-item-icon">🔒</span>
      <span><strong>Compra Segura</strong> via Mercado Livre</span>
    </div>
    <div class="trust-item">
      <span class="trust-item-icon">⚡</span>
      <span><strong>Links Diretos</strong> e Confiáveis</span>
    </div>
    <div class="trust-item">
      <span class="trust-item-icon">📦</span>
      <span><strong>Entrega Rápida</strong> Garantida</span>
    </div>
  </section>

  <!-- ====== VITRINE (LINKS MERCADO LIVRE) ====== -->
  <section id="vitrine" class="store-wrap">
    <div class="store-header">
      <div>
        <h2 class="store-title">🛍️ Catálogo de Produtos</h2>
        <p class="store-sub">Clique em "Comprar" para ir direto ao Mercado Livre</p>
      </div>

      <div class="controls">
        <input 
          id="q" 
          class="inp" 
          type="search"
          placeholder="Buscar (ex: caneta, livro, organizador)..." 
          aria-label="Buscar produtos"
        />
        <select id="cat" class="sel" aria-label="Filtrar por categoria">
          <option value="Todos">Todas as categorias</option>
          <option value="Produtos Diversos">Produtos Diversos</option>
          <option value="Revistas Infantis / Livros de Colorir">Revistas Infantis / Livros de Colorir</option>
        </select>
      </div>
    </div>

    <div class="pillbar">
      <div class="pill">✅ Produtos de qualidade selecionados</div>
      <div class="pill">🚀 Atualização frequente do catálogo</div>
      <div class="pill">💳 Múltiplas formas de pagamento</div>
    </div>

    <div id="grid" class="grid"></div>
    <div id="empty" class="empty">
      <div class="empty-icon">🔍</div>
      <p><strong>Nenhum item encontrado</strong> com esse filtro ou busca.<br>Tente outros termos ou categorias.</p>
    </div>
  </section>

  <!-- ====== CTA SECTION ====== -->
  <section class="cta-section">
    <h2>Não encontrou o que procura?</h2>
    <p>Entre em contato conosco e sugira produtos para nosso catálogo!</p>
    <a href="https://www.instagram.com/papel_arte_brasil" class="cta-btn" target="_blank">📱 Siga-nos no Instagram</a>
  </section>

  <!-- ====== FOOTER ====== -->
  <footer id="contato">
    <div class="footer-content">
      <p><strong>Papel & Arte Brasil</strong></p>
      <p>Sua loja online de papelaria, organização e livros infantis</p>
      
      <div class="social-links">
        <a href="https://www.instagram.com/papel_arte_brasil" target="_blank" rel="noopener noreferrer">📱 Instagram</a>
        <a href="https://www.mercadolivre.com.br" target="_blank" rel="noopener noreferrer">🛒 Mercado Livre</a>
      </div>

      <p style="margin-top: 20px; font-size: 12px;">
        © 2026 Papel & Arte Brasil • Todos os direitos reservados<br>
        Desenvolvido com ❤️ para oferecer a melhor experiência
      </p>
    </div>
  </footer>

  <script>
    // ===== FUNÇÃO PARA EXTRAIR IMAGEM DO MERCADO LIVRE =====
    async function fetchProductImage(meliLink) {
      try {
        // Converte link encurtado para URL completa se necessário
        let fullUrl = meliLink;
        if (meliLink.includes('meli.la/')) {
          // Segue o redirect para obter URL completa
          const response = await fetch(meliLink, { 
            method: 'HEAD',
            mode: 'no-cors'
          });
          fullUrl = response.url || meliLink;
        }

        // Extrai ID do produto da URL
        const productId = meliLink.match(/(\d+)/)?.[1];
        if (!productId) return null;

        // Tenta usar API de proxy para buscar dados do produto
        // Nota: Isso funciona melhor com a API oficial do Mercado Livre
        const apiUrl = `https://api.mercadolibre.com/items/${productId}`;
        
        try {
          const response = await fetch(apiUrl, { mode: 'cors' });
          const data = await response.json();
          
          if (data.pictures && data.pictures.length > 0) {
            return data.pictures[0].url;
          }
        } catch (e) {
          console.log('API indisponível para:', productId);
        }

        return null;
      } catch (error) {
        console.error('Erro ao buscar imagem:', error);
        return null;
      }
    }

    // ===== DADOS DE PRODUTOS =====
    const items = [
      // ===== PRODUTOS DIVERSOS =====
      { cat: "Produtos Diversos", name: "Produto 01", link: "https://meli.la/11LGGc5", img: "" },
      { cat: "Produtos Diversos", name: "Produto 02", link: "https://meli.la/2do4Yg8", img: "" },
      { cat: "Produtos Diversos", name: "Produto 03", link: "https://meli.la/15DpzQr", img: "" },
      { cat: "Produtos Diversos", name: "Produto 04", link: "https://meli.la/2w2Xv4J", img: "" },
      { cat: "Produtos Diversos", name: "Produto 05", link: "https://meli.la/2oAqtqP", img: "" },
      { cat: "Produtos Diversos", name: "Produto 06", link: "https://meli.la/1KEDQ3g", img: "" },
      { cat: "Produtos Diversos", name: "Produto 07", link: "https://meli.la/1g23fCu", img: "" },
      { cat: "Produtos Diversos", name: "Produto 08", link: "https://meli.la/1Doedt7", img: "" },
      { cat: "Produtos Diversos", name: "Produto 09", link: "https://meli.la/32cRb4B", img: "" },
      { cat: "Produtos Diversos", name: "Produto 10", link: "https://meli.la/2G5Q5Vt", img: "" },
      { cat: "Produtos Diversos", name: "Produto 11", link: "https://meli.la/1j9a5Q2", img: "" },
      { cat: "Produtos Diversos", name: "Produto 12", link: "https://meli.la/15DpzQr", img: "" },

      // ===== REVISTAS INFANTIS / LIVROS DE COLORIR =====
      { cat: "Revistas Infantis / Livros de Colorir", name: "Colorir 01", link: "https://meli.la/2QEMQH7", img: "" },
      { cat: "Revistas Infantis / Livros de Colorir", name: "Colorir 02", link: "https://meli.la/2BsmQxx", img: "" },
      { cat: "Revistas Infantis / Livros de Colorir", name: "Colorir 03", link: "https://meli.la/1yntYj6", img: "" },
      { cat: "Revistas Infantis / Livros de Colorir", name: "Colorir 04", link: "https://meli.la/1LaZx6j", img: "" },
      { cat: "Revistas Infantis / Livros de Colorir", name: "Colorir 05", link: "https://meli.la/1MGJAJi", img: "" },
      { cat: "Revistas Infantis / Livros de Colorir", name: "Colorir 06", link: "https://meli.la/1wU2npm", img: "" },
      { cat: "Revistas Infantis / Livros de Colorir", name: "Colorir 07", link: "https://meli.la/1HCHE5W", img: "" },
      { cat: "Revistas Infantis / Livros de Colorir", name: "Colorir 08", link: "https://meli.la/2M87Hzq", img: "" },
      { cat: "Revistas Infantis / Livros de Colorir", name: "Colorir 09", link: "https://meli.la/2gCLwku", img: "" },
    ];

    const grid = document.getElementById("grid");
    const empty = document.getElementById("empty");
    const q = document.getElementById("q");
    const cat = document.getElementById("cat");

    // Carrega imagens dos produtos
    async function loadProductImages() {
      for (const item of items) {
        if (!item.img) {
          const imageUrl = await fetchProductImage(item.link);
          if (imageUrl) {
            item.img = imageUrl;
            console.log(`✅ Imagem carregada para: ${item.name}`);
          } else {
            console.log(`⚠️ Imagem não encontrada para: ${item.name}`);
          }
        }
      }
      render();
    }

    function render() {
      const term = (q.value || "").trim().toLowerCase();
      const c = cat.value;

      const filtered = items.filter(it => {
        const okCat = (c === "Todos") || (it.cat === c);
        const okTerm = !term || (it.name.toLowerCase().includes(term));
        return okCat && okTerm;
      });

      grid.innerHTML = filtered.map((it, index) => `
        <article class="card" data-product="${index}">
          <div class="img-wrapper">
            <a href="${it.link}" target="_blank" rel="noopener noreferrer" style="width: 100%; height: 100%; display: flex; align-items: center; justify-content: center;">
              ${it.img ? `
                <img 
                  class="img" 
                  src="${it.img}" 
                  alt="${it.name}"
                  loading="lazy"
                  onload="this.classList.add('loaded')"
                  onerror="this.style.display='none'; this.parentElement.querySelector('.img-placeholder') && (this.parentElement.querySelector('.img-placeholder').style.display='flex')"
                >
                <div class="img-placeholder" style="display: none; width: 100%; height: 100%; align-items: center; justify-content: center;">📦</div>
              ` : `
                <div class="img-placeholder" style="display: flex; width: 100%; height: 100%; align-items: center; justify-content: center;">📦</div>
              `}
            </a>
            <span class="badge">${it.cat.split(' / ')[0]}</span>
          </div>

          <div class="content">
            <h3 class="name">${it.name}</h3>
            <p class="meta">✅ Disponível no Mercado Livre</p>
          </div>

          <div class="actions">
            <a class="btn buy" href="${it.link}" target="_blank" rel="noopener noreferrer">Comprar</a>
            <a class="btn view" href="${it.link}" target="_blank" rel="noopener noreferrer">Ver</a>
          </div>
        </article>
      `).join("");

      empty.style.display = filtered.length ? "none" : "block";
    }

    // Event listeners com debounce para search
    let searchTimeout;
    q.addEventListener("input", () => {
      clearTimeout(searchTimeout);
      searchTimeout = setTimeout(render, 300);
    });

    cat.addEventListener("change", render);

    // Carrega imagens ao iniciar
    loadProductImages();

    // Smooth scroll
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
          e.preventDefault();
          target.scrollIntoView({ behavior: 'smooth', block: 'start' });
        }
      });
    });
  </script>

</body>
</html>
