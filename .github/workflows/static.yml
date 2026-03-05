<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Você</title>

    <!-- Configurações para o Ícone no WhatsApp (Open Graph) -->
    <!-- Substitua o conteúdo de 'content' pelas informações que desejar -->
    <meta property="og:title" content="Uma surpresa para você...">
    <meta property="og:description" content="Algo que eu não podia dizer em público. Abra quando estiver sozinha.">
    <!-- Substitua o link abaixo por uma URL de imagem real (JPG ou PNG) hospedada na internet -->
    <meta property="og:image" content="https://images.unsplash.com/photo-1516589174184-c685266e4873?q=80&w=500&auto=format&fit=crop">
    <meta property="og:type" content="website">

    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Poppins:wght@300;400;600&display=swap');

        body {
            background-color: #0a0a0a;
            color: #e5e5e5;
            font-family: 'Poppins', sans-serif;
            overflow: hidden;
            margin: 0;
        }

        .font-serif {
            font-family: 'Playfair Display', serif;
        }

        .slide {
            display: none;
            height: 100vh;
            width: 100vw;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            padding: 2rem;
            text-align: center;
            position: absolute;
            top: 0;
            left: 0;
            background: radial-gradient(circle at center, #1a0505 0%, #0a0a0a 100%);
        }

        .slide.active {
            display: flex;
            animation: fadeIn 1.5s ease-out forwards;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); filter: blur(5px); }
            to { opacity: 1; transform: translateY(0); filter: blur(0); }
        }

        .text-glow {
            text-shadow: 0 0 15px rgba(220, 38, 38, 0.5);
        }

        .btn-next {
            border: 1px solid rgba(220, 38, 38, 0.3);
            background: rgba(220, 38, 38, 0.1);
            backdrop-filter: blur(5px);
            transition: all 0.3s ease;
        }

        .btn-next:hover {
            background: rgba(220, 38, 38, 0.3);
            box-shadow: 0 0 20px rgba(220, 38, 38, 0.4);
        }

        .floating-heart {
            position: absolute;
            color: rgba(220, 38, 38, 0.2);
            pointer-events: none;
            z-index: 0;
            animation: float 6s infinite ease-in-out;
        }

        @keyframes float {
            0% { transform: translateY(0) rotate(0deg); opacity: 0; }
            50% { opacity: 0.5; }
            100% { transform: translateY(-100vh) rotate(360deg); opacity: 0; }
        }

        .overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(0deg, rgba(0,0,0,0.8) 0%, rgba(0,0,0,0) 50%, rgba(0,0,0,0.8) 100%);
            pointer-events: none;
            z-index: 10;
        }
    </style>
</head>
<body>

    <div class="overlay"></div>
    <div id="particles-container"></div>

    <!-- Slides -->
    <div class="slide active" id="slide-1">
        <h2 class="text-sm uppercase tracking-[0.3em] text-red-600 mb-4 font-semibold">Só para os seus olhos</h2>
        <h1 class="text-4xl md:text-6xl font-serif italic text-glow">Algumas coisas não podem ser ditas em público...</h1>
        <p class="mt-8 text-gray-400 max-w-md">Feche a porta, relaxe e clique abaixo quando estiver pronta.</p>
        <button onclick="nextSlide(1)" class="btn-next mt-10 px-8 py-3 rounded-full text-white uppercase tracking-widest text-xs">Entrar no meu mundo</button>
    </div>

    <div class="slide" id="slide-2">
        <h1 class="text-3xl md:text-5xl font-serif leading-tight max-w-2xl">O jeito que você move os lábios quando fala... tira meu foco, mas desperta meus <span class="text-red-500 italic">piores instintos</span>.</h1>
        <button onclick="nextSlide(2)" class="btn-next mt-12 px-8 py-3 rounded-full text-white uppercase tracking-widest text-xs">Continue...</button>
    </div>

    <div class="slide" id="slide-3">
        <h1 class="text-3xl md:text-5xl font-serif leading-tight max-w-2xl">Eu passo o dia imaginando minhas mãos percorrendo curvas que as roupas insistem em esconder.</h1>
        <p class="mt-6 text-red-400 italic font-serif text-xl">"A paciência é uma virtude que eu perco sempre que te vejo."</p>
        <button onclick="nextSlide(3)" class="btn-next mt-12 px-8 py-3 rounded-full text-white uppercase tracking-widest text-xs">E depois?</button>
    </div>

    <div class="slide" id="slide-4">
        <h1 class="text-3xl md:text-5xl font-serif leading-tight max-w-2xl">Quero sentir o calor da sua pele contra a minha até que não saibamos onde um termina e o outro começa.</h1>
        <p class="mt-6 text-gray-400">Sem pressa, sem limites, apenas o som da nossa respiração ficando curta.</p>
        <button onclick="nextSlide(4)" class="btn-next mt-12 px-8 py-3 rounded-full text-white uppercase tracking-widest text-xs">O que você quer de mim?</button>
    </div>

    <div class="slide" id="slide-5">
        <h1 class="text-4xl md:text-6xl font-serif text-red-600 italic mb-6">Eu quero tudo.</h1>
        <p class="text-xl max-w-xl leading-relaxed text-gray-200">
            Quero seus sussurros no meu ouvido, seus arrepios sob meu toque e aquele olhar que você só faz quando está perdendo o controle.
        </p>
        <button onclick="nextSlide(5)" class="btn-next mt-12 px-8 py-3 rounded-full text-white uppercase tracking-widest text-xs">Como termina?</button>
    </div>

    <div class="slide" id="slide-6">
        <h1 class="text-3xl md:text-5xl font-serif mb-8">Não termina. <br>Apenas começa.</h1>
        <p class="text-gray-400 mb-10">Estou contando os segundos para transformar essas palavras em toques.</p>
        <div class="flex flex-col gap-4">
            <!-- Link atualizado com o seu número -->
            <a href="https://wa.me/5541987995285?text=Acabei%20de%20ver%20a%20sua%20surpresa...%20e%20agora%20quem%20está%20sem%20ar%20sou%20eu." target="_blank" id="messageLink" class="btn-next px-10 py-4 rounded-lg bg-red-700 text-white font-bold text-center">Me diga o que sentiu</a>
            <button onclick="restart()" class="text-xs text-gray-500 hover:text-red-400 transition">Ver novamente</button>
        </div>
    </div>

    <script>
        function nextSlide(current) {
            const currentSlide = document.getElementById(`slide-${current}`);
            const nextSlide = document.getElementById(`slide-${current + 1}`);
            
            if (nextSlide) {
                currentSlide.classList.remove('active');
                setTimeout(() => {
                    nextSlide.classList.add('active');
                }, 50);
            }
        }

        function restart() {
            document.querySelectorAll('.slide').forEach(s => s.classList.remove('active'));
            document.getElementById('slide-1').classList.add('active');
        }

        function createParticles() {
            const container = document.getElementById('particles-container');
            const icons = ['❤', '✧', '◈', '❤'];
            
            setInterval(() => {
                const p = document.createElement('div');
                p.className = 'floating-heart';
                p.innerText = icons[Math.floor(Math.random() * icons.length)];
                p.style.left = Math.random() * 100 + 'vw';
                p.style.fontSize = (Math.random() * 20 + 10) + 'px';
                p.style.animationDuration = (Math.random() * 5 + 5) + 's';
                container.appendChild(p);

                setTimeout(() => {
                    p.remove();
                }, 10000);
            }, 800);
        }

        window.onload = createParticles;
    </script>
</body>
</html>
