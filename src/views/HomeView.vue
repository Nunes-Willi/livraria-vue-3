<template>
  <div class="all">
    <div>
      <div class="up">
        <div class="logo-container">
          <img src="@/imagens/Logo.png" alt="Logo" class="logo" />
        </div>
        <div>
          <router-link to="/avaliadores" class="evaluator-button"
            >Página para o Avaliador</router-link
          >
        </div>
      </div>
      <header class="header">
        <img
          src="@/imagens/homes.jpeg"
          alt="Header Image"
          class="header-image"
        />
        <div class="header-text">
          <div class="header-content">
            <h1>Bem-vindo ao HEX</h1>
            <p class="header-subtitle">Melhor site de Hackathons do Brasil</p>
            <router-link to="/participantes" class="botao"
              >Participar de um Hackathon</router-link
            >
          </div>
        </div>
      </header>

      <div class="main-container">
        <div class="flexible-content">
          <h2 class="section-title">O que é o Hackathon?</h2>
          <div class="content-item">
            <div class="content-text">
              <div class="content-wrapper">
                <p>
                  Imagine que você precise resolver um problema da sua empresa,
                  da sua escola, do seu bairro ou de qualquer grupo no qual você
                  pertença, e isso precise ser feito através do uso de alguma
                  tecnologia. E mais, você precisa de uma solução o mais rápido
                  possível… Pode ser que você precise de um Hackathon! Bom, caso
                  você não saiba, Hackathon significa maratona de programação. O
                  termo resulta de uma combinação das palavras inglesas “hack”
                  (programar de forma excepcional) e “marathon” (maratona).
                  Sendo assim, o Hackathon é um evento que reúne programadores,
                  designers e outros profissionais ligados ao desenvolvimento de
                  software para uma maratona de programação, cujo objetivo é
                  desenvolver um software ou solução tecnológica que atenda a um
                  fim específico. A maratona pode durar entre um dia ou uma
                  semana. E ao final, você terá soluções surpreendentes… Nesses
                  eventos, os participantes têm a oportunidade de conhecer
                  outros profissionais da área, fazer Networking, participar de
                  um projeto colaborativo em um ambiente específico de
                  programação e ainda concorrer a prêmios. O que faz um evento
                  como esse ser um sucesso é o desafio. Lembrando que não pode
                  faltar a diversão!
                </p>
                <img
                  src="@/imagens/imgcontent.jpeg"
                  alt="Content Image 1"
                  class="content-image"
                />
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="section-background">
        <h2 style="color: white">Quem pode participar</h2>
        <p style="color: white">
          Nos hackathons tanto podem participar equipes da empresa promotora do
          evento, quanto equipe de fora da empresa. Esta equipes podem ser
          formadas por alunos do ensino médio, quanto de faculdade ou até
          profissionais liberais. A grande ganho, conhecimento e soluções para
          os problemas vêem justamente da união destas pessoas como visões de
          mundos diferentes.
        </p>
        <img
          src="@/imagens/Hreuniao.png"
          alt="Nova Imagem"
          class="nova-imagem"
        />
      </div>

      <div class="bordered-section">
        <h2 class="section-title">Imagens de outras edições</h2>
        <div class="image-group">
          <img src="@/imagens/Group28.png" alt="Imagem 1" class="group-image" />
        </div>
      </div>
    </div>
    <div class="footer">
      <div class="footer_text">©Hackathon Experience ltda.</div>
      <div class="footer_text">CNPJ 73.986.422/0001-51</div>
      <div class="footer_text">+55 (47) 94789-2213</div>
    </div>
  </div>
</template>

<style scoped>
.botao {
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}

.all {
  background: linear-gradient(to bottom right, #1b4341 0%, #1c3132 50%) bottom
      right / 50% 50% no-repeat,
    linear-gradient(to bottom left, #1b4341 0%, #1c3132 50%) bottom left / 50%
      50% no-repeat,
    linear-gradient(to top left, #1b4341 0%, #1c3132 50%) top left / 50% 50%
      no-repeat,
    linear-gradient(to top right, #1b4341 0%, #1c3132 50%) top right / 50% 50%
      no-repeat;
}
/* ... (estilos existentes) ... */

/* Botão para o avaliador */
.evaluator-button {
  position: fixed;
  top: 10px;
  right: 10px;
  background: transparent;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  z-index: 999;
}

/* Adicione a seguinte regra para centralizar as imagens */
.image-group {
  display: flex;
  justify-content: center;
}

.logo-container {
  position: absolute;
  top: 10px;
  left: 10px;
  z-index: 999;
}

.logo {
  width: 187px; /* Ajuste o tamanho da logo conforme necessário */
  height: 58px;
}

.main-container {
  margin: 20px;
  border: 1px solid white;
  padding: 10px;
}

.header {
  position: relative;
  text-align: center;
  color: white;
  height: 400px;
}

.header-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.header-text {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
}

.header-content {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}

.header-subtitle {
  color: white;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  font-size: 20px;
}

.cta-button {
  margin-top: 15px;
  padding: 10px 20px;
  background: transparent;
  color: white;
  border: 2px solid white;
  border-radius: 5px;
  cursor: pointer;
}

.cta-button:hover {
  background: white;
  color: #333;
}

.flexible-content {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 20px;
  padding: 20px;
}

.content-item {
  text-align: center;
}

.content-wrapper {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}

.content-image {
  width: 700px;
  height: 300px;
  margin-left: 100px;
}

.content-text {
  font-size: 18px;
  margin-bottom: 10px;
  color: white;
  text-align: justify;
  padding-right: 190px;
}

.section-background {
  background-color: #224948; /* Cor de fundo diferente */
  padding: 20px; /* Adiciona preenchimento interno */
  border-radius: 5px; /* Adiciona uma borda arredondada */
  margin-top: 20px; /* Adiciona margem superior */
  text-align: center; /* Centraliza o texto */
}

.section-background h2,
.section-background p {
  margin: 0 auto; /* Centraliza os textos horizontalmente */
  color: white; /* Cor do texto */
}

.nova-imagem {
  margin-top: 20px;
  width: 1000px;
  height: 500px;
}

.bordered-section {
  margin-top: 20px;
  padding: 20px;
  border: 2px solid white; /* Borda branca */
}

.section-title {
  color: white; /* Cor do título */
  text-align: center;
}

.group-image {
  width: 1500px;
  height: 1000px;
  margin: 10px;
  object-fit: cover;
}
h2 {
  font-weight: 600;
}
.footer {
  background-color: #224948;
  color: white;
  display: flex;
  flex-direction: row;
  justify-content: center;
  text-align: center;
  height: 70px;
  padding: 70px;
  margin-top: 20px;
}
.footer_text {
  margin-right: 10px;
}
</style>
