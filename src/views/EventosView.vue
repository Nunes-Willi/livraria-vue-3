<template>
  <div>
    <div class="header">
      <div class="logo-container">
        <img src="@/imagens/Logo.png" alt="Logo" class="logo" />
        <p class="participant-center">Central do Participante</p>
      </div>
      <div class="header-buttons">
        <router-link to="/CInscricao" class="header-button"
          >Minhas Inscrições</router-link
        >
        <button class="header-button">Conta</button>
      </div>
    </div>
    <div class="search-container">
      <div class="title_pri"><h1 class="events-title">EVENTOS</h1></div>
      <div class="image_back">
        <input type="text" placeholder="Pesquisar" class="search-input" />
      </div>
    </div>

    <main class="main-container">
      <div class="card card1">
        <div class="card-content">
          <h2 class="event-title">Hackathon IFC - Araquari</h2>
          <p>Data: 24 de Nov</p>
          <p>Horário: 7:30</p>
          <p>Local: IFC Campus Araquari</p>
          <router-link to="/inscricaop" class="subscribe-button"
            >Inscreva-se</router-link
          >
        </div>
      </div>

      <div class="card card2">
        <div class="card-content">
          <h2 class="event-title">Hackathon IFC - Araquari</h2>
          <p>Data</p>
          <p>Horário: 7:30</p>
          <p>Local: IFC Campus Araquari</p>
          <router-link to="/inscricaop" class="subscribe-button"
            >Inscreva-se</router-link
          >
        </div>
      </div>

      <div class="card card3">
        <div class="card-content">
          <h2 class="event-title">Card 3</h2>
          <p>Descrição do card 3.</p>
          <p>Horário: 7:30</p>
          <p>Local: IFC Campus Araquari</p>
          <router-link to="/inscricaop" class="subscribe-button"
            >Inscreva-se</router-link
          >
        </div>
      </div>
    </main>
  </div>
</template>

<script></script>

<style scoped>
.events-title {
  font-size: 24px;
  font-weight: bold;
  color: white;
  text-align: center;
  margin-top: 10px;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
  background-color: #224948;
}

.logo-container {
  display: flex;
  align-items: center;
}

.participant-center {
  margin-left: 10px;
  color: white;
}

.header-buttons {
  display: flex;
}

.header-button {
  margin-left: 10px;
  padding: 8px 16px;
  background-color: transparent;
  color: white;
  border: 1px solid white;
  border-radius: 4px;
  cursor: pointer;
}

.card-content {
  position: relative;
}

.event-title {
  text-decoration: underline;
}

.subscribe-button {
  position: absolute;
  bottom: 10px;
  right: 10px;
  padding: 8px 16px;
  background-color: transparent;
  color: white;
  border: 1px solid white;
  border-radius: 4px;
  cursor: pointer;
}

.search-container {
  position: relative;
  width: 100%;
  height: 200px;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  background-image: url("@/imagens/evento.png");
  display: flex;
  flex-direction: column;
}

.search-input {
  z-index: 2;
  padding: 8px;
  border: none;
  border-radius: 15px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 800px;
  margin-top: 10px;
}

.background-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.main-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px;
  background-color: #224849;
  position: relative;
  z-index: 1;
}

.card {
  width: 800px;
  padding: 20px;
  margin: 20px;
  border: 1px solid #333;
  border-radius: 8px;
  color: white;
  background-size: cover;
  background-position: center;
  position: relative;
}

.card::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.5); /* Cor do filtro preto */
  border-radius: 8px; /* Garante que o filtro preto tenha as mesmas bordas arredondadas que o card */
}

.card1 {
  background-image: url("@/imagens/ifc2.png"); /* Substitua pelo caminho da sua imagem */
}

.card2 {
  background-image: url("@/imagens/ifc2.png"); /* Substitua pelo caminho da sua imagem */
}

.card3 {
  background-image: url("@/imagens/ifc2.png"); /* Substitua pelo caminho da sua imagem */
}

.card h2 {
  font-size: 18px;
  margin-bottom: 10px;
}

.card p {
  font-size: 14px;
}
</style>
