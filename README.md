# JachimowiczMebel1999
<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Stolarstwo Premium</title>
    <style>
        body {
            margin: 0;
            font-family: "Segoe UI", sans-serif;
            background: #ffffff;
            color: #333;
        }

        header {
            position: sticky;
            top: 0;
            background: white;
            padding: 15px 40px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid #ddd;
            z-index: 1000;
        }

        header nav a {
            margin-left: 25px;
            text-decoration: none;
            text-transform: uppercase;
            color: #333;
            font-weight: 600;
            transition: 0.3s;
        }

        header nav a:hover {
            color: #a87946;
        }

        .hero {
            background: url('https://images.unsplash.com/photo-1503387762-592deb58ef4e?auto=format&fit=crop&w=1600&q=60') center/cover;
            height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: flex-start;
            padding: 60px;
            color: white;
            text-shadow: 0 0 10px rgba(0,0,0,0.7);
        }

        .hero h1 {
            font-size: 58px;
            margin: 0 0 10px;
        }

        .hero p {
            font-size: 20px;
            max-width: 500px;
            margin-bottom: 25px;
        }

        .btn {
            display: inline-block;
            padding: 12px 28px;
            background: #a87946;
            color: white;
            text-decoration: none;
            border-radius: 4px;
            transition: 0.3s;
        }
        .btn:hover {
            background: #91683f;
        }

        section {
            padding: 70px 40px;
            max-width: 1200px;
            margin: auto;
        }

        h2 {
            text-align: center;
            font-size: 36px;
            margin-bottom: 50px;
        }

        /* OFERTA */
        .offer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }
        .offer-box {
            background: #fafafa;
            padding: 25px;
            border-radius: 8px;
            border: 1px solid #eee;
            transition: 0.3s;
        }
        .offer-box:hover {
            transform: translateY(-5px);
            border-color: #a87946;
        }

        /* KONFIGURATOR */
        .configurator {
            max-width: 600px;
            margin: auto;
            padding: 30px;
            background: #fafafa;
            border: 1px solid #eee;
            border-radius: 8px;
        }

        label {
            display: block;
            margin: 15px 0 5px;
        }

        select, input {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 6px;
        }

        #calc {
            margin-top: 20px;
            background: #a87946;
            color: white;
            border: none;
            padding: 12px;
            width: 100%;
            cursor: pointer;
            border-radius: 6px;
        }

        #calc:hover {
            background: #91683f;
        }

        #result {
            text-align: center;
            margin-top: 20px;
            font-size: 22px;
        }

        /* KONTAKT */
        .contact-form {
            max-width: 600px;
            margin: auto;
        }

        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 12px;
            margin: 12px 0;
            border-radius: 6px;
            border: 1px solid #ccc;
        }

        .contact-form button {
            padding: 12px 25px;
            background: #a87946;
            color: white;
            border: none;
            border-radius: 6px;
            cursor: pointer;
        }

        footer {
            background: #111;
            color: white;
            text-align: center;
            padding: 25px;
            margin-top: 60px;
        }

        @media(max-width: 700px) {
            .hero h1 { font-size: 38px; }
            .hero p { font-size: 16px; }
        }
    </style>
</head>

<body>

<header>
    <div class="logo"><strong>Stolarstwo Premium</strong></div>
    <nav>
        <a href="#home">Główna</a>
        <a href="#offer">Oferta</a>
        <a href="#configurator">Konfigurator</a>
        <a href="#about">O nas</a>
        <a href="#contact">Kontakt</a>
    </nav>
</header>

<!-- HERO -->
<section class="hero" id="home">
    <h1>Meble na wymiar z pasją</h1>
    <p>Tworzymy wyjątkowe meble, dopasowane do Twojego wnętrza. Precyzja, jakość i ponad 20 lat doświadczenia.</p>
    <a href="#offer" class="btn">Poznaj ofertę</a>
</section>

<!-- OFERTA -->
<section id="offer">
    <h2>Nasza oferta</h2>
    <div class="offer-grid">
        <div class="offer-box">
            <h3>Kuchnie na wymiar</h3>
            <p>Projektujemy i wykonujemy funkcjonalne kuchnie z najwyższej jakości materiałów.</p>
        </div>
        <div class="offer-box">
            <h3>Szafy i garderoby</h3>
            <p>Systemy przesuwne, szafy wnękowe i wolnostojące – perfekcyjnie dopasowane.</p>
        </div>
        <div class="offer-box">
            <h3>Meble biurowe</h3>
            <p>Profesjonalne wykończenia i ergonomiczne rozwiązania dla firm.</p>
        </div>
        <div class="offer-box">
            <h3>Renowacja mebli</h3>
            <p>Przywracamy dawny blask meblom drewnianym każdej epoki.</p>
        </div>
    </div>
</section>

<!-- KONFIGURATOR -->
<section id="configurator">
    <h2>Konfigurator mebli</h2>

    <div class="configurator">
        <label for="type">Rodzaj mebla:</label>
        <select id="type">
            <option value="1000">Szafa</option>
            <option value="1500">Kuchnia</option>
            <option value="800">Biurko</option>
            <option value="600">Stół</option>
        </select>

        <label for="material">Materiał:</label>
        <select id="material">
            <option value="1">Płyta laminowana</option>
            <option value="1.4">Drewno lite</option>
            <option value="1.2">Fornir</option>
        </select>

        <label for="size">Wymiary (m²):</label>
        <input type="number" id="size" placeholder="np. 3" />

        <button id="calc">Oblicz wycenę</button>

        <div id="result"></div>
    </div>
</section>

<!-- O NAS -->
<section id="about">
    <h2>O nas</h2>
    <p style="max-width: 800px; margin: auto; font-size: 18px; line-height: 1.6;">
        Jesteśmy lokalną firmą stolarską z ponad 20-letnim doświadczeniem. 
        Specjalizujemy się w projektowaniu i produkcji mebli na wymiar – od kuchni, przez garderoby, 
        po nietypowe realizacje indywidualne. Każdy projekt traktujemy z pasją i dbałością o szczegóły.
    </p>
</section>

<!-- KONTAKT -->
<section id="contact">
    <h2>Kontakt</h2>
    <div class="contact-form">
        <input type="text" placeholder="Imię i nazwisko">
        <input type="email" placeholder="Adres e-mail">
        <textarea rows="6" placeholder="Twoja wiadomość"></textarea>
        <button>Wyślij</button>
    </div>
</section>

<footer>
    © 2025 Stolarstwo Premium – Wszelkie prawa zastrzeżone
</footer>

<script>
document.getElementById("calc").addEventListener("click", () => {
    const type = parseFloat(document.getElementById("type").value);
    const material = parseFloat(document.getElementById("material").value);
    const size = parseFloat(document.getElementById("size").value);

    if (!size || size <= 0) {
        document.getElementById("result").innerHTML = "Podaj poprawne wymiary.";
        return;
    }

    const price = type * material * size;
    document.getElementById("result").innerHTML = 
        "Szacowana cena: <strong>" + price.toFixed(2) + " zł</strong>";
});
</script>

</body>
</html>
