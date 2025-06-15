<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Minha Namorada</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://www.youtube.com/iframe_api"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;700&family=Poppins:wght@300;400;600&display=swap');
        
        .font-dancing {
            font-family: 'Dancing Script', cursive;
        }
        
        .font-poppins {
            font-family: 'Poppins', sans-serif;
        }
        
        .heart {
            position: absolute;
            pointer-events: none;
            animation: float 4s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% {
                transform: translateY(0) rotate(0deg);
                opacity: 1;
            }
            50% {
                transform: translateY(-20px) rotate(10deg);
                opacity: 0.8;
            }
        }
        
        .photo-gallery img {
            transition: all 0.3s ease;
        }
        
        .photo-gallery img:hover {
            transform: scale(1.05);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        
        .love-letter {
            background: url('https://images.unsplash.com/photo-1518199266791-5375a83190b7?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80') center/cover;
            position: relative;
        }
        
        .love-letter::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(255, 255, 255, 0.85);
        }
    </style>
</head>
<body class="bg-pink-50 font-poppins">
    <div id="hearts-container"></div>
    <iframe id="bg-music" width="0" height="0" src="https://www.youtube.com/embed/rtOvBOTyX00?autoplay=0&enablejsapi=1&loop=1" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    
    <header class="bg-gradient-to-r from-pink-500 to-red-400 text-white py-8 px-4 text-center shadow-lg">
        <h1 class="text-4xl md:text-6xl font-bold font-dancing mb-4">Para Minha Namorada</h1>
        <p class="text-xl md:text-2xl font-dancing">O amor da minha vida ( Danyelly )</p>
        <div class="mt-6">
            <button onclick="playMusic()" class="bg-white text-pink-600 px-6 py-2 rounded-full font-semibold hover:bg-pink-100 transition">
                <i class="fas fa-music mr-2"></i> Play Music
            </button>
        </div>
    </header>
    
    <section class="love-letter py-16 px-4 md:px-8 my-8 rounded-lg shadow-inner relative overflow-hidden">
        <div class="max-w-4xl mx-auto relative z-10">
            <h2 class="text-3xl md:text-4xl font-bold text-center font-dancing text-pink-700 mb-8">Minha Querida...</h2>
            <div class="bg-white bg-opacity-90 p-8 rounded-lg shadow-md">
                <p class="text-lg md:text-xl mb-4 text-gray-800">Desde o momento em que te conheci, minha vida ganhou novas cores...</p>
                <p class="text-lg md:text-xl mb-4 text-gray-800">Seu sorriso ilumina meus dias mais cinzentos...</p>
                <p class="text-lg md:text-xl mb-4 text-gray-800">Este site é apenas uma pequena demonstração do que sinto por você...</p>
                <p class="text-2xl font-dancing text-center text-pink-600 mt-8">Eu te amo mais do que palavras podem expressar.</p>
            </div>
        </div>
    </section>
    
    <section class="py-12 px-4 md:px-8">
        <h2 class="text-3xl font-bold text-center font-dancing text-pink-700 mb-12">Poema para Você</h2>
        <div class="max-w-2xl mx-auto bg-white p-8 rounded-xl shadow-lg">
            <div class="font-dancing text-xl text-gray-800 space-y-6">
                <p>Nos teus olhos encontro o meu refúgio,</p>
                <p>No teu sorriso, a luz que me guia,</p>
                <p>Nos teus braços, meu porto seguro,</p>
                <p>Na tua voz, a melodia do dia.</p>
                <p class="mt-8 text-pink-600 text-2xl text-center">E assim, meu amor, eu te dedico</p>
                <p class="text-pink-600 text-2xl text-center">Cada verso que nasce do coração,</p>
                <p class="text-pink-600 text-2xl text-center">Pois és tu a minha poesia,</p>
                <p class="text-pink-600 text-2xl text-center">Eterna, pura, sem fim nem razão.</p>
            </div>
        </div>
    </section>
    
    <section class="bg-gradient-to-r from-red-400 to-pink-500 text-white py-12 px-4 text-center my-8 rounded-lg shadow-lg">
        <h2 class="text-3xl font-bold font-dancing mb-6">Tempo Juntos</h2>
        <div class="grid grid-cols-3 gap-4 max-w-2xl mx-auto">
            <div class="bg-white bg-opacity-20 p-4 rounded-lg">
                <div id="years" class="text-4xl font-bold">3</div>
                <div>Anos</div>
            </div>
            <div class="bg-white bg-opacity-20 p-4 rounded-lg">
                <div id="months" class="text-4xl font-bold">6</div>
                <div>Meses</div>
            </div>
            <div class="bg-white bg-opacity-20 p-4 rounded-lg">
                <div id="days" class="text-4xl font-bold">22</div>
                <div>Dias</div>
            </div>
        </div>
    </section>
    
    <section class="py-12 px-4 text-center">
        <button onclick="revealMessage()" class="bg-pink-600 text-white px-6 py-3 rounded-full font-semibold hover:bg-pink-700 transition">
            Clique para uma mensagem secreta
        </button>
        <div id="secret-message" class="mt-8 hidden max-w-2xl mx-auto bg-pink-100 p-6 rounded-lg shadow-md">
            <h3 class="text-2xl font-dancing text-pink-700 mb-4">Surpresa!</h3>
            <p class="text-lg">Eu te amo mais do que tudo neste mundo. Você é a razão do meu sorriso todos os dias.</p>
            <p class="text-lg mt-4">- Wallacy seu namorado que te ama muito ❤️</p>
        </div>
    </section>
    
    <script>
        function revealMessage() {
            const message = document.getElementById('secret-message');
            message.classList.toggle('hidden');
        }

        function playMusic() {
            const player = document.getElementById('bg-music').contentWindow;
            const buttonIcon = document.querySelector('button i');
            
            if (buttonIcon.classList.contains('fa-music')) {
                player.postMessage('{"event":"command","func":"playVideo","args":""}', '*');
                buttonIcon.className = 'fas fa-pause mr-2';
            } else {
                player.postMessage('{"event":"command","func":"pauseVideo","args":""}', '*');
                buttonIcon.className = 'fas fa-music mr-2';
            }
        }
        
        // Create floating hearts
        function createHearts() {
            const container = document.getElementById('hearts-container');
            const heart = document.createElement('div');
            heart.innerHTML = '❤️';
            heart.className = 'heart';
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDuration = Math.random() * 3 + 2 + 's';
            heart.style.fontSize = Math.random() * 20 + 10 + 'px';
            container.appendChild(heart);
            
            setTimeout(() => {
                heart.remove();
            }, 5000);
        }
        
        setInterval(createHearts, 300);
    </script>
    
    <footer class="bg-pink-800 text-white py-8 px-4 text-center">
        <p class="text-xl font-dancing mb-4">Para sempre seu</p>
        <div class="flex justify-center space-x-4 text-2xl">
            <a href="#" class="hover:text-pink-300 transition"><i class="fab fa-instagram"></i></a>
            <a href="#" class="hover:text-pink-300 transition"><i
