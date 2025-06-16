<script setup lang="ts">
    import { ref } from 'vue';

    const isOpen = ref(false);
</script>

<template>
    <header>
      <nav class="bg-slate-950 text-white py-4">
        <div class="container mx-auto flex items-center justify-between px-4 md:px-0">
            <div class="flex items-center">
                <img src="../assets/images/logo.jpg" alt="Logo de la empresa de cámaras de seguridad" class="h-8 mr-4">
                <a href="#" class="text-xl font-bold">LookTech</a>
            </div>

            <div class="md:hidden ">
                <button @click="isOpen = !isOpen" class="text-white focus:outline-none">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" v-if="!isOpen" d="M4 6h16M4 12h16M4 18h16"></path>
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" v-if="isOpen" d="M6 18L18 6M6 6l12 12"></path>
                </svg>
                </button>
            </div>

            <div class="hidden md:flex space-x-4">
                <a href="#" class="hover:text-gray-200">Inicio</a>
                <a href="#" class="hover:text-gray-200">Cámaras de Seguridad</a>
                <a href="#" class="hover:text-gray-200">Acerca de</a>
                <a href="#" class="hover:text-gray-200">Servicios</a>
                <a href="#" class="hover:text-gray-200">Contacto</a>
            </div>
            </div>

            <div v-if="isOpen" class="md:hidden bg-slate-950 pb-4">
            <div class="flex flex-col items-center space-y-4">
                <a href="#" class="block text-white hover:text-gray-200 w-full text-center py-2">Inicio</a>
                <a href="#" class="block text-white hover:text-gray-200 w-full text-center py-2">Cámaras de Seguridad</a>
                <a href="#" class="block text-white hover:text-gray-200 w-full text-center py-2">Acerca de</a>
                <a href="#" class="block text-white hover:text-gray-200 w-full text-center py-2">Servicios</a>
                <a href="#" class="block text-white hover:text-gray-200 w-full text-center py-2">Contacto</a>
            </div>
            </div>
        </nav>
    </header>
    <section 
        class="relative h-screen bg-cover bg-center flex items-center bg-[url('../assets/images/background.jpg')]" 
    >
        <div class="absolute inset-0 bg-black opacity-50"></div>

        <div class="container mx-auto relative z-10 flex flex-col md:flex-row items-center py-10 md:py-0 px-4">
            <div class="w-full md:w-1/2 text-white text-center md:text-left mb-10 md:mb-0">
                <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-6">
                Cámaras de seguridad para proteger lo que es realmente valioso para ti.
                </h1>
                <p class="text-lg md:text-xl mb-8 max-w-xl mx-auto md:mx-0 opacity-90">
                Protege tu negocio y a tu familia con nuestros servicios en Look Tech.
                </p>
                <a href="#" class="inline-block bg-slate-950 hover:bg-slate-700 text-white font-semibold py-3 px-8 rounded-lg shadow-lg transition duration-300 transform hover:scale-105">
                Contáctanos
                </a>
            </div>

            <div class="w-full md:w-1/2 flex justify-center items-center">
                <img 
                src="../assets/images/camaras.png" 
                alt="Varias cámaras de seguridad" 
                class="max-w-full h-auto object-contain"
                style="max-height: 80vh;"
                >
            </div>
        </div>
    </section>
    <Section>
        <div class="flex justify-center">
            <div class="pt-20 pb-20 px-4 md:px-0 text-center">
                <h4 class="text-3xl md:text-3xl lg:text-4xl font-semibold text-gray-800">
                    CATEGORÍAS MÁS POPULARES EN CÁMARAS DE SEGURIDAD
                </h4>
            </div>
        </div>
        <div class="container mx-auto py-8 px-4">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 justify-items-center">
            <!-- Card 1 -->
                <div class="max-w-sm bg-white rounded-xl shadow-lg overflow-hidden flex flex-col">
                    <div class="flex justify-center">
                    <img
                        src="../assets/images/paquete-camaras.png"
                        alt="Paquete de Cámaras de Seguridad"
                        class="w-full h-auto object-cover"
                    >
                    </div>

                    <div class="p-6 flex flex-col flex-grow">
                    <h3 class="text-xl md:text-2xl font-bold text-gray-800 uppercase text-center mb-4">
                        PAQUETE DE CÁMARAS DE SEGURIDAD
                    </h3>
                    <p class="text-gray-600 text-sm md:text-base leading-relaxed mb-6 text-justify flex-grow">
                        Un paquete de Cámaras de Seguridad para cada necesidad, grabación 24hrs, tecnología de ultra almacenamiento
                        con visión nocturna, detección de movimiento y App para móviles gratis, sin rentas para verlas en cualquier
                        parte.
                    </p>

                    <div class="text-center mt-auto">
                        <a
                        href="#"
                        class="inline-block border border-slate-950 text-slate-950 font-semibold py-3 px-6 rounded-lg
                                hover:bg-slate-950 hover:text-white transition duration-300 ease-in-out"
                        >
                        Paquetes de Cámaras
                        </a>
                    </div>
                    </div>
                </div>

                <!-- Card 2 -->
                <div class="max-w-sm bg-white rounded-xl shadow-lg overflow-hidden flex flex-col">
                    <div class="flex justify-center">
                    <img
                        src="../assets/images/camaras-seguridad.png"
                        alt="Paquete de Cámaras de Seguridad"
                        class="w-80 h-auto object-cover"
                    >
                    </div>

                    <div class="p-6 flex flex-col flex-grow">
                    <h3 class="text-xl md:text-2xl font-bold text-gray-800 uppercase text-center mb-4">
                        CÁMARAS DE SEGURIDAD
                    </h3>
                    <p class="text-gray-600 text-sm md:text-base leading-relaxed mb-6 text-justify flex-grow">
                        La mejor en de Cámaras de Seguridad domo, Ip, inalámbricas, panorámicas, 4K, térmicas, visión nocturna, antivandálicas, para intemperie, para climas extremos, PTZ y analogas.
                    </p>

                    <div class="text-center mt-auto">
                        <a
                        href="#"
                        class="inline-block border border-slate-950 text-slate-950 font-semibold py-3 px-6 rounded-lg
                                hover:bg-slate-950 hover:text-white transition duration-300 ease-in-out"
                        >
                        Cámaras de Seguridad
                        </a>
                    </div>
                    </div>
                </div>

                <!-- Card 3 -->
                <div class="max-w-sm bg-white rounded-xl shadow-lg overflow-hidden flex flex-col">
                    <div class="flex justify-center">
                    <img
                        src="../assets/images/camara-wifi.png"
                        alt="Paquete de Cámaras de Seguridad"
                        class="w-35 h-auto object-cover"
                    >
                    </div>

                    <div class="p-6 flex flex-col flex-grow">
                    <h3 class="text-xl md:text-2xl font-bold text-gray-800 uppercase text-center mb-4">
                        CÁMARAS WIFI
                    </h3>
                    <p class="text-gray-600 text-sm md:text-base leading-relaxed mb-6 text-justify flex-grow">
                        Amplio catálogo con las Cámaras Wifi más completas; video UHD 4K, audio bidireccional disuasorio, alertas inmediatas, seguimiento de personas, trasmisión Wi-Fi Inalámbrica, almacenamiento interno, garantía y soporte.
                    </p>

                    <div class="text-center mt-auto">
                        <a
                        href="#"
                        class="inline-block border border-slate-950 text-slate-950 font-semibold py-3 px-6 rounded-lg
                                hover:bg-slate-950 hover:text-white transition duration-300 ease-in-out"
                        >
                        Cámaras WIFI
                        </a>
                    </div>
                    </div>
                </div>
            </div>
        </div>
    </Section>
    <section 
        class="mt-20 relative h-150 bg-cover bg-center flex items-center p-4 md:p-8 lg:p-16 bg-[url('../assets/images/background-teziutlan.png')]" 
    >
        <div class="absolute inset-0 bg-black opacity-50"></div>

        <div class="relative z-10 text-white max-w-4xl mx-auto text-center md:text-left">
        <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-6">
            CÁMARAS DE VIGILANCIA
        </h1>
        <p class="text-lg md:text-xl mb-8 opacity-90">
            Si buscas Cámaras de vigilancia en Teziutlán Puebla, nosotros somos tu mejor opción
            contamos con todas las soluciones en videovigilancia para todas tus necesidades como:
            oficina, industrias, hogar, hoteles, fabricas, cadenas comerciales y mucho más...
        </p>
        <a 
            href="#" 
            class="inline-block bg-slate-950 hover:bg-slate-700 text-white font-semibold py-3 px-8 rounded-lg 
                shadow-lg transition duration-300 transform hover:scale-105"
        >
            Ir a Paquetes de Cámaras
        </a>
        </div>
    </section>
    <section class="bg-white py-25 px-4 md:px-8 lg:px-16">
        <div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-8 items-start">
            <div class="text-left">
                <h2 class="text-2xl md:text-3xl font-bold text-gray-800 mb-6 leading-tight">
                ¿PORQUÉ SOMOS TU MEJOR OPCIÓN EN VENTA DE CÁMARAS DE SEGURIDAD?
                </h2>
                <p class="text-gray-700 text-lg md:text-xl leading-relaxed">
                Simple, somos una <strong class="font-semibold text-slate-950">empresa 100% Teziuteca</strong>
                con más experiencia en <strong class="font-semibold text-slate-950">Cámaras de Seguridad</strong>
                en toda la zona. ¡Con nosotros compra SEGURIDAD!
                </p>
            </div>

            <div class="space-y-8">
                <div class="flex items-start">
                    <div class="flex-shrink-0 mr-4 mt-1">
                        <svg class="w-8 h-8 text-slate-950" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                            <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path>
                        </svg>
                    </div>
                    <div>
                        <h3 class="text-xl font-semibold text-gray-800 mb-2">Calidad y honestidad</h3>
                        <p class="text-gray-600">
                        Ofrecemos a nuestros clientes productos de calidad con soluciones adecuadas para satisfacer
                        sus necesidades y brindarles tranquilidad.
                        </p>
                    </div>
                    </div>

                    <div class="flex items-start">
                    <div class="flex-shrink-0 mr-4 mt-1">
                        <svg class="w-8 h-8 text-slate-950" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                            <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path>
                        </svg>
                    </div>
                    <div>
                        <h3 class="text-xl font-semibold text-gray-800 mb-2">Garantía</h3>
                        <p class="text-gray-600">
                        Ofrecemos a nuestros clientes garantía de nuestros servicios y productos de fábrica así como la
                        instalación.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <section class="bg-white py-10 px-4 md:px-8 lg:px-16">
        <div class="max-w-4xl mx-auto text-center">
            <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-6">
               ¿QUIENES SOMOS?
            </h2>

            <p class="text-gray-700 text-lg md:text-xl leading-relaxed">
                Somos una empresa líder en Seguridad electrónica, dedicada a la asesoría, venta e instalación de
                equipos de Videovigilancia (CCTV) y videocámaras de seguridad, de última tecnología para casas
                y negocios, ofreciéndole mucho valor agregado a los productos que comercializa por la constante
                capacitación de su personal.
            </p>
        </div>
    </section>
    <section class="bg-white py-12 px-4 md:px-8 lg:px-16">
        <div class="max-w-7xl mx-auto">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="flex flex-col bg-white rounded-lg shadow-lg overflow-hidden border border-gray-200">
                    <div class="p-4 flex justify-center items-center h-48">
                        <img
                        src="../assets/images/camara-wifi2.png"
                        alt="Cámara de domo para negocios"
                        class="max-w-[10rem] h-auto object-contain"
                        />
                    </div>
                    <div class="p-6 flex flex-col flex-grow">
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">Videovigilancia para negocios</h3>
                        <p class="text-gray-700 mb-6 flex-grow">
                        Con sus cámaras puede <strong class="font-bold">Supervisar, Escuchar y Grabar</strong> su negocio a distancia
                        en tiempo real, con tecnología inteligente para Prevenir, Aumentar su Productividad,
                        Reducir Costos y Tiempos.
                        </p>
                        <div class="mt-auto">
                            <button class="w-full bg-slate-950 hover:bg-slate-800 text-white font-semibold py-3 px-6 rounded-md transition duration-300">
                                SABER MÁS.
                            </button>
                        </div>
                    </div>
                </div>
                <div class="flex flex-col bg-white rounded-lg shadow-lg overflow-hidden border border-gray-200">
                    <div class="p-4 flex justify-center items-center h-48">
                        <img
                        src="../assets/images/camaras-hogar.png"
                        alt="Cámara bullet para el hogar"
                        class="max-w-[15rem] h-auto object-contain"
                        />
                    </div>
                    <div class="p-6 flex flex-col flex-grow">
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">Videovigilancia para el hogar</h3>
                        <p class="text-gray-700 mb-6 flex-grow">
                        Disuasión, tecnología inteligente, monitoreo, grabación y visualización en
                        cualquier parte del mundo las 24 horas, libre de contratos y
                        soporte técnico; todo esto a un muy bajo costo.
                        </p>
                        <div class="mt-auto">
                            <button class="w-full bg-slate-950 hover:bg-slate-800 text-white font-semibold py-3 px-6 rounded-md transition duration-300">
                                SABER MÁS.
                            </button>
                        </div>
                    </div>
                </div>
                <div class="flex flex-col bg-white rounded-lg shadow-lg overflow-hidden border border-gray-200">
                    <div class="p-4 flex justify-center items-center h-48">
                        <img
                        src="../assets/images/camara-wifi2.png"
                        alt="Cámara de domo para instalación"
                        class="max-w-[10rem] h-auto object-contain"
                        />
                    </div>
                    <div class="p-6 flex flex-col flex-grow">
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">Instalación y Soporte Técnico</h3>
                        <p class="text-gray-700 mb-6 flex-grow">
                        Técnicos <strong class="font-bold">CERTIFICADOS EN CCTV</strong> y en constante
                        capacitación para trabajar con diferentes marcas, le
                        asesorarán para la correcta elección, instalación y
                        protección de su equipo de videovigilancia.
                        </p>
                        <div class="mt-auto">
                            <button class="w-full bg-slate-950 hover:bg-slate-800 text-white font-semibold py-3 px-6 rounded-md transition duration-300">
                                SABER MÁS.
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <div>
       <footer class="bg-slate-950 text-white py-12 px-4">
            <div class="container mx-auto grid grid-cols-1 md:grid-cols-4 gap-8 text-center md:text-left">
                <div class="flex flex-col items-center md:items-start mb-6 md:mb-0">
                    <img 
                    src="../assets/images/logo.jpg" 
                    alt="Logo LookTech" 
                    class="h-16 mb-4"
                    >
                    <p class="text-sm">Protegiendo lo que es valioso para ti.</p>
                </div>

                <div class="mb-6 md:mb-0">
                    <h5 class="font-bold text-lg mb-4">Contacto</h5>
                    <p class="text-sm mb-2">Email: <a href="mailto:look-tech@gmail.com" class="hover:underline">look-tech@gmail.com</a></p>
                    <p class="text-sm">Tel: <a href="tel:2313333333" class="hover:underline">231-333-33-33</a></p>
                    <p class="text-sm mt-2">Teziutlán, Puebla, México</p>
                </div>

                <div class="mb-6 md:mb-0">
                    <h5 class="font-bold text-lg mb-4">Redes Sociales</h5>
                    <ul class="space-y-2">
                    <li><a href="#" class="hover:underline text-sm">Facebook</a></li>
                    <li><a href="#" class="hover:underline text-sm">Instagram</a></li>
                    <li><a href="#" class="hover:underline text-sm">Twitter</a></li>
                    <li><a href="#" class="hover:underline text-sm">Whatsapp</a></li>
                    </ul>
                </div>

                <div>
                    <h5 class="font-bold text-lg mb-4">Horarios</h5>
                    <p class="text-sm leading-relaxed">
                    Contáctenos para cualquier consulta de Lunes a Domingo de 9:00 am a 8:00 pm.
                    </p>
                </div>

                </div>

                <div class="border-t border-gray-700 mt-8 pt-8 text-center text-sm opacity-80">
                    &copy; 2025 LookTech. Todos los derechos reservados.
                </div>
        </footer>
    </div>
</template>

<style scoped>
</style>
