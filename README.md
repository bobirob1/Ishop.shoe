# Ishop.shoe
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Magazin de Haine</title>
    <link rel="stylesheet" href="styles.css">
    <script defer src="script.js"></script>
</head>
<body>
    <header>
        <nav>
            <h1>Magazinul Meu de Haine</h1>
            <ul>
                <li><a href="#produse">Produse</a></li>
                <li><a href="#despre">Despre Noi</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><a href="#cos">Coș de Cumpărături</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="produse">
            <h2>Produsele Noastre</h2>
            <div class="produse-container">
                <div class="produs" data-nume="Rochie Eleganta" data-pret="150">
                    <img src="imagine1.jpg" alt="Produs 1">
                    <h3>Rochie Eleganta</h3>
                    <p>Pret: 150 RON</p>
                    <button class="adauga-cos">Adaugă în Coș</button>
                </div>
                <div class="produs" data-nume="Blugi Moderni" data-pret="200">
                    <img src="imagine2.jpg" alt="Produs 2">
                    <h3>Blugi Moderni</h3>
                    <p>Pret: 200 RON</p>
                    <button class="adauga-cos">Adaugă în Coș</button>
                </div>
                <div class="produs" data-nume="Tricou Casual" data-pret="75">
                    <img src="imagine3.jpg" alt="Produs 3">
                    <h3>Tricou Casual</h3>
                    <p>Pret: 75 RON</p>
                    <button class="adauga-cos">Adaugă în Coș</button>
                </div>
            </div>
        </section>

        <section id="despre">
            <h2>Despre Noi</h2>
            <p>Suntem un magazin de haine dedicat stilului si calitatii. Oferim o gama variata de produse pentru toate gusturile si ocaziile.</p>
        </section>

        <section id="contact">
            <h2>Contact</h2>
            <form action="submit_form.php" method="post">
                <label for="nume">Nume:</label>
                <input type="text" id="nume" name="nume" required>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>

                <label for="mesaj">Mesaj:</label>
                <textarea id="mesaj" name="mesaj" required></textarea>

                <button type="submit">Trimite</button>
            </form>
        </section>

        <section id="cos">
            <h2>Coș de Cumpărături</h2>
            <div class="cos-container">
                <table>
                    <thead>
                        <tr>
                            <th>Produs</th>
                            <th>Preț</th>
                            <th>Cantitate</th>
                            <th>Total</th>
                            <th>Acțiune</th>
                        </tr>
                    </thead>
                    <tbody id="cos-produse">
                        <!-- Produsele adăugate în coș vor apărea aici -->
                    </tbody>
                </table>
                <div class="total">
                    <h3>Total de plată: <span id="total-pret">0</span> RON</h3>
                </div>
                <button id="finalizeaza-comanda">Finalizează Comanda</button>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Magazinul Meu de Haine. Toate drepturile rezervate.</p>
    </footer>
</body>
</html>
