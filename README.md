# zielona-architektura
<!DOCTYPE html>
<html lang="pl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Zielony Krajobraz</title>
  <style>
    body { margin:0; font-family:sans-serif; background:#fff; color:#064E3B; }
    header, footer { background:#D1FAE5; padding:1rem; text-align:center; }
    header nav a { margin:0 1rem; color:#064E3B; text-decoration:none; }
    section { padding:2rem; }
    .services, .gallery { display:grid; gap:1rem; }
    .services { grid-template-columns:repeat(auto-fit, minmax(250px,1fr)); }
    .service-card { border:1px solid #A7F3D0; background:#ECFDF5; padding:1rem; border-radius:8px; }
    .gallery { grid-template-columns:repeat(auto-fit, minmax(200px,1fr)); }
    .gallery img { width:100%; border-radius:8px; height:auto; object-fit:cover; }
    form { max-width:500px; margin:0 auto; display:grid; gap:1rem; }
    input, textarea { padding:0.8rem; border:1px solid #A7F3D0; border-radius:4px; }
    button { padding:0.8rem; border:none; border-radius:4px; background:#047857; color:#fff; cursor:pointer; }
    button:hover { background:#065F46; }
    .contact-info { text-align:center; margin-top:1rem; }
    .contact-info p { margin:0.2rem 0; display:flex; justify-content:center; align-items:center; gap:0.5rem; }
  </style>
</head>
<body>
  <header>
    <h1>Zielony Krajobraz</h1>
    <nav>
      <a href="#home">Strona Główna</a>
      <a href="#services">Oferta</a>
      <a href="#gallery">Galeria</a>
      <a href="#contact">Kontakt</a>
    </nav>
  </header>
  <section id="home"><h2>Nasze Usługi</h2><p>Projektujemy, zakładamy i pielęgnujemy ogrody, przestrzenie zielone oraz ogrody naturalistyczne z pasją i dbałością o każdy szczegół.</p></section>
  <section id="services"><div class="services">
    <div class="service-card"><h3>Specjalistyczne roboty budowlane</h3><p>Pozostałe specjalistyczne roboty budowlane, gdzie indziej niesklasyfikowane.</p></div>
    <div class="service-card"><h3>Systemy nawadniania</h3><p>Montaż systemów nawadniania ogrodów.</p></div>
    <div class="service-card"><h3>Architektura krajobrazu</h3><p>Działalność w zakresie architektury i projektowania zieleni.</p></div>
    <div class="service-card"><h3>Projekty koncepcyjne</h3><p>Wizualizacje 2D/3D ogrodów, parków i przestrzeni zielonych.</p></div>
    <div class="service-card"><h3>Fotografia ogrodów</h3><p>Zdjęcia realizacji ogrodów dla portfolio i klientów.</p></div>
    <div class="service-card"><h3>Zagospodarowanie terenów</h3><p>Zakładanie ogrodów, trawników, parków.</p></div>
    <div class="service-card"><h3>Pielęgnacja zieleni</h3><p>Koszenie trawy, podlewanie, nawożenie, przycinanie drzew i krzewów.</p></div>
    <div class="service-card"><h3>Budowa elementów ogrodowych</h3><p>Oczka wodne, ścieżki, tarasy, altany i inne.</p></div>
    <div class="service-card"><h3>Utrzymanie czystości</h3><p>Usuwanie chwastów, liści i śniegu z terenów zielonych.</p></div>
  </div></section>
  <section id="gallery"><h2>Galeria Projektów</h2><div class="gallery">
    <img src="https://source.unsplash.com/600x400/?garden,landscape,1" alt="Projekt 1">
    <img src="https://source.unsplash.com/600x400/?garden,landscape,2" alt="Projekt 2">
    <img src="https://source.unsplash.com/600x400/?garden,landscape,3" alt="Projekt 3">
    <img src="https://source.unsplash.com/600x400/?garden,landscape,4" alt="Projekt 4">
    <img src="https://source.unsplash.com/600x400/?garden,landscape,5" alt="Projekt 5">
    <img src="https://source.unsplash.com/600x400/?garden,landscape,6" alt="Projekt 6">
  </div></section>
  <section id="contact"><h2>Kontakt</h2>
    <form onsubmit="event.preventDefault(); alert('Dziękujemy! Wiadomość wysłana.');">
      <input type="text" placeholder="Imię i nazwisko" required>
      <input type="email" placeholder="Adres e-mail" required>
      <textarea placeholder="Wiadomość" required></textarea>
      <button type="submit">Wyślij wiadomość</button>
    </form>
    <div class="contact-info">
      <p>✉️ dominikadomyslawska67@gmail.com</p>
      <p>📞 +48 600 123 456</p>
    </div>
  </section>
  <footer><p>© 2025 Zielony Krajobraz. Wszelkie prawa zastrzeżone.</p></footer>
  <script>
    document.querySelectorAll('nav a').forEach(a => {
      a.addEventListener('click', e => {
        e.preventDefault();
        document.querySelector(a.hash).scrollIntoView({ behavior: 'smooth' });
      });
    });
  </script>
</body>
</html>
