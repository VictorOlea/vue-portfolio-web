<template>
  <BentoGrid>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 2 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
      ><a
        href="https://vue-sismos.netlify.app/"
        target="_blank"
        rel="noopener noreferrer"
        :class="projectStyle['project-link']"
      >
        <section :class="projectStyle['project-card']">
          <h2 :class="projectStyle['project-title']">Sismos App</h2>
          <div :class="projectStyle['project-icon']">
            <img
              src="../assets/earthquake.svg"
              alt="Earthquake Icon"
              width="36"
              height="36"
            />
          </div>
          <p :class="projectStyle['project-content']">
            Web app para visualizar los últimos sismos registrados en Chile.
          </p>
        </section>
      </a>
    </BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 2 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
      ><a
        href="https://react-dashboard-mockup.netlify.app/"
        target="_blank"
        rel="noopener noreferrer"
        :class="projectStyle['project-link']"
      >
        <section :class="projectStyle['project-card']">
          <h2 :class="projectStyle['project-title']">Dashboard</h2>
          <div :class="projectStyle['project-icon']">
            <img
              src="../assets/dashboard.svg"
              alt="Dashboard Icon"
              width="36"
              height="36"
            />
          </div>
          <p :class="projectStyle['project-content']">
            Informe interactivo para análisis de datos.
          </p>
        </section>
      </a>
    </BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 2 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
      ><a
        href="https://geo-dashboard-react.netlify.app/"
        target="_blank"
        rel="noopener noreferrer"
        :class="projectStyle['project-link']"
      >
        <section :class="projectStyle['project-card']">
          <h2 :class="projectStyle['project-title']">Geo Dashboard</h2>
          <div :class="projectStyle['project-icon']">
            <img
              src="../assets/geo.svg"
              alt="Geo Icon"
              width="36"
              height="36"
            />
          </div>
          <p :class="projectStyle['project-content']">
            Dashboard interactivo con datos georreferenciados.
          </p>
        </section>
      </a>
    </BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 2 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
      ><a
        href="https://vue-crypto-tracker-app.netlify.app/"
        target="_blank"
        rel="noopener noreferrer"
        :class="projectStyle['project-link']"
      >
        <section :class="projectStyle['project-card']">
          <h2 :class="projectStyle['project-title']">Crypto Tracker</h2>
          <div :class="projectStyle['project-icon']">
            <img
              src="../assets/bitcoin.svg"
              alt="Bitcoin Icon"
              width="36"
              height="36"
            />
          </div>
          <p :class="projectStyle['project-content']">
            Web app para el seguimiento de criptomonedas en tiempo real.
          </p>
        </section>
      </a></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 2 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
      ><a
        href="https://bento-vue-app.netlify.app/"
        target="_blank"
        rel="noopener noreferrer"
        :class="projectStyle['project-link']"
      >
        <section :class="projectStyle['project-card']">
          <h2 :class="projectStyle['project-title']">Bento Design</h2>
          <div :class="projectStyle['project-icon']">
            <img
              src="../assets/bento-box.svg"
              alt="Bento Icon"
              width="36"
              height="36"
            />
          </div>
          <p :class="projectStyle['project-content']">
            Diseño web moderno inspirado en Bento Grid.
          </p>
        </section>
      </a>
    </BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 2 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
      ><a
        href="https://github.com/VictorOlea/Placa-Control-Helice"
        target="_blank"
        rel="noopener noreferrer"
        :class="projectStyle['project-link']"
      >
        <section :class="projectStyle['project-card']">
          <h2 :class="projectStyle['project-title']">PCB Design</h2>
          <div :class="projectStyle['project-icon']">
            <img
              src="../assets/electronics.svg"
              alt="Electronic Icon"
              width="36"
              height="36"
            />
          </div>
          <p :class="projectStyle['project-content']">
            Desarrollo de PCBs personalizados y electrónica al detalle.
          </p>
        </section>
      </a></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 2 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
      ><a
        href="https://mini-robot-esp32.netlify.app/"
        target="_blank"
        rel="noopener noreferrer"
        :class="projectStyle['project-link']"
      >
        <section :class="projectStyle['project-card']">
          <h2 :class="projectStyle['project-title']">Robotica Educativa</h2>
          <div :class="projectStyle['project-icon']">
            <img
              src="../assets/robot.svg"
              alt="Robot Icon"
              width="36"
              height="36"
            />
          </div>
          <p :class="projectStyle['project-content']">
            Robots modulares con electrónica integrada.
          </p>
        </section> </a
      >></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 2 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
      ><a
        href="#"
        target="_blank"
        rel="noopener noreferrer"
        :class="projectStyle['project-link']"
      >
        <section :class="projectStyle['project-card']">
          <h2 :class="projectStyle['project-title']">Portfolio</h2>
          <div :class="projectStyle['project-icon']">
            <img
              src="../assets/portfolio.svg"
              alt="Vue Icon"
              width="36"
              height="36"
            />
          </div>
          <p :class="projectStyle['project-content']">
            Portafolio: perfil, servicios y proyectos destacados.
          </p>
        </section>
      </a></BentoCard
    >
  </BentoGrid>
</template>

<script setup lang="ts">
import BentoGrid from "../components/BentoGrid.vue";
import BentoCard from "../components/BentoCard.vue";
import projectStyle from "../styles/project.module.css";
</script>
