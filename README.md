# Rizal

<html lang="en">

  <h1>Dr. Jose Rizal</h1>
  <img src="rizal_portrait.jpg" alt="Jose Rizal Portrait">

  <nav>
    <a href="#early-life">Early Life</a> |
    <a href="#education">Education</a> |
    <a href="#works">Famous Works</a> |
    <a href="#legacy">Legacy</a>
  </nav>

  <!-- 🔍 Search bar -->
  <div id="search-container">
    <input type="text" id="search-input" placeholder="Search something about Jose Rizal..." oninput="searchText()">
  </div>

  <!-- 📚 Content -->
  <section id="early-life">
    <h2>Early Life</h2>
    <p>Jose Rizal was born on June 19, 1861, in Calamba, Laguna, Philippines. He was the seventh child in a well-off family. From an early age, he showed remarkable intelligence and a deep love for learning.</p>
    <img src="calamba_church.jpg" alt="Calamba Church">
  </section>

  <section id="education">
    <h2>Education</h2>
    <p>Rizal studied at the Ateneo Municipal and later at the University of Santo Tomas before pursuing further studies in Europe. He earned degrees in medicine and philosophy from prestigious institutions in Madrid, Paris, and Heidelberg.</p>
    <img src="ust_seal.svg" alt="UST Seal">
  </section>

  <section id="works">
    <h2>Famous Works</h2>
    <p>He wrote "Noli Me Tangere" and "El Filibusterismo," two novels that exposed the injustices of Spanish rule in the Philippines and inspired a movement toward independence.</p>
    <img src="noli_me_tangere.jpg" alt="Noli Me Tangere Cover">
  </section>

  <section id="legacy">
    <h2>Legacy</h2>
    <p>Jose Rizal's execution on December 30, 1896, solidified his status as a martyr and national hero. His legacy continues to inspire Filipinos to this day.</p>
    <img src="rizal_monument.jpg" alt="Rizal Monument">
  </section>

  <footer>
    <p>Website created for educational purposes. &copy; 2025</p>
  </footer>

  <!-- 🔍 JavaScript for search -->
  <script>
    function searchText() {
      const input = document.getElementById("search-input").value.toLowerCase();
      const sections = document.querySelectorAll("section p, section h2");

      sections.forEach(el => {
        el.innerHTML = el.textContent;
        if (input) {
          const regex = new RegExp((${input}), "gi");
          el.innerHTML = el.textContent.replace(regex, <span class="highlight">$1</span>);
        }
      });
    }
  </script>

</body>
</html>
