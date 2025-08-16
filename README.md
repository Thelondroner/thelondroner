<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfólio Imobiliário</title>
    <!-- Tailwind CSS via CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts - Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <!-- Font Awesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            /* Using the hero image as the main background for the entire body */
            background-image: url('https://i.imgur.com/C6pcLi3.jpg');
            background-size: cover;
            background-repeat: no-repeat;
            background-attachment: fixed; /* Ensures the background stays put as you scroll slides */
            background-position: center;
        }
        .slide {
            display: none;
        }
        .slide.active {
            display: flex;
        }
        /* Custom styles for the video placeholder */
        .video-placeholder {
            position: relative;
            width: 100%;
            padding-top: 56.25%; /* 16:9 Aspect Ratio */
            background-color: #000;
            cursor: pointer;
        }
        .video-placeholder-icon {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 4rem;
            color: white;
            opacity: 0.8;
            transition: opacity 0.3s;
        }
        .video-placeholder:hover .video-placeholder-icon {
            opacity: 1;
        }
    </style>
</head>
<body class="flex items-center justify-center min-h-screen p-4">

    <!-- Presentation Container with semi-transparent background -->
    <div id="presentation-container" class="relative w-full max-w-5xl h-[calc(100vh-2rem)] md:h-[600px] bg-black bg-opacity-40 rounded-2xl shadow-xl flex flex-col overflow-hidden transition-all duration-500">

        <!-- Slides Container -->
        <div id="slides-wrapper" class="w-full flex-1 flex transition-all duration-500 ease-in-out">
            
            <!-- Slide 1: Title Slide -->
            <div id="slide-1" class="slide active w-full flex-shrink-0 flex flex-col items-center justify-center p-8 md:p-16 text-center transition-opacity duration-500">
                <h1 class="text-4xl md:text-6xl font-extrabold text-white mb-4">The Londroner | Aerial & Real Estate Photography</h1>
                <p class="text-lg md:text-2xl font-medium text-gray-200">Serviços Profissionais de Fotografia & Vídeo com Drone</p>
            </div>

            <!-- Slide 2: About Me -->
            <div id="slide-2" class="slide w-full flex-shrink-0 flex flex-col items-center justify-center p-8 md:p-16">
                <h2 class="text-3xl md:text-4xl font-bold text-white mb-6">Até agora...</h2>
                <div class="max-w-xl text-center">
                    <p class="text-base md:text-lg text-gray-300 leading-relaxed mb-4">
                        Com mais de uma década de experiência em fotografia, e mais de 6 anos em fotografia imobiliária e aérea, sou apaixonado por capturar a essência de cada propriedade.
                    </p>
                    <p class="text-base md:text-lg text-gray-300 leading-relaxed">
                        Exibi o meu trabalho nas Galerias OXO em Londres na "London Photo Show" e fui publicado numa revista finlandesa de fotografia de rua, demonstrando a minha versatilidade e reconhecimento artístico.
                    </p>
                </div>
            </div>
            
            <!-- Slide 3: Additional Projects -->
            <div id="slide-3" class="slide w-full flex-shrink-0 flex flex-col items-center justify-center p-8 md:p-16">
                <h2 class="text-3xl md:text-4xl font-bold text-white mb-6 text-center">Outros Projetos</h2>
                <div class="max-w-xl text-center">
                    <p class="text-base md:text-lg text-gray-300 leading-relaxed mb-4">
                        Criei um documento para uma agência de aluguer casas de férias no Panamá, com o objetivo de ajudar os proprietários a melhorar o design das suas casas. A finalidade era torná-las o mais atraente possível para maximizar o revenue.
                    </p>
                    <p class="text-base md:text-lg text-gray-300 leading-relaxed">
                        Além disso, na minha experiência anterior numa startup de short term luxury vacation rentals, desenvolvi um "Guia do Fotógrafo". Este guia instruía os fotógrafos sobre a melhor forma de capturar a essência de uma casa, garantindo que a qualidade visual refletisse o padrão de luxo.
                    </p>
                </div>
            </div>

            <!-- Slide 4: Services Offered (formerly Slide 3) -->
            <div id="slide-4" class="slide w-full flex-shrink-0 flex flex-col items-center justify-center p-8 md:p-16">
                <h2 class="text-3xl md:text-4xl font-bold text-white mb-8">Serviços</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-2 gap-8 w-full max-w-4xl justify-center">
                    <!-- Re-added the background image for Professional Photography -->
                    <div class="p-6 rounded-xl flex flex-col items-center text-center relative bg-black bg-opacity-50 border border-gray-700 bg-cover bg-center" style="background-image: url('https://i.imgur.com/2RFs425.jpg');">
                        <div class="relative z-10 flex flex-col items-center">
                            <i class="fas fa-camera text-4xl text-white mb-4"></i>
                            <h3 class="text-xl font-semibold text-white mb-2">Fotografia Profissional</h3>
                            <p class="text-sm text-gray-200">Fotografias de interior, exterior e detalhe que captam todos os ângulos.</p>
                        </div>
                    </div>
                    <!-- Updated the background image for Aerial Drone Video -->
                    <div class="p-6 rounded-xl flex flex-col items-center text-center relative bg-black bg-opacity-50 border border-gray-700 bg-cover bg-center" style="background-image: url('https://i.imgur.com/4JyoCVs.jpeg');">
                        <div class="relative z-10 flex flex-col items-center">
                            <i class="fas fa-drone text-4xl text-white mb-4"></i>
                            <h3 class="text-xl font-semibold text-white mb-2">Vídeo Aéreo com Drone</h3>
                            <p class="text-sm text-gray-200">Imagens aéreas em 4K de alta definição e fotos dinâmicas para mostrar a localização da propriedade.</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Slide 5: Interior Photography Portfolio (formerly Slide 4) -->
            <div id="slide-5" class="slide w-full flex-shrink-0 flex flex-col items-center p-8 md:p-16 overflow-y-auto">
                <h2 class="text-3xl md:text-4xl font-bold text-white mb-8">Interiores</h2>
                <div class="grid grid-cols-2 gap-4 w-full">
                    <img src="https://i.imgur.com/qm6Vg9H.jpeg" alt="Imagem de portfólio de interior de sala de estar" class="w-full h-48 object-cover rounded-lg shadow-md transition-transform duration-300 hover:scale-105">
                    <img src="https://i.imgur.com/5k4p6xd.jpeg" alt="Imagem de portfólio de interior de cozinha" class="w-full h-48 object-cover rounded-lg shadow-md transition-transform duration-300 hover:scale-105">
                    <img src="https://i.imgur.com/mxVDgW1.jpeg" alt="Imagem de portfólio de interior de quarto" class="w-full h-48 object-cover rounded-lg shadow-md transition-transform duration-300 hover:scale-105">
                    <img src="https://i.imgur.com/z4cSZcJ.jpeg" alt="Imagem de portfólio de interior de casa de banho" class="w-full h-48 object-cover rounded-lg shadow-md transition-transform duration-300 hover:scale-105">
                </div>
            </div>

            <!-- Slide 6: Exterior Photography Portfolio (formerly Slide 5) -->
            <div id="slide-6" class="slide w-full flex-shrink-0 flex flex-col items-center p-8 md:p-16 overflow-y-auto">
                <h2 class="text-3xl md:text-4xl font-bold text-white mb-8">Exterior Terrestre & Aéreo</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-4 w-full max-w-3xl">
                    <img src="https://placehold.co/600x400/e2e8f0/64748b?text=Exterior+Diurno" alt="Imagem de portfólio de exterior" class="w-full h-auto rounded-lg shadow-md transition-transform duration-300 hover:scale-105">
                    <img src="https://placehold.co/600x400/dbeafe/1e40af?text=Imagem+Editada" alt="Imagem de portfólio de crepúsculo" class="w-full h-auto rounded-lg shadow-md transition-transform duration-300 hover:scale-105">
                </div>
            </div>

            <!-- Slide 7: Drone Video Portfolio (formerly Slide 6) -->
            <div id="slide-7" class="slide w-full flex-shrink-0 flex flex-col items-center p-8 md:p-16 overflow-y-auto">
                <h2 class="text-3xl md:text-4xl font-bold text-white mb-4 text-center">Portfólio de Vídeo com Drone</h2>
                <div class="video-placeholder w-full max-w-4xl rounded-2xl overflow-hidden shadow-2xl">
                    <div class="video-placeholder-icon">
                        <i class="fas fa-play"></i>
                    </div>
                </div>
                <p class="mt-4 text-center text-gray-400 text-sm">
                    Este é um espaço reservado. Aqui poderia incorporar o seu vídeo com drone de 60-90 segundos.
                </p>
            </div>

            <!-- Slide 8: Before & After (formerly Slide 7) -->
            <div id="slide-8" class="slide w-full flex-shrink-0 flex flex-col items-center justify-center p-8 md:p-16">
                <h2 class="text-3xl md:text-4xl font-bold text-white mb-8 text-center">Antes & Depois</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8 w-full max-w-4xl">
                    <div class="flex flex-col items-center">
                        <h3 class="text-xl font-semibold text-gray-300 mb-4">Antes</h3>
                        <img src="https://i.imgur.com/q9BkBEm.jpeg" alt="Imagem original antes da edição" class="w-full h-auto rounded-lg shadow-md">
                    </div>
                    <div class="flex flex-col items-center">
                        <h3 class="text-xl font-semibold text-gray-300 mb-4">Depois</h3>
                        <img src="https://i.imgur.com/qm6Vg9H.jpeg" alt="Imagem editada após o pós-processamento" class="w-full h-auto rounded-lg shadow-md">
                    </div>
                </div>
            </div>

            <!-- Slide 9: Pricing & Packages (formerly Slide 8) -->
            <div id="slide-9" class="slide w-full flex-shrink-0 flex flex-col items-center p-8 md:p-16 overflow-y-auto">
                <h2 class="text-3xl md:text-4xl font-bold text-white mb-8 text-center">Preços & Pacotes</h2>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-6 w-full max-w-5xl">
                    <!-- Package 1 -->
                    <div class="bg-gray-800 p-6 rounded-2xl shadow-lg border border-gray-700 text-center">
                        <h3 class="text-2xl font-bold text-gray-200 mb-2">Pacote Inicial</h3>
                        <p class="text-4xl font-extrabold text-white mb-4">$350</p>
                        <ul class="text-left text-gray-300 space-y-2 mb-6">
                            <li class="flex items-center"><i class="fas fa-check-circle text-green-500 mr-2"></i> Fotografia Profissional</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-green-500 mr-2"></i> 25 Imagens Editadas</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-green-500 mr-2"></i> Galeria Online</li>
                        </ul>
                        <button class="w-full bg-green-700 text-white font-semibold py-3 px-6 rounded-full hover:bg-green-800 transition-colors duration-300">
                            Saber Mais
                        </button>
                    </div>
                    <!-- Package 2 -->
                    <div class="bg-gray-700 p-6 rounded-2xl shadow-lg border-2 border-gray-600 text-center scale-105">
                        <h3 class="text-2xl font-bold text-gray-200 mb-2">Pacote Premium</h3>
                        <p class="text-4xl font-extrabold text-white mb-4">$600</p>
                        <ul class="text-left text-gray-300 space-y-2 mb-6">
                            <li class="flex items-center"><i class="fas fa-check-circle text-green-500 mr-2"></i> Todos os itens do Pacote Inicial</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-green-500 mr-2"></i> 45 Imagens Editadas</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-green-500 mr-2"></i> Imagens Aéreas com Drone</li>
                        </ul>
                        <button class="w-full bg-green-700 text-white font-semibold py-3 px-6 rounded-full hover:bg-green-800 transition-colors duration-300">
                            Saber Mais
                        </button>
                    </div>
                    <!-- Package 3 -->
                    <div class="bg-gray-800 p-6 rounded-2xl shadow-lg border border-gray-700 text-center">
                        <h3 class="text-2xl font-bold text-gray-200 mb-2">À La Carte</h3>
                        <p class="text-4xl font-extrabold text-white mb-4">Personalizado</p>
                        <ul class="text-left text-gray-300 space-y-2 mb-6">
                            <li class="flex items-center"><i class="fas fa-check-circle text-green-500 mr-2"></i> Fotografia ao Crepúsculo</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-green-500 mr-2"></i> Tour Virtual 3D</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-green-500 mr-2"></i> Orçamento Personalizado</li>
                        </ul>
                        <button class="w-full bg-green-700 text-white font-semibold py-3 px-6 rounded-full hover:bg-green-800 transition-colors duration-300">
                            Contacte-nos
                        </button>
                    </div>
                </div>
            </div>

            <!-- Slide 10: Contact Information (formerly Slide 9) -->
            <div id="slide-10" class="slide w-full flex-shrink-0 flex flex-col items-center justify-center p-8 md:p-16">
                <h2 class="text-3xl md:text-4xl font-bold text-white mb-8 text-center">Entre em contacto!</h2>
                <div class="bg-gray-800 p-8 rounded-2xl shadow-xl max-w-md w-full text-center">
                    <p class="text-gray-300 mb-4 font-semibold text-lg">Luís Cutileiro Santos</p>
                    <p class="text-400 mb-2 text-white"><i class="fas fa-phone mr-2 text-green-400"></i> +351 910 599 626</p>
                    <p class="text-400 mb-2 text-white"><i class="fas fa-phone mr-2 text-green-400"></i> +44 (0)7453015680</p>
                    <p class="text-400 mb-2 text-white"><i class="fas fa-envelope mr-2 text-green-400"></i> luis.cutileiro.santos@gmail.com</p>
                    <div class="flex justify-center mt-4 space-x-4">
                        <a href="https://www.instagram.com/the_londroner" class="text-gray-400 hover:text-green-500 transition-colors duration-200"><i class="fab fa-instagram text-2xl"></i></a>
                        <a href="https://www.linkedin.com/in/luiscutileirosantos/" class="text-gray-400 hover:text-green-500 transition-colors duration-200"><i class="fab fa-linkedin text-2xl"></i></a>
                    </div>
                </div>
            </div>
            
        </div>

        <!-- Navigation Buttons -->
        <div class="absolute bottom-4 left-0 right-0 flex justify-center space-x-4">
            <button id="prev-btn" class="bg-white text-gray-800 py-2 px-6 rounded-full shadow-lg hover:bg-gray-200 transition-colors duration-300">
                <i class="fas fa-arrow-left mr-2"></i> Anterior
            </button>
            <button id="next-btn" class="bg-white text-gray-800 py-2 px-6 rounded-full shadow-lg hover:bg-gray-200 transition-colors duration-300">
                Próximo <i class="fas fa-arrow-right ml-2"></i>
            </button>
        </div>
    </div>

    <!-- JavaScript for Slideshow Logic -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const slides = document.querySelectorAll('.slide');
            const nextBtn = document.getElementById('next-btn');
            const prevBtn = document.getElementById('prev-btn');
            let currentSlideIndex = 0;

            /**
             * Updates the visibility of the slides to show only the active one.
             * @param {number} index The index of the slide to display.
             */
            const showSlide = (index) => {
                slides.forEach((slide) => {
                    slide.classList.remove('active');
                    slide.style.display = 'none'; // Ensure it's hidden for screen readers
                });
                slides[index].classList.add('active');
                slides[index].style.display = 'flex'; // Display the active slide
            };

            /**
             * Advances to the next slide, looping back to the beginning if at the end.
             */
            const nextSlide = () => {
                currentSlideIndex = (currentSlideIndex + 1) % slides.length;
                showSlide(currentSlideIndex);
            };

            /**
             * Goes back to the previous slide, looping to the end if at the beginning.
             */
            const prevSlide = () => {
                currentSlideIndex = (currentSlideIndex - 1 + slides.length) % slides.length;
                showSlide(currentSlideIndex);
            };

            // Add event listeners for the navigation buttons
            nextBtn.addEventListener('click', nextSlide);
            prevBtn.addEventListener('click', prevSlide);

            // Initialize the slideshow
            showSlide(currentSlideIndex);
        });
    </script>
</body>
</html>

