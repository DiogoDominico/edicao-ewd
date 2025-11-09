<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>EWD Investimentos</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f5f5f5;
      color: #333;
    }
    header {
      background-color: #002e5b;
      color: white;
      padding: 1rem 2rem;
      display: flex;
      align-items: center;
      gap: 1rem;
    }
    header img {
      height: 60px;
      width: auto;
    }
    header h1 {
      margin: 0;
      font-size: 1.8rem;
    }
    header p {
      margin: 0;
      font-size: 1rem;
      color: #cdd7e0;
    }
    section {
      padding: 2rem;
      max-width: 1000px;
      margin: auto;
    }
    .destaque {
      font-size: 1.5rem;
      margin: 1rem 0;
      color: #002e5b;
    }
    .numeros,
    .parceiros,
    .faq,
    .depoimentos,
    .formulario {
      background: white;
      margin: 2rem 0;
      padding: 2rem;
      border-radius: 12px;
      box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
    }
    .numeros ul,
    .parceiros ul {
      list-style: none;
      padding: 0;
    }
    .numeros li,
    .parceiros li {
      margin: 0.5rem 0;
    }
    .cta {
      text-align: center;
      margin: 3rem 0;
    }
    .cta button {
      background-color: #007bff;
      color: white;
      padding: 1rem 2rem;
      font-size: 1rem;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }
    .cta button:hover {
      background-color: #0056b3;
    }
    .formulario form {
      display: flex;
      flex-direction: column;
      gap: 1rem;
      max-width: 600px;
      margin: auto;
    }
    .formulario input,
    .formulario textarea {
      padding: 1rem;
      border: 1px solid #ccc;
      border-radius: 8px;
      font-size: 1rem;
      transition: border-color 0.3s ease, box-shadow 0.3s ease;
    }
    .formulario input:focus,
    .formulario textarea:focus {
      border-color: #007bff;
      box-shadow: 0 0 0 3px rgba(0, 123, 255, 0.2);
      outline: none;
    }
    .formulario button {
      background-color: #28a745;
      color: white;
      padding: 1rem;
      font-size: 1rem;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }
    .formulario button:hover {
      background-color: #218838;
    }
    footer {
      background-color: #002e5b;
      color: white;
      text-align: center;
      padding: 1rem;
    }
  </style>
</head>
<body>
  <header>
    <img src="Screenshot_20251108_164219_WhatsApp.jpg" alt="Logo EWD Investimentos" />
    <div>
      <h1>EWD Investimentos</h1>
      <p>Consultoria de Investimentos e Gestão de Patrimônio Personalizada</p>
    </div>
  </header>

  <section>
    <p class="destaque">
      O modelo de gestão de patrimônio mais bem-sucedido no mundo, agora disponível para você.
    </p>
    <p>
      Na <strong>EWD Investimentos</strong>, oferecemos uma abordagem personalizada para atender aos seus objetivos financeiros, com transparência e alinhamento total aos seus interesses.
    </p>
  </section>

  <section class="parceiros">
    <h2>Parceiros</h2>
    <ul>
      <li>BTG Pactual</li>
      <li>XP Investimentos</li>
      <li>Warren</li>
      <li>Avenue</li>
      <li>Interactive Brokers</li>
    </ul>
  </section>

  <section class="faq">
    <h2>Perguntas Frequentes</h2>
    <p>
      <strong>Qual o valor mínimo para ser cliente?</strong><br />
      Atendemos clientes com investimentos a partir de R$ 100.000,00.
    </p>
    <p>
      <strong>Como é feita a cobrança?</strong><br />
      Cobramos uma taxa mensal baseada no valor atual da sua carteira, alinhando nossos interesses aos seus.
    </p>
    <p>
      <strong>Preciso sair da minha assessoria atual?</strong><br />
      Sim, para garantir um atendimento exclusivo e alinhado, é necessário migrar para a EWD Investimentos.
    </p>
  </section>

  <section class="formulario">
    <h2>Agende sua Consultoria</h2>
    <p>Preencha o formulário abaixo e entraremos em contato para agendar uma reunião personalizada.</p>
    <form action="https://formspree.io/f/xgvkgdzw" method="POST">
      <input type="text" name="nome" placeholder="Seu nome completo" required />
      <input type="email" name="email" placeholder="Seu e-mail" required />
      <input type="tel" name="telefone" placeholder="Seu telefone" required />
      <textarea name="mensagem" rows="4" placeholder="Mensagem ou dúvida (opcional)"></textarea>
      <button type="submit">Enviar</button>
    </form>
  </section>

  <section class="cta">
    <h2>Pronto para transformar a gestão do seu patrimônio?</h2>
    <p>Agende uma consultoria gratuita com nossos especialistas.</p>
    <button onclick="document.querySelector('.formulario').scrollIntoView({ behavior: 'smooth' });">
      Agendar Consultoria
    </button>
  </section>

  <footer>
    <p>&copy; 2025 EWD Investimentos. Todos os direitos reservados.</p>
    <p>Política de Privacidade | Termos de Uso | Contato: ewdparticipacoes@hotmail.com</p>
  </footer>
</body>
</html>
