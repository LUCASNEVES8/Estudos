<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Power Soccer - Futebol em Cadeira de Rodas Motorizada</title>
    <style>
        /* Reset e estilos base */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }
        
        body {
            background-color: #f5f5f5;
            color: #333;
            line-height: 1.6;
        }
        
        /* Cabeçalho */
        header {
            background: linear-gradient(135deg, #1e5799 0%, #207cca 100%);
            color: white;
            padding: 2rem 0;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .header-content {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            position: relative;
            z-index: 2;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }
        
        .header-img {
            width: 100%;
            max-height: 300px;
            object-fit: cover;
            margin-top: 1rem;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        
        /* Navegação */
        nav {
            background-color: #333;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 20px;
        }
        
        .logo {
            color: white;
            font-weight: bold;
            font-size: 1.2rem;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 1.5rem;
        }
        
        .nav-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: #4dabf7;
        }
        
        .menu-toggle {
            display: none;
            cursor: pointer;
            color: white;
            font-size: 1.5rem;
        }
        
        /* Conteúdo principal */
        main {
            max-width: 1200px;
            margin: 2rem auto;
            padding: 0 20px;
        }
        
        section {
            margin-bottom: 3rem;
            background-color: white;
            border-radius: 8px;
            padding: 2rem;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        
        h2 {
            color: #1e5799;
            margin-bottom: 1.5rem;
            font-size: 1.8rem;
            border-bottom: 2px solid #eee;
            padding-bottom: 0.5rem;
        }
        
        p {
            margin-bottom: 1rem;
        }
        
        /* Galeria */
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 1.5rem;
        }
        
        .gallery img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            border-radius: 8px;
            transition: transform 0.3s;
            cursor: pointer;
        }
        
        .gallery img:hover {
            transform: scale(1.03);
        }
        
        /* Vídeo */
        .video-container {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
            margin: 2rem 0;
            border-radius: 8px;
        }
        
        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: none;
        }
        
        /* Rodapé */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 2rem 0;
            margin-top: 2rem;
        }
        
        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .social-links {
            margin: 1rem 0;
        }
        
        .social-links a {
            color: white;
            margin: 0 10px;
            font-size: 1.5rem;
            transition: color 0.3s;
        }
        
        .social-links a:hover {
            color: #4dabf7;
        }
        
        /* Responsividade */
        @media (max-width: 768px) {
            .nav-links {
                position: fixed;
                top: 70px;
                left: -100%;
                width: 100%;
                height: calc(100vh - 70px);
                background-color: #333;
                flex-direction: column;
                align-items: center;
                padding-top: 2rem;
                transition: left 0.3s;
            }
            
            .nav-links.active {
                left: 0;
            }
            
            .nav-links li {
                margin: 1rem 0;
            }
            
            .menu-toggle {
                display: block;
            }
            
            h1 {
                font-size: 2rem;
            }
            
            h2 {
                font-size: 1.5rem;
            }
        }
        
        @media (max-width: 480px) {
            .header-content, .nav-container, main, .footer-content {
                padding: 0 15px;
            }
            
            section {
                padding: 1.5rem;
            }
            
            h1 {
                font-size: 1.8rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="header-content">
            <h1>Power Soccer</h1>
            <p>O emocionante futebol em cadeira de rodas motorizada</p>
            <img src="https://images.unsplash.com/photo-1600679472829-3044539ce8ed?ixlib=rb-1.2.1&auto=format&fit=crop&w=1200&q=80" alt="Jogadores de Power Soccer em ação" class="header-img">
        </div>
    </header>
    
    <nav>
        <div class="nav-container">
            <div class="logo">Power Soccer</div>
            <div class="menu-toggle">☰</div>
            <ul class="nav-links">
                <li><a href="#sobre">Sobre</a></li>
                <li><a href="#regras">Regras</a></li>
                <li><a href="#equipamento">Equipamento</a></li>
                <li><a href="#galeria">Galeria</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </div>
    </nav>
    
    <main>
        <section id="sobre">
            <h2>Sobre o Power Soccer</h2>
            <p>O Power Soccer, também conhecido como Powerchair Football, é um esporte adaptado para pessoas com deficiências físicas que utilizam cadeiras de rodas motorizadas. É uma modalidade emocionante que combina estratégia, habilidade e trabalho em equipe.</p>
            <p>O esporte foi desenvolvido na França em 1970 e desde então se espalhou por todo o mundo, sendo praticado em mais de 30 países. No Brasil, o Power Soccer vem ganhando popularidade e já conta com várias equipes competitivas.</p>
            <p>O jogo é disputado em uma quadra de basquete com times de 4 jogadores cada (3 na linha e 1 goleiro). A bola usada é maior que uma de futebol tradicional (33cm de diâmetro) para facilitar o manejo com as cadeiras.</p>
            
            <div class="video-container">
                <iframe width="560" height="315" src="https://www.youtube.com/embed/VIDEO_ID" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>
        </section>
        
        <section id="regras">
            <h2>Regras Básicas</h2>
            <p>O Power Soccer segue regras específicas adaptadas para o uso das cadeiras de rodas motorizadas:</p>
            <ul style="margin-left: 2rem; margin-bottom: 1rem;">
                <li>Jogo dividido em 2 tempos de 20 minutos cada</li>
                <li>Contato entre cadeiras é permitido, mas com limites de força</li>
                <li>Dois toques consecutivos na bola são permitidos antes de passar para outro jogador</li>
                <li>O goleiro pode defender com as mãos dentro da área</li>
                <li>Laterais e escanteios são cobrados com a cadeira</li>
                <li>Faltas resultam em tiros livres diretos ou indiretos</li>
            </ul>
            <p>O objetivo, como no futebol tradicional, é marcar gols no time adversário. A habilidade de controlar a bola com a cadeira e trabalhar em equipe são fundamentais para o sucesso no jogo.</p>
        </section>
        
        <section id="equipamento">
            <h2>Equipamento Necessário</h2>
            <p>Para praticar Power Soccer são necessários alguns equipamentos específicos:</p>
            
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; margin-top: 1.5rem;">
                <div style="background: #f8f9fa; padding: 1.5rem; border-radius: 8px;">
                    <h3 style="color: #1e5799; margin-bottom: 1rem;">Cadeira de Rodas Especial</h3>
                    <p>Cadeiras motorizadas adaptadas com protetores frontais (bumpers) que ajudam no controle da bola e protegem os jogadores.</p>
                </div>
                
                <div style="background: #f8f9fa; padding: 1.5rem; border-radius: 8px;">
                    <h3 style="color: #1e5799; margin-bottom: 1rem;">Bola Oficial</h3>
                    <p>Bola de 33cm de diâmetro (maior que uma bola de futebol tradicional) para facilitar o manejo com as cadeiras.</p>
                </div>
                
                <div style="background: #f8f9fa; padding: 1.5rem; border-radius: 8px;">
                    <h3 style="color: #1e5799; margin-bottom: 1rem;">Quadra Adaptada</h3>
                    <p>Geralmente uma quadra de basquete com marcações específicas para o Power Soccer.</p>
                </div>
            </div>
        </section>
        
        <section id="galeria">
            <h2>Galeria de Fotos</h2>
            <p>Confira momentos emocionantes do Power Soccer ao redor do mundo:</p>
            
            <div class="gallery">
                <img src="https://images.unsplash.com/photo-1543357480-c60d400e2ef9?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Jogo de Power Soccer">
                <img src="https://images.unsplash.com/photo-1517649763962-0c623066013b?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Jogador controlando a bola">
                <img src="https://images.unsplash.com/photo-1519861531473-9200262188bf?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Time comemorando gol">
                <img src="https://images.unsplash.com/photo-1541252260731-5f1231f6f6b9?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Goleiro defendendo">
                <img src="https://images.unsplash.com/photo-1517649763962-0c623066013b?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Torneio de Power Soccer">
                <img src="https://images.unsplash.com/photo-1543357480-c60d400e2ef9?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Jogadores em formação">
            </div>
        </section>
        
        <section id="contato">
            <h2>Entre em Contato</h2>
            <p>Interessado em praticar Power Soccer ou saber mais sobre o esporte? Entre em contato conosco!</p>
            
            <form style="margin-top: 1.5rem; display: grid; gap: 1rem; max-width: 600px;">
                <div>
                    <label for="nome" style="display: block; margin-bottom: 0.5rem;">Nome:</label>
                    <input type="text" id="nome" style="width: 100%; padding: 0.5rem; border: 1px solid #ddd; border-radius: 4px;">
                </div>
                
                <div>
                    <label for="email" style="display: block; margin-bottom: 0.5rem;">Email:</label>
                    <input type="email" id="email" style="width: 100%; padding: 0.5rem; border: 1px solid #ddd; border-radius: 4px;">
                </div>
                
                <div>
                    <label for="mensagem" style="display: block; margin-bottom: 0.5rem;">Mensagem:</label>
                    <textarea id="mensagem" rows="5" style="width: 100%; padding: 0.5rem; border: 1px solid #ddd; border-radius: 4px;"></textarea>
                </div>
                
                <button type="submit" style="background: #1e5799; color: white; border: none; padding: 0.8rem 1.5rem; border-radius: 4px; cursor: pointer; transition: background 0.3s;">Enviar Mensagem</button>
            </form>
        </section>
    </main>
    
    <footer>
        <div class="footer-content">
            <p>&copy; 2023 Power Soccer Brasil - Todos os direitos reservados</p>
            <div class="social-links">
                <a href="#" aria-label="Facebook">📘</a>
                <a href="#" aria-label="Instagram">📷</a>
                <a href="#" aria-label="Twitter">🐦</a>
                <a href="#" aria-label="YouTube">▶️</a>
            </div>
            <p>Desenvolvido com ❤️ para o esporte adaptado</p>
        </div>
    </footer>
    
    <script>
        // Menu mobile
        const menuToggle = document.querySelector('.menu-toggle');
        const navLinks = document.querySelector('.nav-links');
        
        menuToggle.addEventListener('click', () => {
            navLinks.classList.toggle('active');
        });
        
        // Fechar menu ao clicar em um link
        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', () => {
                navLinks.classList.remove('active');
            });
        });
    </script>
</body>
</html>
