<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Чарівні Дзеркала - Преміальна Колекція</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@200;300;400;500;600;700&display=swap" rel="stylesheet">
    
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        gold: {
                            DEFAULT: '#D4AF37',
                            glow: 'rgba(212,175,55,0.4)',
                            light: '#F3E5AB'
                        },
                        black: '#000000',
                        white: '#ffffff'
                    },
                    fontFamily: {
                        sans:['Montserrat', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <link rel="stylesheet" href="style.css">
</head>
<body class="bg-white text-black antialiased overflow-x-hidden">

    <nav class="fixed top-0 w-full z-50 bg-white/80 backdrop-blur-md border-b border-gray-100 py-4 px-8 flex justify-between items-center transition-all duration-300 gsap-nav">
        <div class="text-2xl font-semibold tracking-wider text-black flex items-center gap-2">
            <i data-lucide="sparkles" class="text-gold"></i>
            MAGIC MIRRORS
        </div>
        <ul class="hidden md:flex gap-8 text-sm font-medium tracking-wide">
            <li><a href="#catalog" class="hover:text-gold transition-colors">Каталог</a></li>
            <li><a href="#benefits" class="hover:text-gold transition-colors">Переваги</a></li>
            <li><a href="#showroom" class="hover:text-gold transition-colors">Шоурум</a></li>
            <li><a href="#contact" class="hover:text-gold transition-colors">Контакти</a></li>
        </ul>
        <button class="bg-black text-white px-6 py-2 rounded-full text-sm font-medium hover:bg-gold transition-all duration-300 gold-glow-hover">
            Замовити
        </button>
    </nav>

    <header class="relative h-screen flex items-center justify-center overflow-hidden">
        <div class="absolute inset-0 z-0 parallax-bg">
            <div class="absolute inset-0 bg-black/30 z-10"></div>
            <img src="https://images.unsplash.com/photo-1618220179428-22790b46a0eb?q=80&w=2000&auto=format&fit=crop" alt="Interior with mirror" class="w-full h-[120%] object-cover object-center" />
        </div>
        <div class="relative z-10 text-center px-4 max-w-5xl mx-auto flex flex-col items-center">
            <h1 class="text-white text-5xl md:text-7xl lg:text-8xl font-light tracking-tight mb-6 gsap-hero-fade">
                Чарівні Дзеркала
            </h1>
            <p class="text-white/90 text-lg md:text-2xl font-light mb-10 max-w-2xl gsap-hero-fade delay-1">
                Ексклюзивна колекція преміальних дзеркал для створення довершеного простору
            </p>
            <div class="flex gap-4 gsap-hero-fade delay-2">
                <a href="#catalog" class="bg-gold text-white px-8 py-4 rounded-full text-lg font-medium tracking-wide gold-glow hover:bg-white hover:text-black transition-all duration-500">
                    Переглянути Колекцію
                </a>
            </div>
        </div>
    </header>

    <section id="catalog" class="py-32 px-4 md:px-8 max-w-7xl mx-auto">
        <div class="text-center mb-20 gsap-fade-up">
            <h2 class="text-4xl md:text-5xl font-light tracking-tight mb-4">Колекція Дзеркал</h2>
            <div class="w-24 h-1 bg-gold mx-auto rounded-full gold-glow"></div>
        </div>
        <div id="catalog-container" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-12">
        </div>
    </section>

    <section id="benefits" class="py-32 bg-gray-50 px-4 md:px-8">
        <div class="max-w-7xl mx-auto">
            <div class="text-center mb-20 gsap-fade-up">
                <h2 class="text-4xl md:text-5xl font-light tracking-tight mb-4">Чому обирають нас</h2>
                <div class="w-24 h-1 bg-gold mx-auto rounded-full gold-glow"></div>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-16 text-center">
                <div class="gsap-fade-up p-12 bg-white rounded-3xl shadow-sm hover:shadow-xl transition-shadow duration-500 border border-transparent hover:border-gold/30">
                    <div class="flex justify-center mb-6 text-gold">
                        <i data-lucide="award" class="w-16 h-16"></i>
                    </div>
                    <div class="text-6xl font-light text-gold mb-4 counter-target" data-target="25">0</div>
                    <p class="text-xl font-medium tracking-wide text-gray-800">років досвіду</p>
                    <p class="text-gray-500 mt-4 leading-relaxed">Створюємо шедеври, що витримують випробування часом та трендами.</p>
                </div>
                <div class="gsap-fade-up p-12 bg-white rounded-3xl shadow-sm hover:shadow-xl transition-shadow duration-500 border border-transparent hover:border-gold/30">
                    <div class="flex justify-center mb-6 text-gold">
                        <i data-lucide="heart" class="w-16 h-16"></i>
                    </div>
                    <div class="text-6xl font-light text-gold mb-4 flex justify-center items-center">
                        <span class="counter-target" data-target="100">0</span>%
                    </div>
                    <p class="text-xl font-medium tracking-wide text-gray-800">задоволених клієнтів</p>
                    <p class="text-gray-500 mt-4 leading-relaxed">Бездоганний сервіс та увага до кожної деталі вашого замовлення.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="showroom" class="py-32 px-4 md:px-8 max-w-7xl mx-auto">
        <div class="text-center mb-20 gsap-fade-up">
            <h2 class="text-4xl md:text-5xl font-light tracking-tight mb-4">Шоурум</h2>
            <div class="w-24 h-1 bg-gold mx-auto rounded-full gold-glow"></div>
            <p class="mt-6 text-gray-500 max-w-2xl mx-auto text-lg">Надихніться прикладами інтеграції наших дзеркал у сучасні інтер'єри.</p>
        </div>
        <div id="gallery-container" class="columns-1 md:columns-2 lg:columns-3 gap-6 space-y-6">
        </div>
    </section>

    <section id="contact" class="py-32 bg-black text-white px-4 md:px-8 relative overflow-hidden">
        <div class="absolute top-0 left-0 w-full h-full opacity-10 pointer-events-none">
            <div class="absolute -top-[20%] -left-[10%] w-[50%] h-[50%] bg-gold rounded-full blur-[120px]"></div>
            <div class="absolute bottom-[10%] right-[5%] w-[40%] h-[40%] bg-gold rounded-full blur-[100px]"></div>
        </div>
        <div class="max-w-7xl mx-auto relative z-10">
            <div class="text-center mb-20 gsap-fade-up">
                <h2 class="text-4xl md:text-5xl font-light tracking-tight mb-4">Зв’яжіться з нами</h2>
                <div class="w-24 h-1 bg-gold mx-auto rounded-full gold-glow"></div>
            </div>
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-16">
                <div class="gsap-fade-up bg-white/5 backdrop-blur-lg p-10 rounded-3xl border border-white/10">
                    <form id="contact-form" class="flex flex-col gap-6">
                        <div class="relative">
                            <input type="text" id="name" class="w-full bg-transparent border-b border-white/30 py-4 px-2 text-white placeholder-transparent peer focus:outline-none focus:border-gold transition-colors duration-300" placeholder="Ім'я">
                            <label for="name" class="absolute left-2 -top-2.5 text-xs text-gold/80 transition-all peer-placeholder-shown:text-base peer-placeholder-shown:text-white/50 peer-placeholder-shown:top-4 peer-focus:-top-2.5 peer-focus:text-xs peer-focus:text-gold">Ваше ім'я</label>
                        </div>
                        <div class="relative">
                            <input type="tel" id="phone" class="w-full bg-transparent border-b border-white/30 py-4 px-2 text-white placeholder-transparent peer focus:outline-none focus:border-gold transition-colors duration-300" placeholder="Телефон">
                            <label for="phone" class="absolute left-2 -top-2.5 text-xs text-gold/80 transition-all peer-placeholder-shown:text-base peer-placeholder-shown:text-white/50 peer-placeholder-shown:top-4 peer-focus:-top-2.5 peer-focus:text-xs peer-focus:text-gold">Номер телефону</label>
                        </div>
                        <div class="relative mb-6">
                            <textarea id="message" rows="4" class="w-full bg-transparent border-b border-white/30 py-4 px-2 text-white placeholder-transparent peer focus:outline-none focus:border-gold transition-colors duration-300 resize-none" placeholder="Повідомлення"></textarea>
                            <label for="message" class="absolute left-2 -top-2.5 text-xs text-gold/80 transition-all peer-placeholder-shown:text-base peer-placeholder-shown:text-white/50 peer-placeholder-shown:top-4 peer-focus:-top-2.5 peer-focus:text-xs peer-focus:text-gold">Ваше повідомлення</label>
                        </div>
                        <button type="submit" class="bg-transparent border border-gold text-gold py-4 rounded-full font-medium tracking-wide hover:bg-gold hover:text-white transition-all duration-500 gold-glow-hover flex justify-center items-center gap-2">
                            <span>Надіслати запит</span>
                            <i data-lucide="arrow-right" class="w-5 h-5"></i>
                        </button>
                    </form>
                </div>
                <div class="gsap-fade-up h-[500px] rounded-3xl overflow-hidden shadow-2xl relative group">
                    <div class="absolute inset-0 border-2 border-transparent group-hover:border-gold/50 transition-colors duration-500 rounded-3xl z-10 pointer-events-none"></div>
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2540.5064509172427!2d30.5234!3d50.4501!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zNTDCsDI3JzAwLjQiTiAzMMKwMzEnMjQuMiJF!5e0!3m2!1sen!2sua!4v1620000000000!5m2!1sen!2sua" width="100%" height="100%" style="border:0; filter: grayscale(100%) invert(90%) contrast(1.2);" allowfullscreen="" loading="lazy"></iframe>
                </div>
            </div>
        </div>
    </section>

    <footer class="bg-black py-12 border-t border-white/10 text-center text-white/50 text-sm">
        <div class="flex justify-center items-center gap-2 mb-4">
            <i data-lucide="sparkles" class="w-4 h-4 text-gold"></i>
            <span class="text-white tracking-widest font-medium">MAGIC MIRRORS</span>
        </div>
        <p>&copy; 2026 Чарівні Дзеркала. Всі права захищені.</p>
    </footer>

    <div id="lightbox" class="fixed inset-0 z-[100] bg-black/95 backdrop-blur-xl hidden opacity-0 flex items-center justify-center p-4 transition-opacity duration-500">
        <button id="lightbox-close" class="absolute top-8 right-8 text-white/50 hover:text-gold transition-colors p-2">
            <i data-lucide="x" class="w-10 h-10"></i>
        </button>
        <img id="lightbox-img" src="" alt="Zoomed view" class="max-w-full max-h-[90vh] object-contain rounded-lg shadow-2xl scale-95 transition-transform duration-500">
    </div>

    <script src="https://unpkg.com/@studio-freight/lenis@1.0.33/dist/lenis.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/ScrollTrigger.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/vanilla-tilt/1.8.1/vanilla-tilt.min.js"></script>
    <script src="https://unpkg.com/lucide@latest"></script>
    <script type="module" src="data.js"></script>
    <script type="module" src="app.js"></script>
</body>
</html>

