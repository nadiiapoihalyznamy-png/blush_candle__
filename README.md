<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Blush Candle — Ніжні ароматичні свічки</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header class="hero">
    <img src="https://honeylife.ua/image/cache/catalog/1%20svschku/%D0%94%D0%BE%20%D0%B4%D0%BD%D1%8F%20%D0%BD%D0%B0%D1%80%D0%BE%D0%B4%D0%B6%D0%B5%D0%BD%D0%BD%D1%8F/%D0%BA%D0%B5%D1%80/1IMG_2408_11zon-500x500.jpg" alt="Blush Candle" class="logo">
    <h1>Blush Candle</h1>
    <p>Ніжність, аромат та тепло для вашого дому</p>
</header>

<section class="products">
    <h2>Наші свічки 🕯️</h2>
    <div class="cards-container">
        <div class="card cheap">
            <img src="https://www.laredim.com/static/content/thumbs/1520-1520/9/31/6hf2rd-d47b91e8faecd549b55a0af419b83319.jpeg" alt="Дешеві свічки">
            <h3>Свічки за $10</h3>
            <p>Бюджетний сегмент — чудовий вибір для подарунка або затишного вечора.</p>
            <span class="price">$10</span>
        </div>
        <div class="card mid">
            <img src="https://cdn4.jysk.com/getimage/wd3.large/243189" alt="Середні свічки">
            <h3>Свічки за $50</h3>
            <p>Середній сегмент — ароматні свічки з натуральними есенціями.</p>
            <span class="price">$50</span>
        </div>
        <div class="card luxe">
            <img src="https://images.prom.ua/4925164095_w640_h640_4925164095.jpg" alt="Люкс свічки">
            <h3>Люкс свічки за $100</h3>
            <p>Преміум-серія — ароматичні свічки ручної роботи з елітними ароматами.</p>
            <span class="price">$100</span>
        </div>
    </div>
</section>

<section class="about">
    <h2>Про магазин</h2>
    <p>
        Магазин Blush Candle створений, щоб дарувати затишок та тепло у вашому домі. 
        Наші ароматичні свічки допомагають розслабитися, створюють особливу атмосферу 
        та роблять буденні вечори чарівними. Ми подбали про те, щоб ви насолоджувалися продуктами, 
        а не турбувалися про деталі виготовлення — кожна свічка створена з любов’ю та турботою.
    </p>
</section>

<section class="gallery">
    <h2>Галерея наших свічок</h2>
    <div class="gallery-container">
    </div>
</section>

<section class="contact">
    <h2>Звʼязатися з нами</h2>
    <p><strong>Ткачук Надія Олександрівна</strong><br>
       Група: 4-12 ФТБ</p>
    <p>Email: <a href="mailto:n.tkachuk_frhtb_12_22_b_d@knute.edu.ua">n.tkachuk_frhtb_12_22_b_d@knute.edu.ua</a></p>
</section>

<footer class="site-footer">
    <img src="https://honeylife.ua/image/cache/catalog/1%20svschku/%D0%94%D0%BE%20%D0%B4%D0%BD%D1%8F%20%D0%BD%D0%B0%D1%80%D0%BE%D0%B4%D0%B6%D0%B5%D0%BD%D0%BD%D1%8F/%D0%BA%D0%B5%D1%80/1IMG_2408_11zon-500x500.jpg" alt="Blush Candle" class="footer-logo">
    <p>© 2025 Blush Candle — ніжне світло та аромат для вашого дому</p>
    <p>Ткачук Надія Олександрівна | Група: 4-12 ФТБ</p>
    <p>Email: <a href="mailto:n.tkachuk_frhtb_12_22_b_d@knute.edu.ua">n.tkachuk_frhtb_12_22_b_d@knute.edu.ua</a></p>
</footer>

<script>
const galleryContainer = document.querySelector('.gallery-container');

// Масив твоїх фото свічок
const candleImages = [
    'https://cdn2.jysk.com/getimage/wd3.large/234292',
    'https://honeylife.ua/image/cache/catalog/1%20svschku/%D0%94%D0%BE%20%D0%B4%D0%BD%D1%8F%20%D0%BD%D0%B0%D1%80%D0%BE%D0%B4%D0%B6%D0%B5%D0%BD%D0%BD%D1%8F/%D0%BC%D0%B0%D0%BD%D0%B3%D0%BE/2IMG_2359-500x500.JPG',
    'https://images.prom.ua/5266386900_w640_h320_svechi-s-nadpisyu.jpg',
    'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSyqgUM6I8E1R8zx4SyLgBUqkJzoQZm76H1HQ&s',
    'https://zapalyizatyshok.com.ua/content/images/12/480x360l95nn0/set-z-trokh-serednikh-svichok-86672388340730.jpg',
    'https://content1.rozetka.com.ua/goods/images/big_tile/546305043.jpg',
    'https://image-thumbs.shafastatic.net/-96198790_310_430',
    'https://image-thumbs.shafastatic.net/2168162432_310_430'
];

// Вставляємо фото на сторінку
candleImages.forEach(src => {
    const img = document.createElement('img');
    img.src = src;
    img.alt = "Свічка";
    galleryContainer.appendChild(img);
});
</script>

</body>
</html>
