<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Endangered Species Guide</title>
    <link rel="stylesheet" href="styles.css">
    <!-- Add Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&family=Merriweather:wght@700&display=swap" rel="stylesheet">
    <style>
        body {
            background-color: #121212;
            color: #ffffff;
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        header {
            background-color: #1e1e1e;
            padding: 20px;
        }
        h1 {
            margin: 0;
            font-size: 2.5em;
            font-family: 'Merriweather', serif;
        }
        p {
            font-size: 1.2em;
            color: #bbbbbb;
        }
        main {
            padding: 20px;
        }
        section {
            background-color: #222;
            padding: 20px;
            border-radius: 10px;
            margin: 20px auto;
            max-width: 800px;
            text-align: left;
        }
        ul {
            list-style-type: none;
            padding: 0;
        }
        li {
            background-color: #333;
            margin: 10px 0;
            padding: 10px;
            border-radius: 5px;
            cursor: pointer;
        }
        img {
            max-width: 100%;
            border-radius: 10px;
            margin-top: 10px;
        }
        footer {
            background-color: #1e1e1e;
            padding: 10px;
            margin-top: 20px;
        }

        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0, 0, 0, 0.8);
            padding-top: 60px;
        }
        .modal-content {
            background-color: #333;
            color: #fff;
            margin: 5% auto;
            padding: 20px;
            border-radius: 10px;
            max-width: 800px;
            text-align: left;
        }
        .close {
            color: #bbb;
            float: right;
            font-size: 28px;
            font-weight: bold;
        }
        .close:hover,
        .close:focus {
            color: #fff;
            text-decoration: none;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <header>
        <h1>Guidoor</h1>
        <p>"Protecting Nature, Preserving Life."</p>
        <img src="https://turbologo.com/designs/76926677" alt="Website Logo">
           </header>
    
    <main>
        <section id="species">
            <h2>Endangered Species</h2>
            <p>Explore some of the world's most endangered animals and learn how we can protect them.</p>
            <ul>
                <li onclick="openModal('tiger')">
                    <strong>Tiger</strong> - Threatened by habitat loss and poaching.
                    <img src="https://iso.500px.com/wp-content/uploads/2015/08/tigers_cover.jpeg" alt="Tiger">
                </li>
                <li onclick="openModal('panda')">
                    <strong>Giant Panda</strong> - Conservation efforts are helping, but they remain at risk.
                    <img src="https://www.worldatlas.com/r/w1200/upload/59/17/19/shutterstock-688280269.jpg" alt="Giant Panda">
                </li>
                <li onclick="openModal('seaturtle')">
                    <strong>Sea Turtle</strong> - Faces dangers from pollution and climate change.
                    <img src="https://w0.peakpx.com/wallpaper/187/91/HD-wallpaper-green-turtle-in-blue-sea-animals.jpg" alt="Sea Turtle">
                </li>
                <li onclick="openModal('snowleopard')">
                    <strong>Snow Leopard</strong> - Affected by habitat fragmentation and hunting.
                    <img src="https://t3.ftcdn.net/jpg/03/18/47/72/360_F_318477235_qtvHD7hAYa8V4Z7cIejqhqIhWlS9hQ6N.jpg" alt="Snow Leopard">
                </li>
                <li onclick="openModal('bluewhale')">
                    <strong>Blue Whale</strong> - Endangered due to ship strikes and ocean pollution.
                    <img src="https://c4.wallpaperflare.com/wallpaper/598/885/248/whale-humpback-whale-animals-wallpaper-preview.jpg" alt="Blue Whale">
                </li>
            </ul>
        </section>
    </main>
    
    <!-- Modals for each species -->
    <div id="tiger" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeModal('tiger')">&times;</span>
            <h2>Tiger</h2>
            <p>The tiger is one of the most iconic and powerful animals on Earth. Tigers are known for their strength, agility, and beautiful striped fur. However, they are facing severe threats due to habitat destruction, poaching, and human-wildlife conflict. Tigers play a crucial role in maintaining the balance of the ecosystem by controlling prey populations. Conservation efforts focus on protecting tiger habitats and combating illegal poaching, especially for their skin and bones.</p>
        </div>
    </div>

    <div id="panda" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeModal('panda')">&times;</span>
            <h2>Giant Panda</h2>
            <p>Native to China, giant pandas are known for their distinctive black-and-white fur and primarily feed on bamboo. While their population has been growing due to successful conservation programs, they remain vulnerable due to their dependence on bamboo forests, which are being destroyed by deforestation and climate change. Conservation efforts, including habitat restoration and anti-poaching laws, have helped bring their numbers up, but they are still at risk of extinction.</p>
        </div>
    </div>

    <div id="seaturtle" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeModal('seaturtle')">&times;</span>
            <h2>Sea Turtle</h2>
            <p>Sea turtles are ancient reptiles that have roamed the oceans for over 100 million years. They are known for their long migrations and vital role in maintaining healthy marine ecosystems by controlling jellyfish populations and maintaining seagrass beds. However, sea turtles face numerous threats, including plastic pollution, climate change, illegal hunting, and loss of nesting sites. Protecting their habitats and reducing marine pollution are key to ensuring their survival.</p>
        </div>
    </div>

    <div id="snowleopard" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeModal('snowleopard')">&times;</span>
            <h2>Snow Leopard</h2>
            <p>Snow leopards are elusive big cats that live in the mountainous regions of Central Asia. They are known for their thick fur and long, bushy tails, which help them navigate the harsh cold climates. Snow leopards face threats from habitat fragmentation, poaching, and retaliation killings from herders. They are an apex predator, and their conservation is vital for maintaining the ecological balance in high-altitude ecosystems. Efforts to protect them include anti-poaching measures and education for local communities.</p>
        </div>
    </div>

    <div id="bluewhale" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeModal('bluewhale')">&times;</span>
            <h2>Blue Whale</h2>
            <p>The blue whale is the largest animal to have ever lived on Earth, growing up to 100 feet in length and weighing as much as 200 tons. Despite their massive size, blue whales are endangered primarily due to historical hunting (whaling) and modern threats such as ship strikes, ocean pollution, and climate change affecting their food sources. Blue whales are filter feeders, consuming vast amounts of krill to sustain their size. Conservation efforts focus on protecting their feeding grounds and ensuring safe migration routes.</p>
        </div>
    </div>

    <footer>
        <p>&copy; 2025 Guidoor. All rights reserved.</p>
    </footer>

    <script>
        // Open Modal
        function openModal(species) {
            document.getElementById(species).style.display = "block";
        }

        // Close Modal
        function closeModal(species) {
            document.getElementById(species).style.display = "none";
        }
    </script>
</body>
</html>
