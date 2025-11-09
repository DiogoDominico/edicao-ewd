<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>EWD Investimentos</title>
  <style>
    :root{
      --azul: #002e5b;
      --dourado: #d4af37;
      --fundo: #f8f8f8;
      --card-bg: #ffffff;
      --texto: #333;
    }
    *{box-sizing:border-box;}
    body{ margin:0; font-family:"Segoe UI", Tahoma, Geneva, Verdana, sans-serif; background:var(--fundo); color:var(--texto); }

    /* cabeçalho */
    header.site-header{
      background:var(--azul);
      padding:16px 24px;
      display:flex;
      align-items:center;
      gap:16px;
    }
    .logo-wrap{
      width: auto;
      height: 60px;
      display:flex;
      align-items:center;
    }
    img.logo{
      height:100%;
      width:auto;
      display:block;
      object-fit:contain;
      border-radius:4px;
    }
    /* fallback text (quando imagem não carregar) */
    .logo-fallback{
      display:none; /* ativado via JS se necessário */
      height:100%;
      padding:8px 12px;
      background:var(--dourado);
      color:var(--azul);
      font-weight:700;
      border-radius:6px;
      align-items:center;
      justify-content:center;
      font-size:1rem;
    }

    header.site-header h1{
      margin:0;
      font-size:20px;
      color:var(--dourado);
      letter-spacing:0.2px;
    }

    /* resto do layout (resumido) */
    .container{ max-width:1100px; margin:28px auto; padding:0 20px; }
    .hero{ background:var(--card-bg); border-radius:12px; padding:32px; box-shadow:0 8px 24px rgba(0,0,0,0.06); }
    .lead{ color:var(--azul); font-size:1.25rem; margin:0 0 12px 0; font-weight:600; }
    .card{ background:var(--card-bg); border-radius:12px; padding:20px; margin-top:20px; box-shadow:0 6px 20px rgba(0,0,0,0.05); }
    .parceiros ul{ list-style:none; padding:0; margin:0; display:flex; flex-wrap:wrap; gap:10px; }
    .parceiros li{ background:#f3f3f3; padding:8px 12px; border-radius:8px; color:var(--azul); font-weight:600; border:1px solid #e6e6e6; }
    .formulario form{ display:flex; flex-direction:column; gap:12px; max-width:680px; }
    input, textarea{ padding:12px; border:1px solid #d0d0d0; border-radius:8px; font-size:16px; width:100%; background:white; }
    input:focus, textarea:focus{ border-color:var(--dourado); box-shadow:0 0 0 4px rgba(212,175,55,0.12); outline:none; }
    .cta{ text-align:center; margin-top:26px; padding:28px; border-radius:12px; background:linear-gradient(180deg,rgba(0,46,91,0.98),rgba(0,46,91,0.95)); color:white; }
    .cta-btn{ background:var(--dourado); color:var(--azul); border:none; padding:12px 20px; border-radius:999px; font-weight:700; cursor:pointer; margin-top:12px; }

    footer{ background:var(--azul); color:white; padding:18px 10px; text-align:center; margin-top:36px; font-size:14px; }

    @media (max-width:700px){
      header.site-header{ padding:12px; }
      header.site-header h1{ font-size:18px; }
      header.site-header img.logo{ height:48px; }
    }
  </style>
</head>
<body>
  <header class="site-header" role="banner">
    <div class="logo-wrap" id="logoWrap">
      <!-- Imagem principal; se falhar, onerror troca para data URI SVG (fallback visual) -->
      <img
        class="logo"
        id="logoImg"
        src="logo-ewd.jpg"
        alt="Logo EWD Investimentos"
        onerror="handleLogoError(this)"
      />
      <div class="logo-fallback" id="logoFallback" aria-hidden="true">EWD Investimentos</div>
    </div>
    <h1>EWD Investimentos</h1>
  </header>

  <main class="container" role="main">
    <section class="hero" aria-label="Apresentação">
      <p class="lead">O modelo de gestão de patrimônio mais bem-sucedido no mundo, agora disponível para você.</p>
      <p>Na <strong>EWD Investimentos</strong>, oferecemos uma abordagem personalizada para atender aos seus objetivos financeiros, com transparência e alinhamento total aos seus interesses.</p>
    </section>

    <section class="card parceiros" aria-label="Parceiros">
      <h2 style="margin-top:0;color:#002e5b;">Parceiros</h2>
      <ul>
        <li>BTG Pactual</li><li>XP Investimentos</li><li>Warren</li><li>Avenue</li><li>Interactive Brokers</li>
      </ul>
    </section>

    <section class="card faq" aria-label="Perguntas Frequentes">
      <h2 style="margin-top:0;color:#002e5b;">Perguntas Frequentes</h2>
      <p><strong>Qual o valor mínimo para ser cliente?</strong><br/>Atendemos clientes com patrimônio a partir de R$ 100.000,00.</p>
      <p><strong>Como é feita a cobrança?</strong><br/>Cobramos uma taxa mensal baseada no valor atual da sua carteira, alinhando nossos interesses aos seus.</p>
      <p><strong>Preciso sair da minha assessoria atual?</strong><br/>Sim — nosso modelo exige relação direta para garantir atendimento exclusivo.</p>
    </section>

    <section class="card formulario" aria-label="Formulário de contato">
      <h2 style="margin-top:0;color:#002e5b;">Agende sua Consultoria</h2>
      <form action="https://formspree.io/f/xgvkgdzw" method="POST" class="formulario" novalidate>
        <input type="text" name="nome" placeholder="Seu nome completo" required />
        <input type="email" name="email" placeholder="Seu e-mail" required />
        <input type="tel" name="telefone" placeholder="Seu telefone" required />
        <textarea name="mensagem" rows="4" placeholder="Mensagem ou dúvida (opcional)"></textarea>
        <button type="submit">Enviar</button>
      </form>
    </section>

    <section class="cta" aria-label="Chamada para ação">
      <h2 style="margin:0;font-size:1.15rem;">Pronto para transformar a gestão do seu patrimônio?</h2>
      <p style="opacity:.95;margin:8px 0 0;">Agende uma consultoria gratuita e descubra o poder de uma gestão realmente personalizada.</p>
      <button class="cta-btn" onclick="document.querySelector('.formulario form')?.scrollIntoView({behavior:'smooth'});">Agendar Consultoria</button>
    </section>
  </main>

  <footer role="contentinfo">
    <div>&copy; 2025 EWD Investimentos. Todos os direitos reservados.</div>
    <div style="opacity:.9;margin-top:6px;">Política de Privacidade | Termos de Uso | Contato: ewdparticipacoes@hotmail.com</div>
  </footer>

  <script>
    // Se a logo não carregar, substitui por um data-uri SVG (visual simples) e mostra fallback textual
    function handleLogoError(imgEl){
      console.warn("Logo não carregou a partir de:", imgEl.src);
      // data-uri SVG simples (dourado fundo branco texto azul)
      const svg = encodeURIComponent(
        '<svg xmlns="http://www.w3.org/2000/svg" width="300" height="80"><rect width="100%" height="100%" fill="%23d4af37"/><text x="16" y="50" font-family="Segoe UI, Tahoma, Geneva, Verdana, sans-serif" font-size="28" fill="%23002e5b">EWD Investimentos</text></svg>'
      );
      imgEl.src = 'data:image/svg+xml;charset=utf-8,' + svg;
      imgEl.alt = "EWD Investimentos - logo (fallback)";
      // mostrar logo textual também (caso queira)
      const fallback = document.getElementById('logoFallback');
      if(fallback) fallback.style.display = 'flex';
    }

    // Diagnóstico rápido: logue o caminho atual
    console.log("Caminho da imagem de logo atual:", document.getElementById('logoImg')?.src || "não encontrado element#logoImg");
  </script>
</body>
</html>
