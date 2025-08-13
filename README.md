<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>La Casa de las Togas CA - E-commerce de Servicios de Graduación</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.4.0/css/all.min.css">
    <link href="https://cdn.jsdelivr.net/npm/@n8n/chat/dist/style.css" rel="stylesheet" />
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
        }
        
        .gradient-bg {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        
        .card-hover {
            transition: all 0.3s ease;
        }
        
        .card-hover:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }
        
        .instagram-embed {
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 8px 32px rgba(0,0,0,0.1);
        }
        
        .service-card {
            background: linear-gradient(145deg, #ffffff, #f0f0f0);
            border: 1px solid #e2e8f0;
        }
        
        .whatsapp-float {
            position: fixed;
            width: 60px;
            height: 60px;
            bottom: 40px;
            right: 40px;
            background-color: #25d366;
            color: #FFF;
            border-radius: 50px;
            text-align: center;
            font-size: 30px;
            box-shadow: 2px 2px 3px #999;
            z-index: 100;
            display: flex;
            align-items: center;
            justify-content: center;
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% {
                box-shadow: 0 0 0 0 rgba(37, 211, 102, 0.7);
            }
            70% {
                box-shadow: 0 0 0 10px rgba(37, 211, 102, 0);
            }
            100% {
                box-shadow: 0 0 0 0 rgba(37, 211, 102, 0);
            }
        }
        
        .hero-pattern {
            background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 1000'%3E%3Cg %3E%3Ccircle fill='%23667eea' cx='50' cy='0' r='50'/%3E%3Cg fill='%236b73e6' %3E%3Ccircle cx='0' cy='50' r='50'/%3E%3Ccircle cx='100' cy='50' r='50'/%3E%3C/g%3E%3Ccircle fill='%237068e2' cx='50' cy='100' r='50'/%3E%3C/g%3E%3C/svg%3E");
            background-size: 100px 200px;
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- WhatsApp Float Button -->
    <a href="https://wa.me/584147622212" target="_blank" class="whatsapp-float">
        <i class="fab fa-whatsapp"></i>
    </a>

    <!-- Header -->
    <header class="bg-white shadow-lg fixed w-full top-0 z-50">
        <nav class="container mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <div class="flex items-center">
                    <i class="fas fa-graduation-cap text-3xl text-purple-600 mr-3"></i>
                    <h1 class="text-2xl font-bold text-gray-800">La Casa de las Togas CA</h1>
                </div>
                <div class="hidden md:flex space-x-6">
                    <a href="#inicio" class="text-gray-700 hover:text-purple-600 transition">Inicio</a>
                    <a href="#servicios" class="text-gray-700 hover:text-purple-600 transition">Servicios</a>
                    <a href="#galeria" class="text-gray-700 hover:text-purple-600 transition">Galería</a>
                    <a href="#contacto" class="text-gray-700 hover:text-purple-600 transition">Contacto</a>
                </div>
                <div class="md:hidden">
                    <button class="text-gray-700 focus:outline-none">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="inicio" class="gradient-bg hero-pattern text-white py-32 mt-16">
        <div class="container mx-auto px-6 text-center">
            <h2 class="text-5xl font-bold mb-6">Especialistas en Graduaciones</h2>
            <p class="text-xl mb-8 max-w-3xl mx-auto">Convertimos tus momentos especiales en recuerdos inolvidables. Servicios integrales de graduación, diseño gráfico, productos personalizados y mucho más.</p>
            <div class="flex flex-wrap justify-center gap-4">
                <a href="#servicios" class="bg-white text-purple-600 px-8 py-3 rounded-full font-semibold hover:bg-gray-100 transition">
                    Ver Servicios
                </a>
                <a href="https://wa.me/584147622212" class="bg-green-500 text-white px-8 py-3 rounded-full font-semibold hover:bg-green-600 transition">
                    <i class="fab fa-whatsapp mr-2"></i>Cotizar Ahora
                </a>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="servicios" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h3 class="text-4xl font-bold text-gray-800 mb-4">Nuestros Servicios</h3>
                <p class="text-gray-600 max-w-2xl mx-auto">Ofrecemos una amplia gama de servicios y productos personalizados para hacer de tu graduación un momento único e inolvidable.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6">
                <!-- Service Cards -->
                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-graduation-cap text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Paquetes de Grados</h4>
                        <p class="text-gray-600 text-sm">Paquetes completos para tu ceremonia de graduación</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-palette text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Diseño Gráfico</h4>
                        <p class="text-gray-600 text-sm">Diseños profesionales para tu marca y eventos</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-medal text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Medallas Personalizadas</h4>
                        <p class="text-gray-600 text-sm">Medallas con diseño único y carácter especial</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-ring text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Anillos de Graduación</h4>
                        <p class="text-gray-600 text-sm">Anillos únicos para celebrar tu logro</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-laser text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Grabados Láser</h4>
                        <p class="text-gray-600 text-sm">Grabados láser de todo tipo con precisión</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-key text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Llaveros Personalizados</h4>
                        <p class="text-gray-600 text-sm">Llaveros acrílicos únicos y personalizados</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-trophy text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Trofeos Personalizados</h4>
                        <p class="text-gray-600 text-sm">Trofeos únicos para reconocer logros especiales</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-user-graduate text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Togas y Biretes</h4>
                        <p class="text-gray-600 text-sm">Togas y biretes de alta calidad para tu graduación</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-book text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Libros Empastados</h4>
                        <p class="text-gray-600 text-sm">Empastado profesional de libros y documentos</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-lightbulb text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Avisos Corpóreos</h4>
                        <p class="text-gray-600 text-sm">Avisos que brillan como tu marca</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-camera text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Fotografía Profesional</h4>
                        <p class="text-gray-600 text-sm">Sesiones fotográficas profesionales</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-certificate text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Diplomas Fotográficos</h4>
                        <p class="text-gray-600 text-sm">Diplomas en papel fotográfico de alta calidad</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-lamp text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Lámparas Acrílicas</h4>
                        <p class="text-gray-600 text-sm">Lámparas acrílicas personalizadas</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-mug-hot text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Tazas Grabadas</h4>
                        <p class="text-gray-600 text-sm">Tazas personalizadas con grabado láser</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-folder text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Carpetas de Graduación</h4>
                        <p class="text-gray-600 text-sm">Carpetas especiales para graduaciones 2025</p>
                    </div>
                </div>

                <div class="service-card rounded-xl p-6 card-hover">
                    <div class="text-center">
                        <i class="fas fa-thermometer text-4xl text-purple-600 mb-4"></i>
                        <h4 class="text-lg font-semibold mb-2">Termos Personalizados</h4>
                        <p class="text-gray-600 text-sm">Termos únicos con tu diseño personalizado</p>
                    </div>
                </div>
            </div>

            <!-- Special Promotions -->
            <div class="mt-16">
                <h4 class="text-3xl font-bold text-center text-gray-800 mb-8">Promociones Especiales</h4>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                    <div class="bg-gradient-to-r from-green-400 to-blue-500 rounded-xl p-6 text-white card-hover">
                        <h5 class="text-xl font-bold mb-3">Promos Económicas</h5>
                        <p class="mb-4">Paquetes especiales a precios increíbles para tu graduación</p>
                        <a href="https://wa.me/584147622212" class="bg-white text-green-600 px-4 py-2 rounded-full font-semibold hover:bg-gray-100 transition">
                            Consultar
                        </a>
                    </div>

                    <div class="bg-gradient-to-r from-purple-400 to-pink-500 rounded-xl p-6 text-white card-hover">
                        <h5 class="text-xl font-bold mb-3">Promos Boys Preescolar/Sexto</h5>
                        <p class="mb-4">Paquetes especiales para los más pequeños</p>
                        <a href="https://wa.me/584147622212" class="bg-white text-purple-600 px-4 py-2 rounded-full font-semibold hover:bg-gray-100 transition">
                            Consultar
                        </a>
                    </div>

                    <div class="bg-gradient-to-r from-yellow-400 to-orange-500 rounded-xl p-6 text-white card-hover">
                        <h5 class="text-xl font-bold mb-3">Préstamos de Toga</h5>
                        <p class="mb-4">Alquiler de togas y biretes de alta calidad</p>
                        <a href="https://wa.me/584147622212" class="bg-white text-yellow-600 px-4 py-2 rounded-full font-semibold hover:bg-gray-100 transition">
                            Consultar
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section id="galeria" class="py-20 bg-gray-100">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h3 class="text-4xl font-bold text-gray-800 mb-4">Nuestra Galería</h3>
                <p class="text-gray-600 max-w-2xl mx-auto">Explora nuestros trabajos y productos a través de nuestras redes sociales. Cada proyecto es único y especial.</p>
            </div>

            <!-- Instagram Videos Section -->
            <div class="mb-12">
                <h4 class="text-2xl font-bold text-center text-gray-800 mb-8">Videos de Nuestros Trabajos</h4>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/reel/DLnO7enOvIk/embed" width="100%" height="400" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/reel/DHbXgkpOh_G/embed" width="100%" height="400" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/reel/DIC3IZGNtqD/embed" width="100%" height="400" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/reel/C4WQfNjgvfz/embed" width="100%" height="400" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/reel/C3NppxxAymT/embed" width="100%" height="400" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/reel/DJXsa0BN26D/embed" width="100%" height="400" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                </div>
            </div>

            <!-- Instagram Photos Section -->
            <div>
                <h4 class="text-2xl font-bold text-center text-gray-800 mb-8">Galería de Productos</h4>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-4">
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/p/DGi5BthOsAl/embed" width="100%" height="300" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/p/DEl_evpuwsH/embed" width="100%" height="300" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/p/DEl-aMmOssB/embed" width="100%" height="300" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/p/DEl9eLrOPMC/embed" width="100%" height="300" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/p/DEl6bvNtzPR/embed" width="100%" height="300" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/p/DEkm-v_uvlD/embed" width="100%" height="300" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/p/DEklDh1ukCt/embed" width="100%" height="300" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/p/DEiwlKhylbk/embed" width="100%" height="300" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/p/DEiv7o-SX5S/embed" width="100%" height="300" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/p/DEgsHUJt6aP/embed" width="100%" height="300" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/p/DEgre7ot1I6/embed" width="100%" height="300" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                    <div class="instagram-embed bg-white p-4 rounded-xl">
                        <iframe src="https://www.instagram.com/p/DEgqaVqtZRW/embed" width="100%" height="300" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contacto" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h3 class="text-4xl font-bold text-gray-800 mb-4">Contáctanos</h3>
                <p class="text-gray-600 max-w-2xl mx-auto">Estamos aquí para hacer realidad tu graduación perfecta. Contacta con nuestro equipo de expertos.</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
                <!-- Contact Info -->
                <div>
                    <div class="bg-gray-50 rounded-xl p-8">
                        <h4 class="text-2xl font-bold text-gray-800 mb-6">Información de Contacto</h4>
                        
                        <div class="space-y-6">
                            <div class="flex items-start">
                                <i class="fas fa-map-marker-alt text-purple-600 text-xl mr-4 mt-1"></i>
                                <div>
                                    <h5 class="font-semibold text-gray-800 mb-1">Ubicación</h5>
                                    <p class="text-gray-600">AV. BOLÍVAR CON CALLE BOMBONA<br>EDF. FIORELLA PISO 1 LOCAL 2<br>MATURÍN EDO MONAGAS</p>
                                </div>
                            </div>

                            <div class="flex items-start">
                                <i class="fab fa-whatsapp text-green-600 text-xl mr-4 mt-1"></i>
                                <div>
                                    <h5 class="font-semibold text-gray-800 mb-1">WhatsApp</h5>
                                    <div class="space-y-1">
                                        <p class="text-gray-600">+58 414-762-2212</p>
                                        <p class="text-gray-600">+58 424-950-0497</p>
                                        <p class="text-gray-600">+58 412-527-4607</p>
                                    </div>
                                </div>
                            </div>

                            <div class="flex items-start">
                                <i class="fas fa-user-tie text-purple-600 text-xl mr-4 mt-1"></i>
                                <div>
                                    <h5 class="font-semibold text-gray-800 mb-1">Presidente</h5>
                                    <p class="text-gray-600">LUIS NAVAS</p>
                                </div>
                            </div>
                        </div>

                        <!-- Social Media -->
                        <div class="mt-8">
                            <h5 class="font-semibold text-gray-800 mb-4">Síguenos en Redes Sociales</h5>
                            <div class="flex space-x-4">
                                <a href="https://instagram.com/lacasadelastogasmonagas" target="_blank" class="bg-gradient-to-r from-purple-500 to-pink-500 text-white p-3 rounded-full hover:scale-110 transition">
                                    <i class="fab fa-instagram text-xl"></i>
                                </a>
                                <a href="https://facebook.com/lacasadelastogas" target="_blank" class="bg-blue-600 text-white p-3 rounded-full hover:scale-110 transition">
                                    <i class="fab fa-facebook-f text-xl"></i>
                                </a>
                                <a href="https://twitter.com/casadelastogas" target="_blank" class="bg-blue-400 text-white p-3 rounded-full hover:scale-110 transition">
                                    <i class="fab fa-twitter text-xl"></i>
                                </a>
                                <a href="https://tiktok.com/@lacasadelastogas" target="_blank" class="bg-black text-white p-3 rounded-full hover:scale-110 transition">
                                    <i class="fab fa-tiktok text-xl"></i>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Contact Form -->
                <div>
                    <div class="bg-gradient-to-r from-purple-600 to-blue-600 rounded-xl p-8 text-white">
                        <h4 class="text-2xl font-bold mb-6">Solicita tu Cotización</h4>
                        <form class="space-y-4">
                            <div>
                                <label class="block text-sm font-medium mb-2">Nombre Completo</label>
                                <input type="text" class="w-full px-4 py-3 rounded-lg bg-white text-gray-800 focus:outline-none focus:ring-2 focus:ring-purple-300">
                            </div>
                            <div>
                                <label class="block text-sm font-medium mb-2">Teléfono</label>
                                <input type="tel" class="w-full px-4 py-3 rounded-lg bg-white text-gray-800 focus:outline-none focus:ring-2 focus:ring-purple-300">
                            </div>
                            <div>
                                <label class="block text-sm font-medium mb-2">Email</label>
                                <input type="email" class="w-full px-4 py-3 rounded-lg bg-white text-gray-800 focus:outline-none focus:ring-2 focus:ring-purple-300">
                            </div>
                            <div>
                                <label class="block text-sm font-medium mb-2">Servicio de Interés</label>
                                <select class="w-full px-4 py-3 rounded-lg bg-white text-gray-800 focus:outline-none focus:ring-2 focus:ring-purple-300">
                                    <option>Paquete de Graduación Completo</option>
                                    <option>Togas y Biretes</option>
                                    <option>Medallas Personalizadas</option>
                                    <option>Anillos de Graduación</option>
                                    <option>Fotografía Profesional</option>
                                    <option>Diseño Gráfico</option>
                                    <option>Grabados Láser</option>
                                    <option>Productos Personalizados</option>
                                    <option>Otros</option>
                                </select>
                            </div>
                            <div>
                                <label class="block text-sm font-medium mb-2">Mensaje</label>
                                <textarea rows="4" class="w-full px-4 py-3 rounded-lg bg-white text-gray-800 focus:outline-none focus:ring-2 focus:ring-purple-300" placeholder="Describe tu proyecto o necesidades..."></textarea>
                            </div>
                            <button type="submit" class="w-full bg-white text-purple-600 py-3 rounded-lg font-semibold hover:bg-gray-100 transition">
                                Enviar Solicitud
                            </button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Why Choose Us Section -->
    <section class="py-20 bg-gray-100">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h3 class="text-4xl font-bold text-gray-800 mb-4">¿Por Qué Elegirnos?</h3>
                <p class="text-gray-600 max-w-2xl mx-auto">Somos más que un proveedor, somos tu aliado para crear momentos inolvidables.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                <div class="text-center">
                    <div class="bg-purple-100 w-20 h-20 rounded-full flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-star text-3xl text-purple-600"></i>
                    </div>
                    <h4 class="text-xl font-semibold mb-2">Calidad Premium</h4>
                    <p class="text-gray-600">Productos de la más alta calidad con materiales resistentes y duraderos</p>
                </div>

                <div class="text-center">
                    <div class="bg-green-100 w-20 h-20 rounded-full flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-heart text-3xl text-green-600"></i>
                    </div>
                    <h4 class="text-xl font-semibold mb-2">Friendly en Todo</h4>
                    <p class="text-gray-600">Servicio amigable y personalizado en cada interacción</p>
                </div>

                <div class="text-center">
                    <div class="bg-blue-100 w-20 h-20 rounded-full flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-rocket text-3xl text-blue-600"></i>
                    </div>
                    <h4 class="text-xl font-semibold mb-2">Entrega Rápida</h4>
                    <p class="text-gray-600">Cumplimos con los tiempos de entrega para tu evento especial</p>
                </div>

                <div class="text-center">
                    <div class="bg-yellow-100 w-20 h-20 rounded-full flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-palette text-3xl text-yellow-600"></i>
                    </div>
                    <h4 class="text-xl font-semibold mb-2">Diseños Únicos</h4>
                    <p class="text-gray-600">Cada producto es personalizado para hacerte único</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-12">
        <div class="container mx-auto px-6">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                <div>
                    <div class="flex items-center mb-4">
                        <i class="fas fa-graduation-cap text-2xl text-purple-400 mr-3"></i>
                        <h3 class="text-xl font-bold">La Casa de las Togas CA</h3>
                    </div>
                    <p class="text-gray-400 mb-4">Especialistas en hacer de tu graduación un momento único e inolvidable. Calidad, diseño y atención personalizada.</p>
                    <div class="flex space-x-3">
                        <a href="https://instagram.com/lacasadelastogasmonagas" class="text-gray-400 hover:text-purple-400 transition">
                            <i class="fab fa-instagram text-xl"></i>
                        </a>
                        <a href="https://facebook.com/lacasadelastogas" class="text-gray-400 hover:text-blue-400 transition">
                            <i class="fab fa-facebook-f text-xl"></i>
                        </a>
                        <a href="https://twitter.com/casadelastogas" class="text-gray-400 hover:text-blue-300 transition">
                            <i class="fab fa-twitter text-xl"></i>
                        </a>
                        <a href="https://tiktok.com/@lacasadelastogas" class="text-gray-400 hover:text-white transition">
                            <i class="fab fa-tiktok text-xl"></i>
                        </a>
                    </div>
                </div>

                <div>
                    <h4 class="text-lg font-semibold mb-4">Servicios Principales</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li>Paquetes de Graduación</li>
                        <li>Togas y Biretes</li>
                        <li>Medallas Personalizadas</li>
                        <li>Anillos de Graduación</li>
                        <li>Fotografía Profesional</li>
                        <li>Diseño Gráfico</li>
                    </ul>
                </div>

                <div>
                    <h4 class="text-lg font-semibold mb-4">Productos Especiales</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li>Grabados Láser</li>
                        <li>Lámparas Acrílicas</li>
                        <li>Trofeos Personalizados</li>
                        <li>Placas de Reconocimiento</li>
                        <li>Llaveros Personalizados</li>
                        <li>Productos en MDF</li>
                    </ul>
                </div>

                <div>
                    <h4 class="text-lg font-semibold mb-4">Contacto</h4>
                    <div class="space-y-2 text-gray-400">
                        <p><i class="fas fa-map-marker-alt mr-2"></i>AV. BOLÍVAR CON CALLE BOMBONA</p>
                        <p class="ml-5">EDF. FIORELLA PISO 1 LOCAL 2</p>
                        <p class="ml-5">MATURÍN EDO MONAGAS</p>
                        <p><i class="fab fa-whatsapp mr-2"></i>+58 414-762-2212</p>
                        <p><i class="fas fa-user-tie mr-2"></i>LUIS NAVAS (Presidente)</p>
                    </div>
                </div>
            </div>

            <div class="border-t border-gray-700 mt-8 pt-8 text-center text-gray-400">
                <p>&copy; 2024 La Casa de las Togas CA. Todos los derechos reservados. | Hacemos de tu graduación un momento único e inolvidable.</p>
            </div>
        </div>
    </footer>

    <!-- Chatbot Integration -->
    <script type="module">
        import { createChat } from 'https://cdn.jsdelivr.net/npm/@n8n/chat/dist/chat.bundle.es.js';
        
        createChat({
            webhookUrl: 'http://localhost:5678/webhook/4b1cbcc2-7225-48fb-9714-f0976ef2d2f8/chat'
        });
    </script>

    <!-- JavaScript for smooth scrolling and interactions -->
    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Add loading animation for Instagram embeds
        document.addEventListener('DOMContentLoaded', function() {
            const iframes = document.querySelectorAll('iframe[src*="instagram.com"]');
            iframes.forEach(iframe => {
                iframe.addEventListener('load', function() {
                    this.style.opacity = '1';
                });
                iframe.style.opacity = '0.5';
                iframe.style.transition = 'opacity 0.3s ease';
            });
        });

        // Form submission handler
        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Get form data
            const formData = new FormData(this);
            const data = Object.fromEntries(formData);
            
            // Create WhatsApp message
            const message = `Hola! Me interesa solicitar información sobre:\n\nNombre: ${data.nombre || 'No especificado'}\nTeléfono: ${data.telefono || 'No especificado'}\nEmail: ${data.email || 'No especificado'}\nServicio: ${data.servicio || 'No especificado'}\nMensaje: ${data.mensaje || 'No especificado'}`;
            
            // Open WhatsApp
            const whatsappUrl = `https://wa.me/584147622212?text=${encodeURIComponent(message)}`;
            window.open(whatsappUrl, '_blank');
            
            // Show success message
            alert('Gracias por tu interés. Te estamos redirigiendo a WhatsApp para continuar la conversación.');
        });

        // Mobile menu toggle
        const mobileMenuBtn = document.querySelector('.md\\:hidden button');
        const mobileMenu = document.querySelector('.md\\:flex');
        
        if (mobileMenuBtn) {
            mobileMenuBtn.addEventListener('click', function() {
                // Toggle mobile menu visibility
                mobileMenu.classList.toggle('hidden');
                mobileMenu.classList.toggle('flex');
                mobileMenu.classList.toggle('flex-col');
                mobileMenu.classList.toggle('absolute');
                mobileMenu.classList.toggle('top-full');
                mobileMenu.classList.toggle('left-0');
                mobileMenu.classList.toggle('w-full');
                mobileMenu.classList.toggle('bg-white');
                mobileMenu.classList.toggle('shadow-lg');
                mobileMenu.classList.toggle('p-4');
            });
        }
    </script>
</body>
</html>

