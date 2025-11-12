# Ephyra
Vendo cosmeticos de beleza
<!doctype html>
<html lang="pt-PT">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Ephyra — Cosmética Premium | Loja</title>
  <meta name="description" content="Ephyra — Cosmética de alta qualidade. Produtos premium para rosto, corpo, cabelos e perfumes. Loja online clean, rápida e otimizada para SEO." />
  <link rel="canonical" href="https://example.com/" />
  <meta name="robots" content="index,follow" />

  <!-- Open Graph / Social -->
  <meta property="og:site_name" content="Ephyra" />
  <meta property="og:title" content="Ephyra — Cosmética Premium" />
  <meta property="og:description" content="Produtos cosméticos de alta qualidade. Beleza consciente, ingredientes selecionados." />
  <meta property="og:type" content="website" />
  <meta property="og:image" content="https://via.placeholder.com/1200x630.png?text=Ephyra" />

  <!-- Twitter card -->
  <meta name="twitter:card" content="summary_large_image" />

  <!-- Structured data (Organization + Website) -->
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "Store",
    "name": "Ephyra",
    "url": "https://example.com/",
    "logo": "https://via.placeholder.com/400x100.png?text=Ephyra",
    "description": "Cosmética de alta qualidade — rosto, corpo, cabelo e perfumes.",
    "sameAs": []
  }
  </script>

  <style>
    :root{
      --bg:#ffffff;--muted:#666;--accent:#0b7256;--gold:#bfa36b;--card:#fcfcfc;
      --maxw:1200px;font-family:Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{margin:0;background:var(--bg);color:#111;line-height:1.45}
    header{border-bottom:1px solid #eee;background:linear-gradient(180deg,#fff,#fbfbfb)}
    .container{max-width:var(--maxw);margin:0 auto;padding:20px}
    .nav{display:flex;align-items:center;gap:20px}
    .logo{font-weight:700;font-size:20px;color:var(--accent)}
    nav ul{list-style:none;margin:0;padding:0;display:flex;gap:12px;align-items:center}
    nav a{color:var(--muted);text-decoration:none;padding:8px;border-radius:8px}
    nav a:hover{color:#000;background:#f6f6f6}
    .search{margin-left:auto;display:flex;gap:8px;align-items:center}
    .search input{padding:8px;border:1px solid #e6e6e6;border-radius:8px}
    .hero{display:grid;grid-template-columns:1fr 420px;gap:24px;align-items:center;padding:40px 0}
    .hero h1{font-size:36px;margin:0 0 10px}
    .hero p{color:var(--muted);margin:0 0 18px}
    .cta{display:inline-block;padding:12px 18px;border-radius:12px;background:var(--accent);color:#fff;text-decoration:none}

    /* product grid */
    .grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(220px,1fr));gap:18px}
    .card{background:var(--card);border:1px solid #f0f0f0;padding:14px;border-radius:12px}
    .card img{width:100%;height:180px;object-fit:cover;border-radius:8px}
    .price{font-weight:700}
    .muted{color:var(--muted)}

    /* cart */
    .cart-btn{position:relative}
    .cart-badge{position:absolute;top:-6px;right:-6px;background:var(--gold);color:#fff;padding:3px 7px;border-radius:999px;font-size:12px}

    /* footer */
    footer{border-top:1px solid #eee;padding:30px 0;margin-top:40px;color:var(--muted)}

    /* responsive */
    @media (max-width:900px){.hero{grid-template-columns:1fr;}.search{width:100%}}
    @media (max-width:520px){.hero h1{font-size:28px}.hero p{font-size:14px}}

    /* small helpers */
    .pill{background:#f5f7f6;padding:6px 10px;border-radius:999px;font-size:13px}
    .btn{display:inline-block;padding:10px 12px;border-radius:10px;background:#111;color:#fff;text-decoration:none}
    .link-muted{color:var(--muted);text-decoration:none}

    /* account modal */
    .modal{position:fixed;left:0;right:0;top:0;bottom:0;background:rgba(0,0,0,0.3);display:none;align-items:center;justify-content:center}
    .modal.open{display:flex}
    .modal .panel{background:#fff;padding:20px;border-radius:12px;max-width:420px;width:100%}

    /* microcopy */
    .small{font-size:13px;color:var(--muted)}
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="logo">Ephyra</div>
      <nav>
        <ul>
          <li><a href="#/" data-nav>Home</a></li>
          <li><a href="#/categoria/rosto" data-nav>Rosto</a></li>
          <li><a href="#/categoria/corpo" data-nav>Corpo</a></li>
          <li><a href="#/categoria/cabelos" data-nav>Cabelos</a></li>
          <li><a href="#/categoria/perfumes" data-nav>Perfumes</a></li>
          <li><a href="#/kits" data-nav>Kits</a></li>
        </ul>
      </nav>

      <div class="search">
        <input id="q" placeholder="Pesquisar produtos..." aria-label="Pesquisar produtos" />
        <button id="searchBtn" class="pill">Pesquisar</button>
        <button id="accountBtn" aria-label="Conta" class="pill">Entrar</button>
        <button id="cartBtn" class="pill cart-btn">Carrinho <span id="cartCount" class="cart-badge">0</span></button>
      </div>
    </div>
  </header>

  <main class="container" id="app">
    <!-- SPA content injected by JS -->
  </main>

  <footer>
    <div class="container">
      <div style="display:flex;justify-content:space-between;flex-wrap:wrap;gap:20px">
        <div style="max-width:420px">
          <h3>Ephyra</h3>
          <p class="small">Cosmética de alta qualidade — ingredientes premium, fórmulas eficazes e compromisso com sustentabilidade.</p>
          <p class="small">© <span id="year"></span> Ephyra. Todos os direitos reservados.</p>
        </div>
        <div>
          <h4>Contacto</h4>
          <p class="small">email: <a href="mailto:info@ephyra.example">info@ephyra.example</a></p>
          <p class="small">Telefone: +351 900 000 000</p>
        </div>
        <div style="min-width:220px">
          <h4>Newsletter</h4>
          <form id="newsletterForm">
            <input type="email" id="newsletterEmail" placeholder="O teu email" required style="padding:8px;border-radius:8px;border:1px solid #eee;width:100%;margin-bottom:8px" />
            <button class="btn" type="submit">Subscrever</button>
            <p class="small" id="newsletterMsg"></p>
          </form>
        </div>
      </div>
    </div>
  </footer>

  <!-- Account modal -->
  <div id="modal" class="modal" role="dialog" aria-modal="true">
    <div class="panel">
      <h3 id="modalTitle">Entrar</h3>
      <div id="authArea">
        <label class="small">Email</label>
        <input id="authEmail" type="email" style="width:100%;padding:8px;margin-bottom:8px" />
        <label class="small">Senha</label>
        <input id="authPass" type="password" style="width:100%;padding:8px;margin-bottom:12px" />
        <div style="display:flex;gap:8px">
          <button id="loginBtn" class="btn">Entrar</button>
          <button id="signupBtn" class="pill">Criar conta</button>
          <button id="closeModal" class="link-muted">Cancelar</button>
        </div>
        <p class="small" id="authMsg"></p>
      </div>
    </div>
  </div>

  <script>
  // -------------------- Basic data & SEO-friendly patterns --------------------
  const SITE = { name: 'Ephyra', desc: 'Cosmética de alta qualidade — rosto, corpo, cabelo e perfumes.' };
  document.getElementById('year').textContent = new Date().getFullYear();

  // placeholder SVG image generator for product images (fast, SEO-friendly alt text)
  function svgPlaceholder(title){
    const svg = encodeURIComponent(`<svg xmlns='http://www.w3.org/2000/svg' width='1200' height='900'><rect width='100%' height='100%' fill='%23f6f6f6'/><text x='50%' y='50%' dominant-baseline='middle' text-anchor='middle' fill='%23999' font-size='36' font-family='Arial'>${title}</text></svg>`);
    return `data:image/svg+xml;charset=utf-8,${svg}`;
  }

  // -------------------- Products (sample) --------------------
  const PRODUCTS = [
    {id:'eph-rosto-01', title:'Sérum Regenerador Ephyra', category:'rosto', price:49.00, excerpt:'Sérum concentrado com vitamina C e ácido hialurónico', image:svgPlaceholder('Sérum Regenerador'), stock:20},
    {id:'eph-rosto-02', title:'Creme Hidratante Diorizante', category:'rosto', price:35.00, excerpt:'Hidratação leve, acabamento luminoso', image:svgPlaceholder('Creme Hidratante'), stock:30},
    {id:'eph-corpo-01', title:'Óleo Corporal Nutritivo', category:'corpo', price:28.00, excerpt:'Óleo seco com aroma suave, toque sedoso', image:svgPlaceholder('Óleo Corporal'), stock:25},
    {id:'eph-cabelo-01', title:'Máscara Reconstrutora', category:'cabelos', price:42.00, excerpt:'Repara fibras capilares danificadas', image:svgPlaceholder('Máscara Reconstrutora'), stock:15},
    {id:'eph-perfume-01', title:'Eau de Parfum Ephyra', category:'perfumes', price:78.00, excerpt:'Fragrância sofisticada com notas amadeiradas', image:svgPlaceholder('Eau de Parfum'), stock:10},
    {id:'eph-kit-01', title:'Kit Ritual Noturno', category:'kits', price:95.00, excerpt:'Sérum + creme + máscara — edição limitada', image:svgPlaceholder('Kit Ritual'), stock:8}
  ];

  // Categories supported (SEO-friendly slug names)
  const CATEGORIES = [
    {slug:'rosto', title:'Rosto'},
    {slug:'corpo', title:'Corpo'},
    {slug:'cabelos', title:'Cabelos'},
    {slug:'perfumes', title:'Perfumes'},
    {slug:'kits', title:'Kits'}
  ];

  // -------------------- Router / Rendering --------------------
  const app = document.getElementById('app');

  function renderHome(){
    document.title = SITE.name + ' — Loja online';
    app.innerHTML = `
      <section class="hero">
        <div>
          <h1>Beleza consciente. Resultados reais.</h1>
          <p>Ephyra combina ingredientes premium com fórmulas sustentáveis. Descobre os nossos best-sellers e rituais de beleza.</p>
          <a class="cta" href="#/categoria/rosto">Ver produtos</a>
          <div style="margin-top:18px" class="small">Frete grátis para encomendas superiores a €60. Política de devolução de 14 dias.</div>
        </div>
        <div style="background:#fafafa;padding:18px;border-radius:12px;text-align:center">
          <img src="${svgPlaceholder('Ephyra')}" alt="Ephyra — cosmética premium" style="width:100%;max-width:340px;border-radius:8px" />
        </div>
      </section>

      <section style="margin-top:28px">
        <h2>Produtos em destaque</h2>
        <div class="grid" id="productGrid"></div>
      </section>

      <section style="margin-top:28px">
        <h3>Por categorias</h3>
        <div style="display:flex;gap:8px;flex-wrap:wrap">
          ${CATEGORIES.map(c=>`<a class="pill" href="#/categoria/${c.slug}">${c.title}</a>`).join('')}
        </div>
      </section>
    `;
    renderProducts(PRODUCTS.slice(0,6));
  }

  function renderProducts(list){
    const grid = document.getElementById('productGrid');
    grid.innerHTML = list.map(p=>`
      <article class="card" data-id="${p.id}">
        <img src="${p.image}" alt="${p.title}" loading="lazy" />
        <h4>${p.title}</h4>
        <div class="small muted">${p.excerpt}</div>
        <div style="display:flex;justify-content:space-between;align-items:center;margin-top:12px">
          <div class="price">€${p.price.toFixed(2)}</div>
          <div>
            <button class="pill" onclick="addToCart('${p.id}',1)">Adicionar</button>
            <a class="link-muted" href="#/produto/${p.id}" style="margin-left:8px">Detalhes</a>
          </div>
        </div>
      </article>`).join('');
  }

  function renderCategory(slug){
    const cat = CATEGORIES.find(c=>c.slug===slug);
    document.title = `${SITE.name} — ${cat ? cat.title : 'Categoria'}`;
    const list = PRODUCTS.filter(p=>p.category===slug);
    app.innerHTML = `<section><h2>${cat ? cat.title : 'Categoria'}</h2><div class="grid" id="productGrid"></div></section>`;
    renderProducts(list);
  }

  function renderProduct(id){
    const p = PRODUCTS.find(x=>x.id===id);
    if(!p){app.innerHTML='<p>Produto não encontrado.</p>';return}
    document.title = `${p.title} — ${SITE.name}`;
    app.innerHTML = `
      <section style="display:grid;grid-template-columns:1fr 360px;gap:20px">
        <div>
          <img src="${p.image}" alt="${p.title}" style="width:100%;max-height:560px;object-fit:cover;border-radius:10px" />
          <h2 style="margin-top:12px">${p.title}</h2>
          <p class="small muted">${p.excerpt}</p>
          <h3>Descrição</h3>
          <p class="small">Descrição detalhada do produto. Ingredientes: água, glicerina, extratos naturais, conservantes aprovados. Uso: aplique diariamente conforme necessidade.</p>
        </div>
        <aside class="card">
          <div class="price">€${p.price.toFixed(2)}</div>
          <p class="small">Stock: ${p.stock}</p>
          <div style="margin-top:12px">
            <label class="small">Quantidade</label>
            <input id="qty" type="number" value="1" min="1" max="${p.stock}" style="width:100%;padding:8px;border-radius:8px;border:1px solid #eee;margin-bottom:8px" />
            <button class="btn" onclick="addToCart('${p.id}',parseInt(document.getElementById('qty').value||1))">Adicionar ao carrinho</button>
          </div>
          <div style="margin-top:10px" class="small muted">Entrega em 2-5 dias úteis. Devolução em 14 dias.</div>
        </aside>
      </section>
    `;
  }

  // -------------------- Cart (localStorage-based) --------------------
  function getCart(){
    return JSON.parse(localStorage.getItem('ephyra_cart')||'{}');
  }
  function saveCart(cart){
    localStorage.setItem('ephyra_cart',JSON.stringify(cart));
    updateCartCount();
  }
  function addToCart(id,q){
    const p = PRODUCTS.find(x=>x.id===id); if(!p) return alert('Produto não encontrado');
    const cart = getCart();
    cart[id] = (cart[id]||0) + q;
    if(cart[id] > p.stock) cart[id] = p.stock;
    saveCart(cart);
    alert('Adicionado ao carrinho');
  }
  function updateCartCount(){
    const cart = getCart();
    const total = Object.values(cart).reduce((s,n)=>s+n,0);
    document.getElementById('cartCount').textContent = total;
  }

  function renderCart(){
    const cart = getCart();
    const items = Object.keys(cart).map(id=>{const p=PRODUCTS.find(x=>x.id===id);return {p,qty:cart[id]}});
    document.title = SITE.name + ' — Carrinho';
    app.innerHTML = `
      <section>
        <h2>O teu carrinho</h2>
        <div id="cartArea"></div>
      </section>
    `;
    const area = document.getElementById('cartArea');
    if(items.length===0){area.innerHTML='<p>O carrinho está vazio.</p>';return}
    area.innerHTML = items.map(it=>`
      <div style="display:flex;gap:12px;align-items:center;margin-bottom:12px;border-bottom:1px solid #f3f3f3;padding-bottom:12px">
        <img src="${it.p.image}" alt="${it.p.title}" style="width:100px;height:70px;object-fit:cover;border-radius:8px" />
        <div style="flex:1">
          <strong>${it.p.title}</strong>
          <div class="small muted">€${it.p.price.toFixed(2)} × ${it.qty} = €${(it.p.price*it.qty).toFixed(2)}</div>
        </div>
        <div style="display:flex;flex-direction:column;gap:8px">
          <input type="number" min="1" max="${it.p.stock}" value="${it.qty}" onchange="changeQty('${it.p.id}',this.value)" style="width:80px;padding:6px;border-radius:8px;border:1px solid #eee" />
          <button class="pill" onclick="removeItem('${it.p.id}')">Remover</button>
        </div>
      </div>
    `).join('');

    const total = items.reduce((s,it)=>s + it.p.price*it.qty,0);
    area.innerHTML += `<div style="margin-top:12px"><strong>Total: €${total.toFixed(2)}</strong></div>`;
    area.innerHTML += `<div style="margin-top:12px"><button class="btn" onclick="checkout()">Finalizar encomenda</button></div>`;
  }

  function changeQty(id,val){
    const cart = getCart(); cart[id]=parseInt(val)||1; saveCart(cart); renderCart();
  }
  function removeItem(id){ const cart=getCart(); delete cart[id]; saveCart(cart); renderCart(); }

  // -------------------- Checkout (placeholder) --------------------
  function checkout(){
    // In a production site you'd redirect to a real checkout (Stripe, PayPal) or submit to your backend.
    // Here we simulate a successful checkout and clear cart.
    if(!confirm('Simular checkout — confirmar encomenda?')) return;
    localStorage.removeItem('ephyra_cart'); updateCartCount();
    app.innerHTML = `<section><h2>Obrigado pela tua encomenda!</h2><p class="small">Isto é uma simulação de checkout. Para aceitar pagamentos reais integra Stripe/PayPal + backend seguro.</p></section>`;
  }

  // -------------------- Simple Account (localStorage mock) --------------------
  function openModal(){ document.getElementById('modal').classList.add('open'); }
  function closeModal(){ document.getElementById('modal').classList.remove('open'); document.getElementById('authMsg').textContent=''; }

  function signup(email,pass){ if(!email||!pass) return showAuthMsg('Preenche email e senha');
    const users = JSON.parse(localStorage.getItem('ephyra_users')||'{}');
    if(users[email]) return showAuthMsg('Conta já existe, por favor entra.');
    users[email]= {pass:pass}; localStorage.setItem('ephyra_users',JSON.stringify(users));
    localStorage.setItem('ephyra_user',email); showAuthMsg('Conta criada. Estás logado.'); closeModal(); updateAccountUI();
  }
  function login(email,pass){ const users=JSON.parse(localStorage.getItem('ephyra_users')||'{}'); if(users[email] && users[email].pass===pass){localStorage.setItem('ephyra_user',email); showAuthMsg('Login bem sucedido'); closeModal(); updateAccountUI();} else showAuthMsg('Email ou senha inválidos'); }
  function logout(){ localStorage.removeItem('ephyra_user'); updateAccountUI(); alert('Saíste da conta.'); }
  function showAuthMsg(m){ document.getElementById('authMsg').textContent = m; }
  function updateAccountUI(){ const user = localStorage.getItem('ephyra_user'); const btn = document.getElementById('accountBtn'); if(user) btn.textContent = user; else btn.textContent='Entrar'; }

  // -------------------- Search & Nav --------------------
  function search(q){ q = (q||'').trim().toLowerCase(); if(!q) return renderHome(); const results = PRODUCTS.filter(p=> (p.title+p.excerpt).toLowerCase().includes(q)); document.title = `Pesquisar: ${q} — ${SITE.name}`; app.innerHTML = `<section><h2>Resultados para "${q}"</h2><div class="grid" id="productGrid"></div></section>`; renderProducts(results); }

  // Simple hash router
  function router(){
    const hash = location.hash.replace('#','')||'/';
    const parts = hash.split('/').filter(Boolean);
    if(hash==='/'||hash==='') return renderHome();
    if(parts[0]==='categoria' && parts[1]) return renderCategory(parts[1]);
    if(parts[0]==='produto' && parts[1]) return renderProduct(parts[1]);
    if(parts[0]==='carrinho' || parts[0]==='cart') return renderCart();
    if(parts[0]==='kits') return renderCategory('kits');
    // fallback
    renderHome();
  }

  // -------------------- Events --------------------
  document.getElementById('searchBtn').addEventListener('click',()=>search(document.getElementById('q').value));
  document.getElementById('q').addEventListener('keyup',(e)=>{ if(e.key==='Enter') search(e.target.value); });
  document.getElementById('cartBtn').addEventListener('click',()=>{ location.hash='#/carrinho'; router(); });
  document.getElementById('accountBtn').addEventListener('click',()=>{ openModal(); });
  document.getElementById('closeModal').addEventListener('click',closeModal);
  document.getElementById('loginBtn').addEventListener('click',()=>{ login(document.getElementById('authEmail').value, document.getElementById('authPass').value); });
  document.getElementById('signupBtn').addEventListener('click',()=>{ signup(document.getElementById('authEmail').value, document.getElementById('authPass').value); });

  document.getElementById('newsletterForm').addEventListener('submit',e=>{
    e.preventDefault(); const email = document.getElementById('newsletterEmail').value; if(!email) return; const list = JSON.parse(localStorage.getItem('ephyra_news')||'[]'); list.push({email,ts:Date.now()}); localStorage.setItem('ephyra_news',JSON.stringify(list)); document.getElementById('newsletterMsg').textContent='Obrigado! Verifica o teu email.'; document.getElementById('newsletterEmail').value='';
  });

  window.addEventListener('hashchange',router);
  window.addEventListener('load',()=>{ router(); updateCartCount(); updateAccountUI(); });

  // Expose some functions for inline handlers
  window.addToCart = addToCart; window.changeQty = changeQty; window.removeItem = removeItem; window.checkout = checkout;
  </script>
</body>
</html>
