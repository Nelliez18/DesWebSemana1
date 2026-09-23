```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Blog Semântico</title>
    <style>
        /* Estilos básicos apenas para organizar visualmente o layout em colunas */
        body { font-family: Arial, sans-serif; line-height: 1.6; margin: 20px; }
        header { background: #333; color: #fff; padding: 10px 20px; }
        nav a { color: #fff; margin-right: 15px; text-decoration: none; }
        .container { display: flex; gap: 20px; margin-top: 20px; }
        main { flex: 3; }
        aside { flex: 1; background: #f4f4f4; padding: 15px; border-radius: 5px; }
        article { margin-bottom: 30px; border-bottom: 1px solid #ccc; padding-bottom: 20px; }
        img { max-width: 100%; height: auto; display: block; margin-top: 10px; }
        form div { margin-bottom: 15px; }
        form label { display: block; font-weight: bold; margin-bottom: 5px; }
        form input[type="text"], form input[type="email"], form input[type="number"], form select { width: 100%; padding: 8px; box-sizing: border-box; }
        footer { text-align: center; margin-top: 20px; padding: 10px; background: #333; color: #fff; }
    </style>
</head>
<body>

    <!-- Cabeçalho principal com título e navegação -->
    <header>
        <h1>DevBlog</h1>
        <nav>
            <a href="#home">Home</a>
            <a href="#artigos">Artigos</a>
            <a href="#sobre">Sobre</a>
        </nav>
    </header>

    <!-- Container flexível para organizar o conteúdo principal e a barra lateral -->
    <div class="container">
        
        <!-- Conteúdo principal do blog -->
        <main id="artigos">
            <article>
                <h2>Entendendo o HTML5 Semântico</h2>
                <p>Usar tags semânticas como header, main, article e aside ajuda os motores de busca (SEO) e tecnologias de assistência a compreenderem a estrutura real do seu site.</p>
                <img src="https://picsum.photos" alt="Ilustração sobre código e semântica web">
            </article>

            <article>
                <h2>A Importância da Validação de Formulários</h2>
                <p>Validar dados diretamente no navegador melhora a experiência do usuário, impedindo o envio de informações incorretas antes mesmo de chegarem ao servidor.</p>
                <img src="https://picsum.photos" alt="Ilustração sobre segurança e formulários web">
            </article>
        </main>

        <!-- Barra lateral com o formulário de inscrição -->
        <aside>
            <h3>Inscrição na Newsletter</h3>
            <!-- Formulário com método GET para exibir os dados inseridos diretamente na URL -->
            <form action="" method="get">
                
                <div>
                    <label for="nome">Nome Completo:</label>
                    <input type="text" id="nome" name="nome" minlength="3" required placeholder="Mínimo 3 letras">
                </div>

                <div>
                    <label for="email">E-mail:</label>
                    <input type="email" id="email" name="email" required placeholder="seu@email.com">
                </div>

                <div>
                    <label for="idade">Idade:</label>
                    <input type="number" id="idade" name="idade" min="18" max="120" required placeholder="De 18 a 120 anos">
                </div>

                <div>
                    <label for="assunto">Assunto de Interesse:</label>
                    <select id="assunto" name="assunto">
                        <option value="html">HTML5 & CSS3</option>
                        <option value="javascript">JavaScript</option>
                        <option value="carreira">Carreira em Tech</option>
                    </select>
                </div>

                <div>
                    <label>
                        <input type="checkbox" id="termos" name="termos" required>
                        Aceito os termos de privacidade
                    </label>
                </div>

                <button type="submit">Inscrever-se</button>
            </form>
        </aside>

    </div>

    <!-- Rodapé da página -->
    <footer>
        <p>&copy; 2026 DevBlog. Todos os direitos reservados.</p>
    </footer>

</body>
</html>
```
