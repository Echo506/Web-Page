<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Disfraces Tétricos para Mascotas</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Creepster&family=Inter:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #111;
        }
        .font-creepster {
            font-family: 'Creepster', cursive;
        }
        /* -- Efecto de goteo de sangre -- */
        .blood-drip {
            position: relative;
        }
        .blood-drip::after {
            content: '';
            position: absolute;
            top: 100%;
            left: 50%;
            transform: translateX(-50%);
            width: 150%;
            height: 50px;
            background-image: radial-gradient(circle at 50% 0, #8B0000 10px, transparent 11px),
                              radial-gradient(circle at 25% 0, #8B0000 15px, transparent 16px),
                              radial-gradient(circle at 75% 0, #8B0000 12px, transparent 13px),
                              radial-gradient(circle at 15% 0, #8B0000 8px, transparent 9px),
                              radial-gradient(circle at 85% 0, #8B0000 18px, transparent 19px);
            background-repeat: no-repeat;
            background-size: 100% 100%;
            filter: drop-shadow(0 2px 2px rgba(0,0,0,0.5));
        }

        /* -- Estilo de las imágenes del collage -- */
        .collage-img {
            transition: transform 0.3s ease, filter 0.3s ease;
            filter: grayscale(50%) contrast(1.1) brightness(0.9);
            border: 4px solid #1a1a1a;
            box-shadow: 0 0 15px rgba(255, 0, 0, 0.4);
        }
        .collage-img:hover {
            transform: scale(1.05) rotate(0deg) !important;
            filter: grayscale(0%) contrast(1) brightness(1);
            z-index: 10;
        }
        
        /* -- Rotaciones aleatorias para el efecto collage -- */
        .rotate-neg-3 { transform: rotate(-3deg); }
        .rotate-2 { transform: rotate(2deg); }
        .rotate-neg-1 { transform: rotate(-1deg); }
        .rotate-3 { transform: rotate(3deg); }
        .rotate-neg-2 { transform: rotate(-2deg); }
        
        .glow-button {
            box-shadow: 0 0 5px #ffc800, 0 0 15px #ffc800, 0 0 25px #ffc800;
        }
        .glow-button:hover {
            box-shadow: 0 0 10px #ffc800, 0 0 25px #ffc800, 0 0 50px #ffc800;
        }
    </style>
</head>
<body class="bg-black text-white overflow-x-hidden">

    <div class="min-h-screen flex flex-col items-center justify-center p-4 md:p-8 relative">

        <!-- Título principal -->
        <header class="text-center mb-8 z-20">
            <h1 class="font-creepster text-6xl md:text-8xl text-red-700 blood-drip" style="text-shadow: 3px 3px 0px #000, 0 0 20px rgba(255,0,0,0.7);">NOCHES DE TERROR</h1>
            <p class="font-creepster text-3xl md:text-5xl text-yellow-400 mt-12" style="text-shadow: 2px 2px 0px #000;">Viste a tu mascota para la ocasión</p>
        </header>

        <!-- Collage de Imágenes -->
        <main class="relative w-full max-w-5xl grid grid-cols-2 md:grid-cols-4 gap-4 items-center justify-center p-4">
            <!-- Imagen 1 -->
            <div class="md:col-span-1 md:row-span-1 z-10">
                <img src="https://huell-a-store.com/cdn/shop/products/product-image-1533514210.jpg?v=1632873432" alt="Perro con disfraz de muñeco diabólico" class="w-full h-auto rounded-lg collage-img rotate-neg-3">
            </div>
            
            <!-- Imagen 2 -->
            <div class="md:col-span-2 md:row-span-2 z-0">
                 <img src="https://huell-a-store.com/cdn/shop/files/S2ba3c0e3e9ea43a992e0787e9c5663e8U.jpg_960x960.jpg?v=1684347209" alt="Gato con disfraz de astronauta" class="w-full h-auto rounded-lg collage-img rotate-2">
            </div>

            <!-- Imagen 3 -->
            <div class="md:col-span-1 md:row-span-1 z-10">
                <img src="https://huell-a-store.com/cdn/shop/products/product-image-1867825396.jpg?v=1632873199" alt="Perro con suéter de calaveras" class="w-full h-auto rounded-lg collage-img rotate-neg-1">
            </div>

             <!-- Imagen 4 -->
             <div class="md:col-span-2 md:row-span-2 z-0">
                <img src="https://huell-a-store.com/cdn/shop/products/product-image-1237930107.jpg?v=1632872392" alt="Gato con disfraz de vaquero" class="w-full h-auto rounded-lg collage-img rotate-3">
             </div>

            <!-- Imagen 5 -->
            <div class="md:col-span-2 md:row-span-1 z-10">
                <img src="https://huell-a-store.com/cdn/shop/products/product-image-1867825350.jpg?v=1632872688" alt="Sudadera negra de Halloween para mascota" class="w-full h-auto rounded-lg collage-img rotate-neg-2">
            </div>

        </main>

        <!-- Llamada a la acción -->
        <footer class="mt-12 text-center z-20">
            <p class="text-lg text-gray-300 mb-6">Este octubre, desata el lado más terrorífico de tu mejor amigo.</p>
            <a href="https://huell-a-store.com/" target="_blank" class="inline-block bg-yellow-500 text-black font-bold font-creepster text-3xl px-10 py-4 rounded-md transition-transform duration-300 hover:scale-110 glow-button">
                ¡COMPRAR AHORA! 🛍️
            </a>
        </footer>
        
        <!-- Elemento decorativo de fondo -->
        <div class="absolute inset-0 bg-black bg-opacity-50" style="background-image: radial-gradient(rgba(139, 0, 0, 0.3) 1px, transparent 1px); background-size: 20px 20px;"></div>

    </div>

</body>
</html>



# Web-Page