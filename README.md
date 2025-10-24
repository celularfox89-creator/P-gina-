<!doctype html>
<html lang="pt-BR">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Smart Peças — Link Page</title>
<style>
  :root{
    --red:#c81f1f;
    --dark1:#0f0f10;
    --dark2:#333;
    --card-bg: rgba(255,255,255,0.06);
    --muted: #bfbfbf;
    --radius: 10px;
    font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
  }
  html,body{height:100%;margin:0;background:linear-gradient(180deg,var(--dark1),#0b0b0b 30%, #1f1f1f 100%);color:#eee}
  .container{max-width:980px;margin:0 auto;padding:22px;}
  /* header */
  .topbar{display:flex;align-items:center;gap:12px;padding:8px 0;}
  .close{width:36px;height:36px;border-radius:50%;display:inline-flex;align-items:center;justify-content:center;background:transparent;border:2px solid rgba(255,255,255,0.06);color:#fff}
  .site-title{font-weight:600;}
  /* hero */
  .logo-wrap{display:flex;flex-direction:column;align-items:center;margin:18px 0 8px}
  .logo{
    width:110px;height:110px;border-radius:999px;background:#fff;display:flex;align-items:center;justify-content:center;
    box-shadow:0 8px 20px rgba(0,0,0,0.6);
  }
  .logo img{max-width:80%;max-height:80%}
  h1{margin:12px 0 24px;font-size:26px;letter-spacing:2px}
  /* video */
  .video-card{max-width:760px;margin:0 auto;border-radius:12px;overflow:hidden;background:var(--card-bg);box-shadow:0 6px 20px rgba(0,0,0,0.6)}
  .video-card iframe, .video-card video{width:100%;height:360px;display:block;border:0}
  /* fale conosco */
  .section-title{margin:22px 0 12px;text-align:center;font-weight:700;color:#ddd}
  .btn-row{display:flex;flex-direction:column;gap:14px;padding:0 12px}
  .btn{
    display:block;text-align:center;padding:18px;border-radius:10px;font-weight:700;text-transform:uppercase;letter-spacing:1px;
    background:var(--red);color:white;border:0;cursor:pointer;box-shadow:0 6px 18px rgba(0,0,0,0.4);
  }
  /* form / pré-cadastro */
  .form-card{margin:20px auto;padding:18px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.03), rgba(255,255,255,0.02));max-width:760px}
  .form-row{display:flex;flex-direction:column;gap:12px}
  label{font-size:13px;color:var(--muted)}
  input[type="text"], input[type="email"], textarea{
    width:100%;padding:14px;border-radius:8px;border:2px solid rgba(255,255,255,0.06);background:rgba(255,255,255,0.02);color:#fff;
    font-size:15px;outline:none;box-sizing:border-box;resize:vertical;
  }
  textarea{min-height:120px}
  .privacy{display:flex;gap:10px;align-items:flex-start;font-size:13px;color:var(--muted);margin-top:8px}
  .privacy a{color:#fff;text-decoration:underline}
  .submit{margin-top:10px;background:rgba(255,255,255,0.08);color:#ddd;padding:14px;border-radius:10px;border:0;font-weight:700;cursor:not-allowed}
  .submit.enabled{background:#3f3f3f;color:#fff;cursor:pointer}
  /* map */
  .map-wrap{margin:28px auto;max-width:760px;border-radius:14px;overflow:hidden;border:1px solid rgba(255,255,255,0.04)}
  .map-wrap iframe{width:100%;height:220px;border:0;display:block}
  /* footer big CTA */
  .big-cta{margin:40px 0;text-align:center;font-size:44px;font-weight:800;color:rgba(255,255,255,0.12);letter-spacing:2px}
  /* floating actions */
  .fab{
    position:fixed;left:18px;bottom:18px;background:#e6f0f0;padding:12px 18px;border-radius:999px;box-shadow:0 10px 30px rgba(0,0,0,0.5);
    display:flex;gap:12px;align-items:center
  }
  .fab button{background:transparent;border:0;padding:10px;border-radius:8px;font-weight:700}
  /* responsiveness */
  @media(min-width:720px){
    .btn-row{flex-direction:row}
    .btn{flex:1}
    .video-card iframe, .video-card video{height:420px}
    .form-row{flex-direction:row}
    .form-row > *{flex:1}
  }
</style>
</head>
<body>
  <div class="container">
    <header class="topbar" role="banner" aria-label="Top bar">
      <div class="close" aria-hidden="true">✕</div>
      <div>
        <div style="font-size:13px;color:#cfcfcf">Instagram · lnK.bio</div>
        <div class="site-title">SMART PEÇAS</div>
      </div>
    </header>

    <main>
      <div class="logo-wrap" role="img" aria-label="Logotipo Smart Peças">
        <div class="logo">
          <!-- Substitua pelo seu logo -->
          <img src="https://via.placeholder.com/120x40?text=Logo" alt="Logo Smart Peças" />
        </div>
        <h1>SMART PEÇAS</h1>
      </div>

      <!-- video -->
      <section class="video-card" aria-labelledby="video-title">
        <div style="padding:12px 14px;color:var(--muted);font-weight:600" id="video-title">Smart Peças</div>
        <!-- troque o iframe pelo seu vídeo (Vimeo/YouTube) -->
        <iframe src="https://player.vimeo.com/video/76979871" title="Vídeo institucional" allow="autoplay; fullscreen" allowfullscreen></iframe>
      </section>

      <!-- fale conosco com dois botões -->
      <div class="section-title">FALE CONOSCO</div>
      <div class="btn-row" role="navigation" aria-label="Fale conosco opções">
        <button class="btn" onclick="scrollToForm()">Varejo</button>
        <button class="btn" onclick="scrollToForm()">Atacado</button>
      </div>

      <!-- formulário de pré-cadastro -->
      <section class="form-card" id="pre-cadastro" aria-labelledby="pre-title">
        <div id="pre-title" style="font-weight:700;margin-bottom:10px">Faça seu pré-cadastro</div>
        <form id="leadForm" class="form-row" onsubmit="handleSubmit(event)">
          <div style="display:flex;flex-direction:column;gap:12px;flex:1">
            <label for="email">seu Email</label>
            <input id="email" name="email" type="email" placeholder="seu Email" required>
            <label for="name">seu nome</label>
            <input id="name" name="name" type="text" placeholder="seu nome" required>
          </div>
          <div style="flex:1;display:flex;flex-direction:column;gap:12px">
            <label for="msg">sua mensagem</label>
            <textarea id="msg" name="message" placeholder="sua mensagem"></textarea>
          </div>

          <div style="flex-basis:100%;margin-top:8px">
            <div class="privacy">
              <input id="agree" type="checkbox" aria-describedby="privacy-desc" />
              <div id="privacy-desc">Concordo que meus dados serão processados por <strong>@smartpecas.korai</strong> de acordo com a <a href="#" target="_blank" rel="noopener">Política de Privacidade</a> deles a fim de responder à minha solicitação.</div>
            </div>
            <button type="submit" id="submitBtn" class="submit" disabled>Enviar mensagem</button>
          </div>
        </form>
      </section>

      <!-- mapa -->
      <div class="section-title">NOSSA LOCALIZAÇÃO</div>
      <div class="map-wrap" aria-hidden="false">
        <!-- Substitua o src abaixo pelo iframe do Google Maps do seu endereço -->
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3656.123456789!2d-46.633308!3d-23.550520!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94ce59a0e...!2sShopping%20Korai!5e0!3m2!1spt-BR!2sbr!4v0000000000000"
          allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
      </div>

      <div class="big-cta">SEJA UM VENDEDOR</div>

      <footer style="padding:18px 0;text-align:center;color:var(--muted)">© 2025 smartpecas. Todos os direitos reservados</footer>
    </main>
  </div>

  <!-- floating actions -->
  <div class="fab" role="toolbar" aria-label="Ações rápidas">
    <button onclick="navigator.share?.({title:'Smart Peças', text:'Conheça Smart Peças', url:location.href}) || alert('Compartilhar não suportado no seu navegador')">🔗 Compartilhar</button>
    <button onclick="window.scrollTo({top:0,behavior:'smooth'})">⬆️ Topo</button>
  </div>

<script>
  // habilita botão de enviar apenas quando checkbox marcado
  const agree = document.getElementById('agree');
  const submitBtn = document.getElementById('submitBtn');

  agree.addEventListener('change', ()=> {
    if (agree.checked) {
      submitBtn.disabled = false;
      submitBtn.classList.add('enabled');
      submitBtn.style.cursor = 'pointer';
    } else {
      submitBtn.disabled = true;
      submitBtn.classList.remove('enabled');
      submitBtn.style.cursor = 'not-allowed';
    }
  });

  function handleSubmit(e){
    e.preventDefault();
    if (!agree.checked) {
      alert('Por favor, aceite a Política de Privacidade.');
      return;
    }
    // exemplo simples: mostra os dados e limpa form
    const data = new FormData(e.target);
    const obj = Object.fromEntries(data.entries());
    // substituir por fetch() para enviar ao seu endpoint
    alert('Formulário enviado:\n' + JSON.stringify(obj, null, 2));
    e.target.reset();
    agree.checked = false;
    submitBtn.disabled = true;
    submitBtn.classList.remove('enabled');
  }

  function scrollToForm(){
    document.getElementById('pre-cadastro').scrollIntoView({behavior:'smooth'});
  }
</script>
</body>
</html>
