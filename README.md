/* Загальні стилі */
body {
    margin: 0;
    font-family: 'Arial', sans-serif;
    background: #F6F0E9;
    color: #3A2F5C;
    scroll-behavior: smooth; /* плавний скрол */
}

a {
    color: #8B5EAA;
    text-decoration: none;
}

a:hover {
    text-decoration: underline;
}

/* Плавне з’явлення елементів */
.fade-in {
    opacity: 0;
    transform: translateY(20px);
    animation: fadeInUp 1s forwards;
    animation-delay: 0.2s;
}

@keyframes fadeInUp {
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* Шапка */
header.hero {
    background: #DAC7E0;
    text-align: center;
    padding: 40px 20px;
}

header.hero .logo {
    max-width: 180px;
    width: 100%;
    height: auto;
    margin-bottom: 20px;
}

header.hero h1, header.hero p {
    animation: fadeInUp 1s forwards;
}

/* Картки товарів */
.cards-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.card {
    background: #fff;
    border-radius: 12px;
    width: 300px;
    box-shadow: 0 6px 15px rgba(0,0,0,0.15);
    overflow: hidden;
    transition: transform 0.3s, box-shadow 0.3s;
    opacity: 0;
    transform: translateY(20px);
    animation: fadeInUp 1s forwards;
}

.card:hover {
    transform: translateY(-8px) scale(1.03);
    box-shadow: 0 12px 25px rgba(0,0,0,0.25);
}

/* Галерея */
.gallery-container img {
    width: 250px;
    border-radius: 12px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    transition: transform 0.3s, box-shadow 0.3s;
    opacity: 0;
    transform: translateY(20px);
    animation: fadeInUp 1s forwards;
}

.gallery-container img:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 20px rgba(0,0,0,0.2);
}

/* About та контакт */
.about, .contact {
    padding: 40px 20px;
    max-width: 900px;
    margin: 0 auto;
    text-align: center;
    opacity: 0;
    transform: translateY(20px);
    animation: fadeInUp 1s forwards;
}

.about h2, .contact h2 {
    margin-bottom: 20px;
}

/* Футер */
.site-footer {
    background: #3A2F5C;
    color: #F6F0E9;
    text-align: center;
    padding: 30px 20px;
    display: flex;
    flex-direction: column;
    align-items: center;
    opacity: 0;
    transform: translateY(20px);
    animation: fadeInUp 1s forwards;
}

/* Адаптивність */
@media (max-width: 992px) {
    .card {
        width: 45%;
    }
    .gallery-container img {
        width: 45%;
    }
}

@media (max-width: 600px) {
    .card {
        width: 90%;
    }
    .gallery-container img {
        width: 90%;
    }
}
// Галерея свічок
const galleryContainer = document.querySelector('.gallery-container');
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

candleImages.forEach((src, index) => {
    const img = document.createElement('img');
    img.src = src;
    img.alt = "Свічка";
    img.classList.add('fade-in');
    img.style.animationDelay = `${0.2 + index * 0.2}s`; // по черзі з’являються
    galleryContainer.appendChild(img);
});

// Анімація для карток товарів
const cards = document.querySelectorAll('.card');
cards.forEach((card, index) => {
    card.classList.add('fade-in');
    card.style.animationDelay = `${0.2 + index * 0.2}s`;
});

// Анімація для about, contact та футера
document.querySelector('.about').classList.add('fade-in');
document.querySelector('.contact').classList.add('fade-in');
document.querySelector('.site-footer').classList.add('fade-in');

