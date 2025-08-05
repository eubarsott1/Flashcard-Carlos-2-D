<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Flashcards - Futebol</title>
    <style>
      /* Estilos básicos para os flashcards */
      body {
        font-family: Arial, sans-serif;
        background: #f0f2f5;
        margin: 0;
        padding: 20px;
      }
      .cabecalho {
        text-align: center;
        margin-bottom: 30px;
      }
      h2 {
        color: #2c3e50;
      }
      #container {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
        gap: 20px;
        max-width: 1000px;
        margin: 0 auto;
      }
      .cartao {
        perspective: 1000px;
        cursor: pointer;
      }
      .geral {
        position: relative;
        width: 100%;
        height: 200px;
        transform-style: preserve-3d;
        transition: transform 0.6s;
      }
      .cartao.flipped .geral {
        transform: rotateY(180deg);
      }
      .cartao-conteudo {
        position: absolute;
        width: 100%;
        height: 100%;
        border-radius: 12px;
        box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        background: white;
        backface-visibility: hidden;
        padding: 20px;
        box-sizing: border-box;
      }
      .card-front {
        color: #2c3e50;
      }
      .card-back {
        background: #2980b9;
        color: white;
        transform: rotateY(180deg);
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
      }
      .design-conteudo h3 {
        margin-top: 0;
        font-weight: bold;
      }
      .cartao-conteudo-pergunta {
        margin: 15px 0 10px;
        font-size: 1.1rem;
      }
      .cartao-conteudo-resposta {
        font-style: italic;
        color: #555;
      }
      footer {
        text-align: center;
        margin-top: 40px;
        font-size: 0.9rem;
        color: #555;
      }
      footer a {
        color: #2980b9;
        text-decoration: none;
      }
      footer a:hover {
        text-decoration: underline;
      }
    </style>
