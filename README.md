<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Конечная форма страницы</title>
  <style>
    /* Общие стили */
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
    }

    /* Стили для шапки */
    header {
      background: linear-gradient(to right, #adadad, #2c2c2c);
      color: #fff;
      padding: 20px 0;
      text-align: center;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }

    /* Стили для галереи изображений */
    .gallery,
    .dual-gallery {
      opacity: 0;
      transform: translateY(20px);
      transition: opacity 0.5s ease, transform 0.5s ease;
    }

    .gallery.animate,
    .dual-gallery.animate {
      opacity: 1;
      transform: translateY(0);
    }

    .gallery,
    .dual-gallery {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      grid-gap: 20px;
      max-width: 800px;
      margin: 20px auto;
      padding: 20px;
      background-color: #fff;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    .gallery-item,
    .dual-gallery-item {
      text-align: center;
    }

    .gallery-item img,
    .dual-gallery-item img {
      width: 100%;
      height: auto;
      border-radius: 8px;
      cursor: pointer;
      transition: transform 0.3s ease;
    }

    .gallery-item img:hover,
    .dual-gallery-item img:hover {
      transform: scale(1.05);
    }

    .caption,
    .dual-caption {
      margin-top: 10px;
    }
  </style>
</head>
<body>

<header>
  <h1>Seven-Miracles</h1>
</header>

<div class="gallery">
  <div class="gallery-item">
    <a href="ссылка_на_страницу_продукта_1">
      <img src="2023-11-19_23-15-34.png" alt="Имя продукта 1">
    </a>
    <div class="caption">Наша команда непосредственно</div>
  </div>
  
  <div class="gallery-item">
    <a href="ссылка_на_страницу_продукта_2">
      <img src="Теория.jpg" alt="Имя продукта 2">
    </a>
    <div class="caption">Теория об электричестве</div>
  </div>
  
  <div class="gallery-item">
    <a href="Это второй main.html">
      <img src="2023-11-19_23-16-05.png" alt="Имя продукта 3">
    </a>
    <div class="caption">Другие калькуляторы</div>
  </div>
  
  <div class="gallery-item">
    <a href="ссылка_на_страницу_продукта_4">
      <img src="2023-11-19_23-27-40.png" alt="Имя продукта 4">
    </a>
    <div class="caption">О нас</div>
  </div>
</div>

<div class="dual-gallery">
  <div class="dual-gallery-item">
    <img src="2023-11-20_01-10-20.png" alt="Первая картинка">
    <div class="dual-caption">Искусство - это форма самовыражения, которая отражает чувства, идеи, эмоции и видение мира через различные творческие средства. Оно является неотъемлемой частью человеческой культуры и имеет множество форм: живопись, скульптура, литература, музыка, театр, кино, танец и многое другое. Искусство вдохновляет, провоцирует мысли и вызывает эмоции у зрителей, слушателей или читателей. Оно способно передавать глубокие смыслы, олицетворять красоту и разнообразие человеческого опыта. Искусство может быть способом выражения индивидуальности художника или средством социальной критики и комментариев.

      Через века искусство служило источником вдохновения для различных культур и обществ. Оно является мощным средством передачи истории, традиций и ценностей, сохраняя наследие прошлого и формируя наше понимание мира.
    </div>
  </div>
  
  <div class="dual-gallery-item">
    <img src="2023-11-20_01-29-09.png" alt="Вторая картинка">
    <div class="dual-caption">Эмоции - это сложные и многогранные переживания, которые возникают в ответ на различные ситуации, события или внутренние переживания. Они представляют собой реакции нашего организма на внешние воздействия и внутренние мысли, вызывая физиологические и психологические изменения.

      Эмоции могут быть разнообразными - от радости, грусти и страха до удивления, злости и восхищения. Каждая эмоция имеет свою уникальную особенность и может проявляться на разном уровне интенсивности. Они могут быть кратковременными или длительными, вспышечными или постоянными, в зависимости от ситуации и субъективного восприятия.
      
      Эмоции играют важную роль в нашей жизни. Они помогают нам понимать и интерпретировать окружающий мир, влияют на наше поведение и принятие решений.</div>
  </div>
</div>

<script>
  document.addEventListener("DOMContentLoaded", function() {
    const gallerySection = document.querySelector('.gallery');
    const dualGallerySection = document.querySelector('.dual-gallery');

    // Добавляем класс animate для запуска анимации
    gallerySection.classList.add('animate');
    dualGallerySection.classList.add('animate');
  });
</script>

</body>
</html>
