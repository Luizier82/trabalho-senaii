<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Site Profissional com PDF</title>
  <style>
    /* Reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    /* Corpo e fundo em tom de cinza claro */
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #e5e5e5;
      color: #222;
      line-height: 1.6;
      padding: 40px;
      min-height: 100vh;
    }

    .container {
      max-width: 1400px;
      margin: 0 auto;
      padding: 60px 100px;
      background-color: #f8f8f8;
      border-radius: 20px;
      box-shadow: 12px 12px 35px #cfcfcf, -12px -12px 35px #ffffff;
    }

    /* Logo ajustado para ocupar mesmo tamanho da lateral */
    .logo {
      display: block;
      width: 100%;
      max-width: 550px; /* largura máxima igual à altura da lateral */
      height: 440px;    /* mesma altura do bloco lateral */
      object-fit: contain;
      margin: 0 auto 60px;
      filter: drop-shadow(0 0 4px rgba(0,0,0,0.15));
      transition: transform 0.3s ease, filter 0.3s ease;
    }

    .logo:hover {
      transform: scale(1.05);
      filter: drop-shadow(0 0 10px rgba(0,0,0,0.3));
    }

    .imagem-texto {
      display: flex;
      flex-wrap: wrap;
      gap: 50px;
      margin-bottom: 80px;
    }

    .imagem-texto img {
      flex: 1 1 50%;
      max-width: 100%;
      height: 440px;
      object-fit: cover;
      border-radius: 16px;
      box-shadow: 8px 8px 25px #d0d0d0, -8px -8px 25px #ffffff;
      transition: transform 0.3s ease;
    }

    .imagem-texto img:hover {
      transform: scale(1.04);
      cursor: pointer;
    }

    .texto-lateral {
      flex: 1 1 50%;
      background-color: #ffffff;
      padding: 40px;
      font-size: 19px;
      border-radius: 16px;
      box-shadow: inset 3px 3px 10px #dcdcdc, inset -3px -3px 10px #ffffff;
      color: #333;
      line-height: 1.8;
      height: 440px;
      overflow-y: auto;
    }

    .diarios {
      margin-top: 60px;
      text-align: center;
      max-width: 1100px;
      margin-left: auto;
      margin-right: auto;
    }

    .diarios h2 {
      font-size: 36px;
      margin-bottom: 30px;
      color: #555;
      text-shadow: 1px 1px 2px #ccc;
      font-weight: 700;
    }

    .texto-diario {
      background-color: #ffffff;
      padding: 40px;
      font-size: 18px;
      border-radius: 16px;
      box-shadow: inset 3px 3px 12px #d1d1d1, inset -3px -3px 12px #ffffff;
      color: #222;
      line-height: 1.8;
      height: 440px;
      overflow-y: auto;
      text-align: left;
      white-space: pre-wrap;
    }

    .btn-pdf {
      margin-top: 40px;
      background-color: #f0f0f0;
      border: none;
      padding: 18px 50px;
      border-radius: 35px;
      color: #333;
      font-weight: 700;
      font-size: 20px;
      cursor: pointer;
      box-shadow: 6px 6px 14px #d1d1d1, -6px -6px 14px #ffffff;
      transition: transform 0.2s ease, box-shadow 0.3s ease;
      user-select: none;
      text-decoration: none;
      display: inline-block;
    }

    .btn-pdf:hover {
      transform: scale(1.05);
      box-shadow: 4px 4px 12px #c4c4c4, -4px -4px 12px #ffffff;
    }

    .btn-pdf:active {
      transform: scale(0.98);
    }

    .whatsapp-btn {
      position: fixed;
      bottom: 25px;
      left: 25px;
      background-color: #f0f0f0;
      color: #333;
      padding: 14px 26px;
      border-radius: 35px;
      font-weight: 700;
      font-size: 16px;
      text-decoration: none;
      box-shadow: 6px 6px 14px #d1d1d1, -6px -6px 14px #ffffff;
      border: none;
      transition: transform 0.2s ease, box-shadow 0.3s ease;
      user-select: none;
      z-index: 1000;
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .whatsapp-btn:hover {
      transform: scale(1.05);
      box-shadow: 4px 4px 12px #c4c4c4, -4px -4px 12px #ffffff;
    }

    @media (max-width: 768px) {
      body {
        padding: 20px;
      }

      .container {
        padding: 30px 20px;
      }

      .imagem-texto {
        flex-direction: column;
        gap: 30px;
      }

      .imagem-texto img,
      .texto-lateral {
        flex: 1 1 100%;
        height: auto;
      }

      .diarios .texto-diario {
        height: auto;
      }

      .logo {
        max-width: 100%;
        height: auto;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- Logo -->
    <img src="blob:https://web.whatsapp.com/cb4905d1-bbb9-4013-ac47-16ea50a80ab7" alt="Logo do Site" class="logo" />

    <!-- Imagem e texto lado a lado -->
    <div class="imagem-texto">
      <img src="OIP.webp" alt="Imagem de exemplo" />
      <div class="texto-lateral">
        <p>
          Você sabia que de acordo com uma pesquisa de 2019 do CFA (conselho federal de
administração) conflitos entre os colaboradores de diferentes gerações, são responsáveis
por 12% da perda de proatividade no ambiente de trabalho?
        </p>
      </div>
    </div>

    <!-- Seção Diários -->
    <div class="diarios">
      <h2>Diários</h2>
      <div class="texto-diario">
        <p>
1 - Diário que poderá ser utilizado em diversos cenários, conflitos, conversas difíceis e situações em que o funcionário não sabe qual caminho tomar. Esse diário de autoajuda direciona o funcionário para uma direção mais saudável mentalmente e socialmente, tanto na vida profissional quanto pessoal.

2- Diário que direciona o funcionário a refletir sobre ações, ajudando a evitar conflitos.

3 - Perguntas de auto análise, sobre situações de conflitos ou dúvidas relacionadas aos seus colegas ou ao seu próprio ambiente de trabalho.

4 - Criar um relatório do dia e classificar as situações que podem ter gerado conflitos em graus de preocupação ou importância.

5 - Espaço reservado ao final do relatório para a resolução de problemas e explicação de como foi solucionado.
m que o usuário edite nada.
        </p>
      </div>

      <a href="https://docs.google.com/forms/d/e/1FAIpQLSco6YIUZNZDI3ZjUJMvN0j-oDHynN-tNnXJTQbXwHTLizqRUA/viewform" target="_blank" class="btn-pdf" role="button" aria-label="Entrar no PDF">
        Entrar no formulario
      </a>
    </div>
  </div>

  <!-- Botão WhatsApp fixo -->
  <a href="https://wa.me/5511999999999" target="_blank" class="whatsapp-btn" aria-label="Contato via WhatsApp">
    Entre em contato conosco
  </a>
</body>
</html>