</head>
<body>
    <header class="cabecalho">
        <div class="titulo">
            <h2>Flashcards de Futebol ⚽️</h2>
        </div>
    </header>
    <main>
        <section id="container">
            <!-- Card 1 -->
            <article class="cartao" onclick="this.classList.toggle('flipped')">
                <div class="geral">
                    <div class="cartao-conteudo card-front">
                        <div class="design-conteudo">
                            <h3>Futebol na veia</h3>
                        </div>
                        <div class="cartao-conteudo-pergunta">Quem foi o campeão da Copa de 2018?</div>
                        <div class="cartao-conteudo-resposta">França, eles mandaram bem demais!</div>
                    </div>
                    <div class="cartao-conteudo card-back">
                        <h3>Resumo</h3>
                        <p>A França ganhou a Copa na Rússia, jogaram muito e conquistaram geral.</p>
                    </div>
                </div>
            </article>

            <!-- Card 2 -->
            <article class="cartao" onclick="this.classList.toggle('flipped')">
                <div class="geral">
                    <div class="cartao-conteudo card-front">
                        <div class="design-conteudo">
                            <h3>Futebol na veia</h3>
                        </div>
                        <div class="cartao-conteudo-pergunta">Quem é o rei dos gols na seleção do Brasil?</div>
                        <div class="cartao-conteudo-resposta">Pelé, o cara é mito!</div>
                    </div>
                    <div class="cartao-conteudo card-back">
                        <h3>Resumo</h3>
                        <p>Pelé marcou 77 gols com a camisa verde e amarela, é lenda viva.</p>
                    </div>
                </div>
            </article>

            <!-- Card 3 -->
            <article class="cartao" onclick="this.classList.toggle('flipped')">
                <div class="geral">
                    <div class="cartao-conteudo card-front">
                        <div class="design-conteudo">
                            <h3>Futebol na veia</h3>
                        </div>
                        <div class="cartao-conteudo-pergunta">Qual time é o rei da Champions League?</div>
                        <div class="cartao-conteudo-resposta">Real Madrid, eles são insanos nessa competição.</div>
                    </div>
                    <div class="cartao-conteudo card-back">
                        <h3>Resumo</h3>
                        <p>Com 14 títulos, o Real domina a Champions e coleciona troféus.</p>
                    </div>
                </div>
            </article>

            <!-- Card 4 -->
            <article class="cartao" onclick="this.classList.toggle('flipped')">
                <div class="geral">
                    <div class="cartao-conteudo card-front">
                        <div class="design-conteudo">
                            <h3>Futebol na veia</h3>
                        </div>
                        <div class="cartao-conteudo-pergunta">Quem ganhou a Bola de Ouro em 2021?</div>
                        <div class="cartao-conteudo-resposta">Messi, claro, o craque nunca decepciona!</div>
                    </div>
                    <div class="cartao-conteudo card-back">
                        <h3>Resumo</h3>
                        <p>Messi levou a Bola de Ouro 2021, mais um prêmio pra coleção do gênio.</p>
                    </div>
                </div>
            </article>

            <!-- Card 5 -->
            <article class="cartao" onclick="this.classList.toggle('flipped')">
                <div class="geral">
                    <div class="cartao-conteudo card-front">
                        <div class="design-conteudo">
                            <h3>Futebol na veia</h3>
                        </div>
                        <div class="cartao-conteudo-pergunta">Quanto tempo dura um jogo oficial?</div>
                        <div class="cartao-conteudo-resposta">90 minutos, na moral.</div>
                    </div>
                    <div class="cartao-conteudo card-back">
                        <h3>Resumo</h3>
                        <p>São dois tempos de 45 minutos cada, sem contar os acréscimos.</p>
                    </div>
                </div>
            </article>

            <!-- Card 6 -->
            <article class="cartao" onclick="this.classList.toggle('flipped')">
                <div class="geral">
                    <div class="cartao-conteudo card-front">
                        <div class="design-conteudo">
                            <h3>Futebol na veia</h3>
                        </div>
                        <div class="cartao-conteudo-pergunta">Quem é o "Fenômeno"?</div>
                        <div class="cartao-conteudo-resposta">Ronaldo, o cara que foi um monstro no ataque.</div>
                    </div>
                    <div class="cartao-conteudo card-back">
                        <h3>Resumo</h3>
                        <p>Ronaldo Nazário marcou história como um dos melhores atacantes do mundo.</p>
                    </div>
                </div>
            </article>

            <!-- Card 7 -->
            <article class="cartao" onclick="this.classList.toggle('flipped')">
                <div class="geral">
                    <div class="cartao-conteudo card-front">
                        <div class="design-conteudo">
                            <h3>Futebol na veia</h3>
                        </div>
                        <div class="cartao-conteudo-pergunta">Qual jogador brasileiro ganhou mais Copas?</div>
                        <div class="cartao-conteudo-resposta">Pelé, o rei das Copas.</div>
                    </div>
                    <div class="cartao-conteudo card-back">
                        <h3>Resumo</h3>
                        <p>Ele ganhou 3 Copas (58, 62 e 70) e é lenda no futebol.</p>
                    </div>
                </div>
            </article>

            <!-- Card 8 -->
            <article class="cartao" onclick="this.classList.toggle('flipped')">
                <div class="geral">
                    <div class="cartao-conteudo card-front">
                        <div class="design-conteudo">
                            <h3>Futebol na veia</h3>
                        </div>
                        <div class="cartao-conteudo-pergunta">Qual time tem o apelido “Furacão”?</div>
                        <div class="cartao-conteudo-resposta">Atlético Paranaense, que joga com tudo!</div>
                    </div>
                    <div class="cartao-conteudo card-back">
                        <h3>Resumo</h3>
                        <p>Conhecido pelo estilo agressivo, o Atlético Paranaense é chamado de Furacão.</p>
                    </div>
                </div>
            </article>

            <!-- Card 9 -->
            <article class="cartao" onclick="this.classList.toggle('flipped')">
                <div class="geral">
                    <div class="cartao-conteudo card-front">
                        <div class="design-conteudo">
                            <h3>Futebol na veia</h3>
                        </div>
                        <div class="cartao-conteudo-pergunta">Quem fez o gol que garantiu o título do Brasil na Copa de 1994?</div>
                        <div class="cartao-conteudo-resposta">Dunga, no pênalti final.</div>
                    </div>
                    <div class="cartao-conteudo card-back">
                        <h3>Resumo</h3>
                        <p>Dunga marcou o pênalti decisivo contra a Itália e levou o Brasil ao tetracampeonato.</p>
                    </div>
                </div>
            </article>
        </section>
    </main>
    <footer>
        <div class="footer-text">
            <a class="texto-rodape">Projeto desenvolvido pela Alura. Melhorado e aplicado por Rafael K.T Nakatsuchi</a>
        </div>
        <div class="mark">
            <a href="https://github.com/eubarsott1">2025 | @eu_.barsotti</a>
        </div>
    </footer>
</body>
</html>
