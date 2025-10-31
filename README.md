<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Traços e Cores - Mandacaru</title>

  <link rel="stylesheet" href="style.css" />
  <!-- ✅ CDN do Glider.js -->
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/glider-js@1/glider.min.css" />
</head>
<body>
  <header>
    <a href="https://mandacaru.example.com" target="_blank">&#8592;</a>
    <h2>Eventos Corporativos</h2>
  </header>

  <main>
    <section class="perfil">
      <img src="img/6a6f3bc5feadcc11e67638471f32636f 1.png" alt="Marcela Camargo">
      <section>
        <h1>Traços e Cores</h1>
        <p>Empreendedora Marcela Camargo</p>
      </section>
    </section>

    <section class="quem-somos">
      <h3>Quem Somos?</h3>
      <p>
        A Traços e Cores é uma marca que transforma argila em louças doces e encantadoras.
        Cada peça é feita à mão pensada para trazer aconchego e um toque especial a cada
        peça no dia a dia. Cafés com amor, dão mais cor.
      </p>
    </section>

    <!-- 🔹 DESTAQUES -->
    <section>
      <section class="section-title">
        <h3>Destaques</h3>
        <section class="arrows">
          <button class="glider-prev-produtos">‹</button>
          <button class="glider-next-produtos">›</button>
        </section>
      </section>

      <section class="glider-contain">
        <section class="glider glider-produtos">
          <a href="https://exemplo.com/produto/1" target="_blank" class="card">
            <img src="img/e93f8407e4b1b90992048faaeeeafcbf 1.png" alt="Tigela Eat Me">
            <section class="info">
              <h4>Tigela Eat Me</h4>
              <p>R$75,00</p>
            </section>
          </a>
          <a href="https://exemplo.com/produto/2" target="_blank" class="card">
            <img src="img/0de8155e9649209e6e12cec39e7286c2 1.png" alt="Kit Japonês">
            <section class="info">
              <h4>Kit Japonês</h4>
              <p>R$34,00</p>
            </section>
          </a>
          <a href="https://exemplo.com/produto/3" target="_blank" class="card">
            <img src="img\c60beb587e3b87981d185e02fc94df4b 1.png" alt="Xicára Abelhinha">
            <section class="info">
              <h4>Xicára Abelinha</h4>
              <p>R$60,00</p>
            </section>
            <a href="https://exemplo.com/produto/3" target="_blank" class="card">
            <img src="img\392b7727f915e26be0b056acf6e383d1 1.png" alt="Tartera">
            <section class="info">
              <h4>Tartera</h4>
              <p>R$49,00</p>
            </section>
          </a>
        </section>
        <main id="dots-produtos" class="glider-dots"></div>
        </section>
    </section>

    <!-- 🔹 COMENTÁRIOS -->
    <section>
      <section class="section-title">
        <h3>Comentários</h3>
        <section class="arrows">
          <button class="glider-prev-comentarios">‹</button>
          <button class="glider-next-comentarios">›</button>
        </section>
      </section>

      <section class="glider-contain">
        <section class="glider glider-comentarios">
          <section class="comentario"><strong>Paula Goís</strong> Comprei essas canecas e foi a melhor coisa! lindas demais</section>
          <section class="comentario"><strong>Isadora Pires</strong> Pires lindos e acabamento impecável.</section>
          <section class="comentario"><strong>Marcela C.</strong> Atendimento super atencioso — amei.</section>
        </section>
        <section id="dots-comentarios" class="glider-dots"></section>
      </section>
    </section>
  </main>

    <h2>MANDACARU</h2>
    <p>Contate nosso suporte</p>
    <small>© 2025 Mandacaru. Todos os direitos reservados.</small>
 

  <!-- ✅ JS do Glider -->
  <script src="https://cdn.jsdelivr.net/npm/glider-js@1/glider.min.js"></script>

  <!-- ✅ Inicialização dos sliders com responsividade -->
  <script>
    window.addEventListener('load', function() {
      // Carrossel de produtos
      new Glider(document.querySelector('.glider-produtos'), {
        slidesToShow: 2,
        slidesToScroll: 1,
        draggable: true,
        dots: '#dots-produtos',
        arrows: {
          prev: '.glider-prev-produtos',
          next: '.glider-next-produtos'
        }
      });
      // Carrossel de comentários
      new Glider(document.querySelector('.glider-comentarios'), {
        slidesToShow: 1,
        slidesToScroll: 1,
        draggable: true,
        dots: '#dots-comentarios',
        arrows: {
          prev: '.glider-prev-comentarios',
          next: '.glider-next-comentarios'
        }
      });
    });
  </script>
</body>
</html>
