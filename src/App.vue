<script setup>
import { ref } from "vue";

const isDark = ref(false);
</script>

<template>
  <div class="portfolio" :class="{ 'dark-mode': isDark }">
    <nav class="navbar">
      <h2>Brickz Aloysius R. Mucati</h2>

      <div class="nav-links">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#interests">Interests</a>
        <a href="#hobbies">Hobbies</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
      </div>
      <button
        class="theme-toggle"
        :class="{ active: isDark }"
        @click="isDark = !isDark"
        aria-label="Toggle dark mode"
      >
        <span class="toggle-icon">
          {{ isDark ? "⏾" : "☀︎" }}
        </span>
      </button>
    </nav>

    <main class="hero" id="home">
      <img
        src="/PROFILE.jpg"
        alt="My profile picture"
        class="profile-picture"
      />
      <h1>Hi, I'm Brickz!</h1>
      <p>BSIT STUDENT | PC BUILDING ENTHUSIAST</p>
      <h2>Exploring the world of PC building.</h2>
      <p>
        I'm an IT student interested in computer hardware, PC components, and
        learning how computers work.
      </p>
      <a class="button" href="#about"> Get to know me </a>
    </main>
    <section id="about" class="about-section">
      <h2>About Me</h2>

      <p>
        I'm a Bachelor of Science in Information Technology student with a
        strong interest in computer hardware, especially PC building.
      </p>

      <p>
        I want to learn more about computer components, how they work together,
        and how to choose parts for different needs and budgets.
      </p>
    </section>

    <section id="interests" class="interests-section">
      <h2>My Interests</h2>

      <div class="interest-cards">
        <div class="interest-card">
          <h3>PC Components</h3>
          <p>
            Learning about computer parts and understanding how each component
            works.
          </p>
        </div>

        <div class="interest-card">
          <h3>PC Building</h3>
          <p>
            Exploring how to assemble computers and choose the right parts for
            different needs.
          </p>
        </div>

        <div class="interest-card">
          <h3>Gaming</h3>
          <p>
            Playing games and enjoying different gaming experiences in my free
            time.
          </p>
        </div>
      </div>
    </section>
    <section id="skills" class="skills-section">
      <h2>My Skills</h2>

      <div class="skills-cards">
        <div class="skill-card">
          <h3>HTML</h3>
        </div>

        <div class="skill-card">
          <h3>CSS</h3>
        </div>

        <div class="skill-card">
          <h3>MySQL</h3>
        </div>

        <div class="skill-card">
          <h3>C++</h3>
        </div>

        <div class="skill-card">
          <h3>Java</h3>
        </div>

        <div class="skill-card">
          <h3>C#</h3>
        </div>
      </div>
    </section>
    <section id="hobbies" class="hobbies-section">
      <h2>My Hobbies</h2>

      <h3>Gaming</h3>
      <div class="hobby-cards">
        <div class="hobby-card">
          <img src="/Valorant.jpeg" alt="Valorant" />
          <h4>Valorant</h4>
        </div>

        <div class="hobby-card">
          <img src="/Tekken7.jpeg" alt="Tekken 7" />
          <h4>Tekken 7</h4>
        </div>

        <div class="hobby-card">
          <img src="/Roblox.png" alt="Roblox" />
          <h4>Roblox</h4>
        </div>

        <div class="hobby-card">
          <img src="/MobileLegends.png" alt="Mobile Legends" />
          <h4>Mobile Legends</h4>
        </div>
      </div>

      <h3>Manga</h3>
      <div class="hobby-cards">
        <div class="hobby-card">
          <img src="/Nisekoi.jpg" alt="Nisekoi" />
          <h4>Nisekoi</h4>
        </div>

        <div class="hobby-card">
          <img src="/MidnightHeart.jpeg" alt="Tune In to the Midnight Heart" />
          <h4>Tune In to the Midnight Heart</h4>
        </div>
      </div>

      <h3>Manhwa</h3>
      <div class="hobby-cards">
        <div class="hobby-card">
          <img src="/Resign.jpg" alt="Ctrl Alt Resign" />
          <h4>Ctrl+Alt+Resign</h4>
        </div>

        <div class="hobby-card">
          <img src="/MiaReturned.jpg" alt="Mia Has Returned" />
          <h4>Mia Has Returned</h4>
        </div>
      </div>

      <h3>Movies</h3>
      <div class="hobby-cards">
        <div class="hobby-card">
          <img src="/HTTYD.png" alt="How to Train Your Dragon" />
          <h4>How to Train Your Dragon</h4>
        </div>

        <div class="hobby-card">
          <img src="/LordOfTheRings.png" alt="Lord of the Rings" />
          <h4>Lord of the Rings</h4>
        </div>

        <div class="hobby-card">
          <img src="/PlanetOfTheApes.png" alt="Planet of the Apes" />
          <h4>Planet of the Apes</h4>
        </div>

        <div class="hobby-card">
          <img src="/TheMazeRunner.png" alt="The Maze Runner" />
          <h4>The Maze Runner</h4>
        </div>
      </div>
    </section>

    <section id="contact" class="contact-section">
      <h2>Contact Me</h2>
      <p>You can find me on these platforms.</p>

      <div class="contact-links">
        <a href="https://www.facebook.com/brickz.mucati" target="_blank" rel="noopener noreferrer">
          <img src="/Facebook.jpeg" alt="Facebook" />
          <span>Facebook</span>
        </a>

        <a href="https://www.instagram.com/rickz.lys/?hl=en" target="_blank" rel="noopener noreferrer">
          <img src="/Instagram.jpeg" alt="Instagram" />
          <span>Instagram</span>
        </a>

        <a href="https://discord.com/users/1365229398357446657" target="_blank" rel="noopener noreferrer">
          <img src="/Discord.jpg" alt="Discord" />
          <span>Discord</span>
        </a>
      </div>
    </section>

    <footer class="footer">
      <p>Brickz Aloysius R. Mucati | My First Portfolio Project</p>
    </footer>
  </div>
</template>
