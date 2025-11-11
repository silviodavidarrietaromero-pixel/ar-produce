<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AR PRODUCE | De la Idea a la Plataforma</title>
    <!-- Load Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Configure Tailwind to use Inter font and define custom colors -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        'studio-dark': '#111827', // Almost black
                        'studio-accent': '#3b82f6', // Bright blue
                        'studio-light': '#f3f4f6', // Light gray
                    }
                }
            }
        }
    </script>
    <!-- Load Lucide icons for visual elements -->
    <script src="https://unpkg.com/lucide@latest/dist/umd/lucide.js"></script>
    <style>
        /* Custom scrollbar style for dark theme */
        body {
            background-color: #111827;
        }
        /* Custom styles for mobile responsiveness and feel */
        .container-padding {
            padding-left: 1rem;
            padding-right: 1rem;
        }
        @media (min-width: 640px) {
            .container-padding {
                padding-left: 2rem;
                padding-right: 2rem;
            }
        }
    </style>
</head>
<body class="font-sans bg-studio-dark text-studio-light antialiased">

    <!-- Header & Navigation -->
    <header class="sticky top-0 z-50 bg-studio-dark/95 backdrop-blur-sm border-b border-gray-700 shadow-lg">
        <div class="max-w-7xl mx-auto flex justify-between items-center py-4 container-padding">
            <!-- Logo/Name -->
            <a href="#inicio" class="text-3xl font-extrabold text-studio-accent tracking-tighter hover:text-studio-light transition duration-300">
                AR PRODUCE
            </a>
            <!-- Desktop Navigation (Hidden on mobile) -->
            <nav class="hidden sm:flex space-x-6 text-gray-300">
                <a href="#inicio" class="hover:text-studio-accent transition duration-200">Inicio</a>
                <a href="#mision" class="hover:text-studio-accent transition duration-200">Misión</a>
                <a href="#servicios" class="hover:text-studio-accent transition duration-200">Servicios</a>
                <a href="#contacto" class="hover:text-studio-accent transition duration-200">Contacto</a>
            </nav>
            <!-- CTA Button for Mobile/Desktop -->
            <a href="#contacto" class="sm:inline-flex bg-studio-accent hover:bg-blue-600 text-white font-bold py-2 px-4 rounded-full transition duration-300 transform hover:scale-105 shadow-lg hidden">
                ¡Graba tu 1er Hit!
            </a>
        </div>
    </header>

    <!-- Main Content -->
    <main>
        <!-- 1. Hero Section -->
        <section id="inicio" class="relative overflow-hidden pt-16 pb-20 sm:pt-24 sm:pb-32 container-padding">
            <div class="max-w-7xl mx-auto relative z-10">
                <div class="text-center">
                    <h1 class="text-4xl sm:text-6xl lg:text-7xl font-extrabold tracking-tight mb-4 leading-tight">
                        <span class="block text-white">De la Idea al Stream:</span>
                        <span class="block text-studio-accent mt-2">Tu Primer Hit.</span>
                    </h1>
                    <p class="mt-4 text-lg sm:text-xl text-gray-400 max-w-3xl mx-auto">
                        AR PRODUCE es el estudio y semillero creado para *jóvenes como tú*. Te damos el micrófono, el equipo profesional y la guía para que tu música deje de ser un demo y se convierta en una realidad en Spotify.
                    </p>
                    <div class="mt-10 flex flex-col sm:flex-row justify-center space-y-4 sm:space-y-0 sm:space-x-4">
                        <a href="#contacto" class="inline-flex items-center justify-center bg-studio-accent hover:bg-blue-600 text-white font-bold py-3 px-8 rounded-full shadow-xl transition duration-300 transform hover:scale-105 text-lg">
                            Reservar mi Primera Sesión
                            <i data-lucide="mic-2" class="w-5 h-5 ml-2"></i>
                        </a>
                        <a href="#servicios" class="inline-flex items-center justify-center bg-gray-700 hover:bg-gray-600 text-studio-light font-bold py-3 px-8 rounded-full shadow-lg transition duration-300 transform hover:scale-105 text-lg">
                            Ver Servicios
                        </a>
                    </div>
                </div>
            </div>
        </section>

        <!-- 2. Mission Section (Manifiesto) -->
        <section id="mision" class="py-20 sm:py-28 bg-gray-800/50 container-padding">
            <div class="max-w-7xl mx-auto">
                <h2 class="text-3xl sm:text-4xl font-bold text-center mb-12 text-white">
                    Nuestro Manifiesto: Impulsamos tu Talento
                </h2>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                    <!-- Value 1 -->
                    <div class="bg-gray-800 p-6 rounded-xl shadow-2xl transition duration-300 hover:shadow-studio-accent/20 hover:scale-[1.02] transform">
                        <i data-lucide="zap" class="w-8 h-8 text-studio-accent mb-4"></i>
                        <h3 class="text-xl font-semibold mb-3 text-white">
                            Energía Cero-Miedo
                        </h3>
                        <p class="text-gray-400">
                            Sabemos que es tu primera vez, y eso es genial. Olvídate de la presión; nuestro ambiente es creativo, relajado y libre de juicios para que experimentes sin límites.
                        </p>
                    </div>
                    <!-- Value 2 -->
                    <div class="bg-gray-800 p-6 rounded-xl shadow-2xl transition duration-300 hover:shadow-studio-accent/20 hover:scale-[1.02] transform">
                        <i data-lucide="trending-up" class="w-8 h-8 text-studio-accent mb-4"></i>
                        <h3 class="text-xl font-semibold mb-3 text-white">
                            Calidad Profesional
                        </h3>
                        <p class="text-gray-400">
                            Tu música merece un sonido competitivo. Usamos equipos de estudio de alta gama para asegurar que tu track tenga la claridad, potencia y mezcla necesaria para destacar.
                        </p>
                    </div>
                    <!-- Value 3 -->
                    <div class="bg-gray-800 p-6 rounded-xl shadow-2xl transition duration-300 hover:shadow-studio-accent/20 hover:scale-[1.02] transform">
                        <i data-lucide="compass" class="w-8 h-8 text-studio-accent mb-4"></i>
                        <h3 class="text-xl font-semibold mb-3 text-white">
                            Guía y Asesoría
                        </h3>
                        <p class="text-gray-400">
                            Te acompañamos en cada etapa: desde pulir la estructura de tu canción hasta entender cómo subirla a las plataformas de streaming. Eres el artista, nosotros el mapa.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- 3. Services Section -->
        <section id="servicios" class="py-20 sm:py-28 container-padding">
            <div class="max-w-7xl mx-auto">
                <h2 class="text-3xl sm:text-4xl font-bold text-center mb-16 text-white">
                    Servicios de Producción
                </h2>
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
                    <!-- Service Card 1: Grabación -->
                    <div class="bg-gray-700/30 p-8 rounded-2xl flex flex-col md:flex-row shadow-xl">
                        <div class="md:w-1/4 flex justify-center md:block mb-4 md:mb-0">
                            <i data-lucide="headphones" class="w-12 h-12 text-studio-accent"></i>
                        </div>
                        <div class="md:w-3/4">
                            <h3 class="text-2xl font-bold mb-2 text-white">
                                01. Grabación de Voces
                            </h3>
                            <p class="text-gray-300 mb-4">
                                Captura la esencia de tu performance. Nuestra cabina con tratamiento acústico y micrófonos de condensador de estudio aseguran que tu voz sea cristalina y potente. Ideal para MCs, cantantes y vocalistas.
                            </p>
                            <span class="text-sm font-semibold text-studio-accent border border-studio-accent px-3 py-1 rounded-full">Enfocado en el Artista</span>
                        </div>
                    </div>
                    <!-- Service Card 2: Producción -->
                    <div class="bg-gray-700/30 p-8 rounded-2xl flex flex-col md:flex-row shadow-xl">
                        <div class="md:w-1/4 flex justify-center md:block mb-4 md:mb-0">
                            <i data-lucide="sliders" class="w-12 h-12 text-studio-accent"></i>
                        </div>
                        <div class="md:w-3/4">
                            <h3 class="text-2xl font-bold mb-2 text-white">
                                02. Producción Musical
                            </h3>
                            <p class="text-gray-300 mb-4">
                                ¿Tienes solo la idea o una letra? Nosotros creamos o pulimos el beat, los arreglos y la estructura para que tu track pase de ser un concepto a una canción totalmente realizada.
                            </p>
                            <span class="text-sm font-semibold text-studio-accent border border-studio-accent px-3 py-1 rounded-full">Desarrollo de Beats</span>
                        </div>
                    </div>
                    <!-- Service Card 3: Mezcla & Mastering -->
                    <div class="bg-gray-700/30 p-8 rounded-2xl flex flex-col md:flex-row shadow-xl">
                        <div class="md:w-1/4 flex justify-center md:block mb-4 md:mb-0">
                            <i data-lucide="volume-2" class="w-12 h-12 text-studio-accent"></i>
                        </div>
                        <div class="md:w-3/4">
                            <h3 class="text-2xl font-bold mb-2 text-white">
                                03. Mezcla y Masterización
                            </h3>
                            <p class="text-gray-300 mb-4">
                                El paso final. Balanceamos todos los elementos de tu track (voces, instrumentos, efectos) y lo preparamos para que suene fuerte y claro en cualquier plataforma (Spotify, YouTube, Radio).
                            </p>
                            <span class="text-sm font-semibold text-studio-accent border border-studio-accent px-3 py-1 rounded-full">Estándar Industrial</span>
                        </div>
                    </div>
                     <!-- Service Card 4: Asesoría -->
                     <div class="bg-gray-700/30 p-8 rounded-2xl flex flex-col md:flex-row shadow-xl">
                        <div class="md:w-1/4 flex justify-center md:block mb-4 md:mb-0">
                            <i data-lucide="book-open-check" class="w-12 h-12 text-studio-accent"></i>
                        </div>
                        <div class="md:w-3/4">
                            <h3 class="text-2xl font-bold mb-2 text-white">
                                04. Asesoría de Carrera
                            </h3>
                            <p class="text-gray-300 mb-4">
                                Más allá del estudio: te orientamos en la distribución digital, derechos de autor básicos y estrategias de promoción para que sepas exactamente qué hacer con tu canción una vez que esté lista.
                            </p>
                            <span class="text-sm font-semibold text-studio-accent border border-studio-accent px-3 py-1 rounded-full">Ruta al Lanzamiento</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- 4. Testimonial / Mockup Portfolio (Proof of Concept) -->
        <section class="py-20 sm:py-28 bg-gray-900/80 container-padding">
            <div class="max-w-7xl mx-auto text-center">
                <h2 class="text-3xl sm:text-4xl font-bold mb-12 text-white">
                    Talento que ya está Sonando
                </h2>
                <blockquote class="max-w-3xl mx-auto bg-gray-800 p-8 rounded-xl shadow-2xl border-l-4 border-studio-accent">
                    <i data-lucide="quote" class="w-8 h-8 text-studio-accent mb-4 mx-auto"></i>
                    <p class="text-xl sm:text-2xl italic text-gray-300 mb-6">
                        "Grabar mi primera canción con AR PRODUCE fue increíble. Me explicaron cada paso y el resultado suena exactamente como lo imaginé. Ahora mi track está en todas las plataformas. ¡Son los mejores!"
                    </p>
                    <footer class="text-right">
                        <cite class="text-white font-semibold block not-italic">- LEO 'The Kid' V., Artista Urbano</cite>
                        <cite class="text-gray-500 text-sm not-italic">Primer Sencillo: "Fuego Lento"</cite>
                    </footer>
                </blockquote>
            </div>
        </section>
        
        <!-- 5. Contact & CTA Section -->
        <section id="contacto" class="py-20 sm:py-28 container-padding">
            <div class="max-w-3xl mx-auto text-center bg-gray-800 p-8 sm:p-12 rounded-2xl shadow-2xl border border-gray-700">
                <h2 class="text-3xl sm:text-4xl font-bold text-white mb-4">
                    ¿Listo para grabar tu himno?
                </h2>
                <p class="text-lg text-gray-400 mb-8">
                    El primer paso es el más importante. Reserva una *consulta gratuita* con nuestro productor para discutir tu proyecto, tus metas y cómo vamos a lograr ese sonido profesional.
                </p>
                <form id="contactForm" class="space-y-4">
                    <div>
                        <input type="text" id="name" placeholder="Tu Nombre" required class="w-full p-3 rounded-lg bg-gray-900 border border-gray-700 text-white placeholder-gray-500 focus:ring-studio-accent focus:border-studio-accent">
                    </div>
                    <div>
                        <input type="email" id="email" placeholder="Tu Email o WhatsApp" required class="w-full p-3 rounded-lg bg-gray-900 border border-gray-700 text-white placeholder-gray-500 focus:ring-studio-accent focus:border-studio-accent">
                    </div>
                    <div>
                        <select id="service" required class="w-full p-3 rounded-lg bg-gray-900 border border-gray-700 text-gray-400 focus:ring-studio-accent focus:border-studio-accent">
                            <option value="" disabled selected>Me interesa...</option>
                            <option value="grabacion">Grabación de una Canción</option>
                            <option value="produccion">Producción de un Beat/Pista</option>
                            <option value="mastering">Mezcla y Masterización</option>
                            <option value="asesoria">Asesoría de Proyecto</option>
                        </select>
                    </div>
                    <div>
                        <textarea id="message" rows="4" placeholder="Cuéntanos brevemente sobre tu proyecto o canción." required class="w-full p-3 rounded-lg bg-gray-900 border border-gray-700 text-white placeholder-gray-500 focus:ring-studio-accent focus:border-studio-accent"></textarea>
                    </div>
                    <button type="submit" class="w-full bg-studio-accent hover:bg-blue-600 text-white font-bold py-3 rounded-full transition duration-300 transform hover:scale-[1.01] shadow-xl text-lg">
                        Enviar Solicitud
                        <i data-lucide="send" class="w-5 h-5 ml-2 inline-block"></i>
                    </button>
                    <!-- Success/Error Message Box -->
                    <div id="statusMessage" class="mt-4 text-center p-3 rounded-lg hidden text-sm"></div>
                </form>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 border-t border-gray-800 mt-10">
        <div class="max-w-7xl mx-auto py-10 container-padding">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-center md:text-left">
                <!-- Col 1: Logo & Mission -->
                <div>
                    <h3 class="text-3xl font-extrabold text-studio-accent mb-3">AR PRODUCE</h3>
                    <p class="text-gray-500 text-sm">
                        Impulsando el futuro de la música. Tu primer hit, grabado profesionalmente.
                    </p>
                </div>
                <!-- Col 2: Quick Links -->
                <div>
                    <h4 class="text-lg font-semibold text-white mb-4">Enlaces Rápidos</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li><a href="#servicios" class="hover:text-studio-accent transition duration-200">Servicios</a></li>
                        <li><a href="#mision" class="hover:text-studio-accent transition duration-200">Manifiesto</a></li>
                        <li><a href="#contacto" class="hover:text-studio-accent transition duration-200">Reservar</a></li>
                    </ul>
                </div>
                <!-- Col 3: Contact Info -->
                <div>
                    <h4 class="text-lg font-semibold text-white mb-4">Contáctanos</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li class="flex items-center justify-center md:justify-start">
                            <i data-lucide="mail" class="w-4 h-4 mr-2 text-studio-accent"></i>
                            arproduce.ing@gmail.com
                        </li>
                        <li class="flex items-center justify-center md:justify-start">
                            <i data-lucide="phone" class="w-4 h-4 mr-2 text-studio-accent"></i>
                            +57 311 692 0781 (WhatsApp)
                        </li>
                        <li class="flex items-center justify-center md:justify-start">
                            <i data-lucide="map-pin" class="w-4 h-4 mr-2 text-studio-accent"></i>
                            [Ciudad, País]
                        </li>
                    </ul>
                </div>
            </div>
            <div class="text-center text-gray-600 text-sm mt-10 pt-6 border-t border-gray-800">
                &copy; 2025 AR PRODUCE. Todos los derechos reservados.
            </div>
        </div>
    </footer>

    <script>
        // Initialize Lucide icons
        lucide.createIcons();

        // Get the form and message box elements
        const contactForm = document.getElementById('contactForm');
        const statusMessage = document.getElementById('statusMessage');

        // Function to display a message
        function displayMessage(message, isSuccess) {
            statusMessage.textContent = message;
            statusMessage.classList.remove('hidden', 'bg-red-900/50', 'text-red-300', 'bg-green-900/50', 'text-green-300');
            if (isSuccess) {
                statusMessage.classList.add('bg-green-900/50', 'text-green-300');
            } else {
                statusMessage.classList.add('bg-red-900/50', 'text-red-300');
            }
        }

        // Handle form submission
        contactForm.addEventListener('submit', function(event) {
            event.preventDefault(); // Prevent default form submission

            // Simple data collection (in a real app, this would send data to a server)
            const name = document.getElementById('name').value;
            const service = document.getElementById('service').value;

            // Simulate a successful submission
            displayMessage(¡Gracias, ${name}! Tu solicitud para '${service}' ha sido recibida. Nos pondremos en contacto contigo muy pronto., true);

            // Clear the form after submission
            contactForm.reset();
        });

        // Function to handle smooth scrolling for navigation
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                // Only prevent default if the target section exists
                const targetId = this.getAttribute('href');
                if (targetId !== '#') {
                    e.preventDefault();
                    document.querySelector(targetId).scrollIntoView({
                        behavior: 'smooth'
                    });
                }
            });
        });

    </script>
</body>
</html>
