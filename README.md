</head>
<body class="bg-gray-900 text-gray-100 min-h-screen font-sans">
    <!-- Navbar -->
    <nav class="bg-gray-900 border-b border-gray-800 fixed w-full z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-16">
                <div class="flex items-center">
                    <div class="flex-shrink-0 flex items-center">
                        <span class="text-red-500 font-bold text-2xl">KSG</span>
                        <span class="ml-2 text-white font-bold text-xl hidden md:block">Kaua Safado Guloso</span>
                    </div>
                    <div class="hidden md:block">
                        <div class="ml-10 flex items-baseline space-x-4">
                            <a href="#" class="bg-gray-800 text-white px-3 py-2 rounded-md text-sm font-medium">Início</a>
                            <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Filmes</a>
                            <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Séries</a>
                            <div class="dropdown relative">
                                <button class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium flex items-center">
                                    Categorias <i class="fas fa-chevron-down ml-1 text-xs"></i>
                                </button>
                                <div class="dropdown-menu absolute hidden bg-gray-800 rounded-md shadow-lg mt-1 py-1 w-48 z-50">
                                    <a href="#" class="block px-4 py-2 text-sm text-gray-300 hover:bg-gray-700">Ação</a>
                                    <a href="#" class="block px-4 py-2 text-sm text-gray-300 hover:bg-gray-700">Comédia</a>
                                    <a href="#" class="block px-4 py-2 text-sm text-gray-300 hover:bg-gray-700">Terror</a>
                                    <a href="#" class="block px-4 py-2 text-sm text-gray-300 hover:bg-gray-700">Drama</a>
                                    <a href="#" class="block px-4 py-2 text-sm text-gray-300 hover:bg-gray-700">Ficção Científica</a>
                                </div>
                            </div>
                            <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white px-3 py-2 rounded-md text-sm font-medium">Favoritos</a>
                        </div>
                    </div>
                </div>
                <div class="hidden md:block">
                    <div class="ml-4 flex items-center md:ml-6">
                        <div class="relative mx-4">
                            <div class="absolute inset-y-0 left-0 pl-3 flex items-center pointer-events-none">
                                <i class="fas fa-search text-gray-400"></i>
                            </div>
                            <input type="text" class="bg-gray-700 text-white rounded-md pl-10 pr-4 py-2 focus:outline-none focus:ring-2 focus:ring-red-500 w-64" placeholder="Buscar filmes...">
                        </div>
                        <button id="theme-toggle" class="p-2 rounded-full text-gray-400 hover:text-white focus:outline-none">
                            <i class="fas fa-moon"></i>
                        </button>
                        <button id="login-btn" class="ml-4 bg-red-600 hover:bg-red-700 text-white px-4 py-2 rounded-md text-sm font-medium">
                            Entrar
                        </button>
                    </div>
                </div>
                <div class="-mr-2 flex md:hidden">
                    <button id="mobile-menu-btn" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-white hover:bg-gray-700 focus:outline-none">
                        <i class="fas fa-bars"></i>
                    </button>
                </div>
            </div>
        </div>
        
        <!-- Mobile menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-gray-900 border-t border-gray-800">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#" class="bg-gray-800 text-white block px-3 py-2 rounded-md text-base font-medium">Início</a>
                <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium">Filmes</a>
                <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium">Séries</a>
                <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium">Categorias</a>
                <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block px-3 py-2 rounded-md text-base font-medium">Favoritos</a>
            </div>
            <div class="pt-4 pb-3 border-t border-gray-800">
                <div class="flex items-center px-5">
                    <div class="relative w-full mx-2">
                        <div class="absolute inset-y-0 left-0 pl-3 flex items-center pointer-events-none">
                            <i class="fas fa-search text-gray-400"></i>
                        </div>
                        <input type="text" class="bg-gray-700 text-white rounded-md pl-10 pr-4 py-2 focus:outline-none focus:ring-2 focus:ring-red-500 w-full" placeholder="Buscar filmes...">
                    </div>
                </div>
                <div class="mt-4 px-2 flex justify-between">
                    <button id="theme-toggle-mobile" class="p-2 rounded-full text-gray-400 hover:text-white focus:outline-none">
                        <i class="fas fa-moon"></i>
                    </button>
                    <button id="login-btn-mobile" class="bg-red-600 hover:bg-red-700 text-white px-4 py-2 rounded-md text-sm font-medium">
                        Entrar
                    </button>
                </div>
            </div>
        </div>
    </nav>

    <!-- Main Content -->
    <main class="pt-20 pb-10">
        <!-- Hero Section -->
        <section class="relative">
            <div class="w-full h-screen max-h-[80vh] bg-gradient-to-r from-gray-900 to-transparent relative overflow-hidden">
                <div class="absolute inset-0 bg-gray-900 opacity-50"></div>
                <img src="https://image.tmdb.org/t/p/original/9dKCd55IuTT5QRs989m9Qlb7d2B.jpg" alt="Duna" class="w-full h-full object-cover">
                <div class="absolute bottom-0 left-0 right-0 bg-gradient-to-t from-gray-900 to-transparent h-1/3"></div>
                <div class="absolute inset-0 flex items-center px-6 md:px-16 lg:px-24">
                    <div class="max-w-2xl z-10">
                        <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-4">Duna: Parte Dois</h1>
                        <div class="flex items-center mb-4">
                            <span class="bg-green-500 text-xs px-2 py-1 rounded mr-2">9.5</span>
                            <span class="text-gray-300 text-sm mr-3">2024</span>
                            <span class="text-gray-300 text-sm">2h 46min</span>
                        </div>
                        <p class="text-gray-300 mb-6">Paul Atreides se une a Chani e aos Fremen enquanto busca vingança contra os conspiradores que destruíram sua família. Enfrentando uma escolha entre o amor de sua vida e o destino do universo, ele deve evitar um futuro terrível que só ele pode prever.</p>
                        <div class="flex space-x-4">
                            <button class="bg-red-600 hover:bg-red-700 text-white px-6 py-2 rounded-md font-medium flex items-center">
                                <i class="fas fa-play mr-2"></i> Assistir
                            </button>
                            <button class="bg-gray-700 hover:bg-gray-600 text-white px-6 py-2 rounded-md font-medium flex items-center">
                                <i class="fas fa-plus mr-2"></i> Minha Lista
                            </button>
                            <button class="bg-gray-700 hover:bg-gray-600 text-white px-4 py-2 rounded-md font-medium flex items-center">
                                <i class="fas fa-users mr-2"></i> Assistir em Grupo
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Content Sections -->
        <div class="container mx-auto px-4 sm:px-6 lg:px-8 mt-8">
            <!-- Netflix Originals -->
            <section class="mb-10">
                <div class="flex justify-between items-center mb-4">
                    <h2 class="text-xl md:text-2xl font-bold flex items-center">
                        <span class="bg-red-600 text-white px-2 mr-3">N</span> Netflix Originals
                    </h2>
                    <a href="#" class="text-gray-400 hover:text-white text-sm">Ver todos</a>
                </div>
                <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 xl:grid-cols-6 gap-4">
                    <!-- Movie Cards -->
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/9PqD3wSIjntyJDBzMNuxuKHwpUD.jpg" alt="Stranger Things" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">Stranger Things</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2016</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/1XDDXPXGiI8g7G4fQJBrQl8v8SJ.jpg" alt="The Witcher" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">The Witcher</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2019</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/34nDCQZwaPs2B4Aim8ShKCr4kFM.jpg" alt="Squid Game" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">Squid Game</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2021</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/7dFZJ2ZJJdcmkp05B9NWlqTJ5tq.jpg" alt="Extraction" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">Extraction</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2020</span>
                                <span class="mx-1">•</span>
                                <span>Filme</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/6XYqxM6Fy8z4p50J5BkEw4qyQEI.jpg" alt="Red Notice" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">Red Notice</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2021</span>
                                <span class="mx-1">•</span>
                                <span>Filme</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/34nDCQZwaPs2B4Aim8ShKCr4kFM.jpg" alt="Money Heist" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">Money Heist</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2017</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- HBO Max Originals -->
            <section class="mb-10">
                <div class="flex justify-between items-center mb-4">
                    <h2 class="text-xl md:text-2xl font-bold flex items-center">
                        <span class="bg-purple-600 text-white px-2 mr-3">H</span> HBO Max Originals
                    </h2>
                    <a href="#" class="text-gray-400 hover:text-white text-sm">Ver todos</a>
                </div>
                <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 xl:grid-cols-6 gap-4">
                    <!-- Movie Cards -->
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/5cnLoWq9o5zLfhyFOwVUfQ9Zy8e.jpg" alt="Game of Thrones" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">Game of Thrones</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2011</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/6UH52Fmau8RPsMAbQbjwN3wJSCj.jpg" alt="The Last of Us" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">The Last of Us</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2023</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/7WsyChQLEftFiDOVTGkv3hFpyyt.jpg" alt="Avengers: Endgame" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">Avengers: Endgame</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2019</span>
                                <span class="mx-1">•</span>
                                <span>Filme</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/8Vt6mWRCeCuplVSkvyUrJqPgfRm.jpg" alt="House of the Dragon" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">House of the Dragon</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2022</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/6f7AR1mcHaLsKGJwmlwjQ9Qr6Dl.jpg" alt="The Batman" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">The Batman</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2022</span>
                                <span class="mx-1">•</span>
                                <span>Filme</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/5cnLoWq9o5zLfhyFOwVUfQ9Zy8e.jpg" alt="Euphoria" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">Euphoria</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2019</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Disney+ Originals -->
            <section class="mb-10">
                <div class="flex justify-between items-center mb-4">
                    <h2 class="text-xl md:text-2xl font-bold flex items-center">
                        <span class="bg-blue-600 text-white px-2 mr-3">D</span> Disney+ Originals
                    </h2>
                    <a href="#" class="text-gray-400 hover:text-white text-sm">Ver todos</a>
                </div>
                <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 xl:grid-cols-6 gap-4">
                    <!-- Movie Cards -->
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/7WsyChQLEftFiDOVTGkv3hFpyyt.jpg" alt="The Mandalorian" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">The Mandalorian</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2019</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/6UH52Fmau8RPsMAbQbjwN3wJSCj.jpg" alt="Loki" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">Loki</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2021</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/8Vt6mWRCeCuplVSkvyUrJqPgfRm.jpg" alt="WandaVision" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">WandaVision</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2021</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/6f7AR1mcHaLsKGJwmlwjQ9Qr6Dl.jpg" alt="The Falcon and the Winter Soldier" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">The Falcon and the Winter Soldier</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2021</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/5cnLoWq9o5zLfhyFOwVUfQ9Zy8e.jpg" alt="Hawkeye" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">Hawkeye</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2021</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/34nDCQZwaPs2B4Aim8ShKCr4kFM.jpg" alt="Moon Knight" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">Moon Knight</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2022</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Prime Video Originals -->
            <section class="mb-10">
                <div class="flex justify-between items-center mb-4">
                    <h2 class="text-xl md:text-2xl font-bold flex items-center">
                        <span class="bg-blue-400 text-white px-2 mr-3">P</span> Prime Video Originals
                    </h2>
                    <a href="#" class="text-gray-400 hover:text-white text-sm">Ver todos</a>
                </div>
                <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 xl:grid-cols-6 gap-4">
                    <!-- Movie Cards -->
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/7WsyChQLEftFiDOVTGkv3hFpyyt.jpg" alt="The Boys" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">The Boys</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2019</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/6UH52Fmau8RPsMAbQbjwN3wJSCj.jpg" alt="The Lord of the Rings: The Rings of Power" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">The Lord of the Rings: The Rings of Power</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2022</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/8Vt6mWRCeCuplVSkvyUrJqPgfRm.jpg" alt="Invincible" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">Invincible</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2021</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/6f7AR1mcHaLsKGJwmlwjQ9Qr6Dl.jpg" alt="The Terminal List" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">The Terminal List</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2022</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/5cnLoWq9o5zLfhyFOwVUfQ9Zy8e.jpg" alt="Reacher" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">Reacher</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2022</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="movie-card relative group">
                        <div class="relative overflow-hidden rounded-lg aspect-[2/3]">
                            <img src="https://image.tmdb.org/t/p/w500/34nDCQZwaPs2B4Aim8ShKCr4kFM.jpg" alt="The Wheel of Time" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                                <button class="play-icon absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-red-600 hover:bg-red-700 text-white rounded-full w-12 h-12 flex items-center justify-center opacity-0 transition-all duration-300">
                                    <i class="fas fa-play"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mt-2">
                            <h3 class="text-sm font-semibold truncate">The Wheel of Time</h3>
                            <div class="flex items-center text-xs text-gray-400">
                                <span>2021</span>
                                <span class="mx-1">•</span>
                                <span>Série</span>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 border-t border-gray-800 py-8">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-lg font-semibold mb-4">Kaua Safado Guloso</h3>
                    <p class="text-gray-400 text-sm">A melhor plataforma para assistir filmes e séries gratuitamente com seus amigos.</p>
                </div>
                <div>
                    <h3 class="text-lg font-semibold mb-4">Links Úteis</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Termos de Serviço</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Política de Privacidade</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">FAQ</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Contato</a></li>
                    </ul>
                </div>
                <div>
                    <h3 class="text-lg font-semibold mb-4">Categorias</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Ação</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Comédia</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Terror</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white text-sm">Drama</a></li>
                    </ul>
                </div>
                <div>
                    <h3 class="text-lg font-semibold mb-4">Redes Sociais</h3>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
            </div>
            <div class="mt-8 pt-8 border-t border-gray-800 text-center text-gray-400 text-sm">
                <p>© 2023 Kaua Safado Guloso. Todos os direitos reservados.</p>
            </div>
        </div>
    </footer>

    <!-- Login Modal -->
    <div id="login-modal" class="fixed inset-0 z-50 hidden overflow-y-auto">
        <div class="flex items-center justify-center min-h-screen pt-4 px-4 pb-20 text-center sm:block sm:p-0">
            <div class="fixed inset-0 transition-opacity" aria-hidden="true">
                <div class="absolute inset-0 bg-gray-900 opacity-75"></div>
            </div>
            <span class="hidden sm:inline-block sm:align-middle sm:h-screen" aria-hidden="true">&#8203;</span>
            <div class="inline-block align-bottom bg-gray-800 rounded-lg text-left overflow-hidden shadow-xl transform transition-all sm:my-8 sm:align-middle sm:max-w-lg sm:w-full">
                <div class="px-4 pt-5 pb-4 sm:p-6 sm:pb-4">
                    <div class="flex justify-between items-start">
                        <h3 class="text-lg leading-6 font-medium text-white mb-4">Entrar no Kaua Safado Guloso</h3>
                        <button id="close-login-modal" class="text-gray-400 hover:text-white">
                            <i class="fas fa-times"></i>
                        </button>
                    </div>
                    <div class="mt-4">
                        <form>
                            <div class="mb-4">
                                <label for="email" class="block text-sm font-medium text-gray-300 mb-1">E-mail</label>
                                <input type="email" id="email" class="bg-gray-700 text-white rounded-md px-3 py-2 w-full focus:outline-none focus:ring-2 focus:ring-red-500">
                            </div>
                            <div class="mb-4">
                                <label for="password" class="block text-sm font-medium text-gray-300 mb-1">Senha</label>
                                <input type="password" id="password" class="bg-gray-700 text-white rounded-md px-3 py-2 w-full focus:outline-none focus:ring-2 focus:ring-red-500">
                            </div>
                            <div class="flex items-center justify-between mb-4">
                                <div class="flex items-center">
                                    <input id="remember-me" type="checkbox" class="h-4 w-4 text-red-600 focus:ring-red-500 border-gray-600 rounded">
                                    <label for="remember-me" class="ml-2 block text-sm text-gray-300">Lembrar de mim</label>
                                </div>
                                <a href="#" class="text-sm text-red-500 hover:text-red-400">Esqueceu a senha?</a>
                            </div>
                            <button type="submit" class="w-full bg-red-600 hover:bg-red-700 text-white py-2 px-4 rounded-md font-medium">Entrar</button>
                        </form>
                        <div class="mt-4 text-center">
                            <p class="text-sm text-gray-400">Não tem uma conta? <a href="#" class="text-red-500 hover:text-red-400">Cadastre-se</a></p>
                        </div>
                        <div class="mt-6">
                            <div class="relative">
                                <div class="absolute inset-0 flex items-center">
                                    <div class="w-full border-t border-gray-600"></div>
                                </div>
                                <div class="relative flex justify-center text-sm">
                                    <span class="px-2 bg-gray-800 text-gray-400">Ou entre com</span>
                                </div>
                            </div>
                            <div class="mt-6 grid grid-cols-2 gap-3">
                                <button type="button" class="w-full inline-flex justify-center py-2 px-4 border border-gray-600 rounded-md shadow-sm bg-gray-700 text-sm font-medium text-white hover:bg-gray-600">
                                    <i class="fab fa-google mr-2"></i> Google
                                </button>
                                <button type="button" class="w-full inline-flex justify-center py-2 px-4 border border-gray-600 rounded-md shadow-sm bg-gray-700 text-sm font-medium text-white hover:bg-gray-600">
                                    <i class="fab fa-facebook-f mr-2"></i> Facebook
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Watch Together Modal -->
    <div id="watch-together-modal" class="fixed inset-0 z-50 hidden overflow-y-auto">
        <div class="flex items-center justify-center min-h-screen pt-4 px-4 pb-20 text-center sm:block sm:p-0">
            <div class="fixed inset-0 transition-opacity" aria-hidden="true">
                <div class="absolute inset-0 bg-gray-900 opacity-75"></div>
            </div>
            <span class="hidden sm:inline-block sm:align-middle sm:h-screen" aria-hidden="true">&#8203;</span>
            <div class="inline-block align-bottom bg-gray-800 rounded-lg text-left overflow-hidden shadow-xl transform transition-all sm:my-8 sm:align-middle sm:max-w-lg sm:w-full">
                <div class="px-4 pt-5 pb-4 sm:p-6 sm:pb-4">
                    <div class="flex justify-between items-start">
                        <h3 class="text-lg leading-6 font-medium text-white mb-4">Assistir em Grupo</h3>
                        <button id="close-watch-together-modal" class="text-gray-400 hover:text-white">
                            <i class="fas fa-times"></i>
                        </button>
                    </div>
                    <div class="mt-4">
                        <p class="text-gray-300 mb-4">Crie uma sessão para assistir com seus amigos. Compartilhe o link abaixo para convidá-los.</p>
                        <div class="mb-4">
                            <label for="watch-together-link" class="block text-sm font-medium text-gray-300 mb-1">Link de convite</label>
                            <div class="flex">
                                <input type="text" id="watch-together-link" value="https://kauasafadoguloso.com/watch/abc123" class="bg-gray-700 text-white rounded-l-md px-3 py-2 w-full focus:outline-none focus:ring-2 focus:ring-red-500" readonly>
                                <button id="copy-link" class="bg-red-600 hover:bg-red-700 text-white px-4 py-2 rounded-r-md font-medium">
                                    <i class="fas fa-copy"></i>
                                </button>
                            </div>
                        </div>
                        <div class="mb-4">
                            <label class="block text-sm font-medium text-gray-300 mb-2">Amigos online</label>
                            <div class="bg-gray-700 rounded-md p-3 max-h-40 overflow-y-auto">
                                <div class="flex items-center justify-between py-2">
                                    <div class="flex items-center">
                                        <div class="h-8 w-8 rounded-full bg-red-500 flex items-center justify-center text-white font-bold mr-3">J</div>
                                        <span class="text-gray-300">João</span>
                                    </div>
                                    <button class="text-red-500 hover:text-red-400 text-sm font-medium">Convidar</button>
                                </div>
                                <div class="flex items-center justify-between py-2">
                                    <div class="flex items-center">
                                        <div class="h-8 w-8 rounded-full bg-blue-500 flex items-center justify-center text-white font-bold mr-3">M</div>
                                        <span class="text-gray-300">Maria</span>
                                    </div>
                                    <button class="text-red-500 hover:text-red-400 text-sm font-medium">Convidar</button>
                                </div>
                                <div class="flex items-center justify-between py-2">
                                    <div class="flex items-center">
                                        <div class="h-8 w-8 rounded-full bg-green-500 flex items-center justify-center text-white font-bold mr-3">P</div>
                                        <span class="text-gray-300">Pedro</span>
                                    </div>
                                    <button class="text-red-500 hover:text-red-400 text-sm font-medium">Convidar</button>
                                </div>
                            </div>
                        </div>
                        <button class="w-full bg-red-600 hover:bg-red-700 text-white py-2 px-4 rounded-md font-medium">Iniciar Sessão</button>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Mobile menu toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        
        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // Theme toggle
        const themeToggle = document.getElementById('theme-toggle');
        const themeToggleMobile = document.getElementById('theme-toggle-mobile');
        
        function toggleTheme() {
            const html = document.documentElement;
            if (html.classList.contains('dark')) {
                html.classList.remove('dark');
                localStorage.setItem('theme', 'light');
                themeToggle.innerHTML = '<i class="fas fa-sun"></i>';
                themeToggleMobile.innerHTML = '<i class="fas fa-sun"></i>';
            } else {
                html.classList.add('dark');
                localStorage.setItem('theme', 'dark');
                themeToggle.innerHTML = '<i class="fas fa-moon"></i>';
                themeToggleMobile.innerHTML = '<i class="fas fa-moon"></i>';
            }
        }
        
        themeToggle.addEventListener('click', toggleTheme);
        themeToggleMobile.addEventListener('click', toggleTheme);
        
        // Check for saved theme preference
        if (localStorage.getItem('theme') === 'light') {
            document.documentElement.classList.remove('dark');
            themeToggle.innerHTML = '<i class="fas fa-sun"></i>';
            themeToggleMobile.innerHTML = '<i class="fas fa-sun"></i>';
        }
        
        // Login modal
        const loginBtn = document.getElementById('login-btn');
        const loginBtnMobile = document.getElementById('login-btn-mobile');
        const loginModal = document.getElementById('login-modal');
        const closeLoginModal = document.getElementById('close-login-modal');
        
        function openLoginModal() {
            loginModal.classList.remove('hidden');
        }
        
        function closeLoginModalFunc() {
            loginModal.classList.add('hidden');
        }
        
        loginBtn.addEventListener('click', openLoginModal);
        loginBtnMobile.addEventListener('click', openLoginModal);
        closeLoginModal.addEventListener('click', closeLoginModalFunc);
        
        // Watch together modal
        const watchTogetherModal = document.getElementById('watch-together-modal');
        const closeWatchTogetherModal = document.getElementById('close-watch-together-modal');
        const copyLinkBtn = document.getElementById('copy-link');
        
        // This would be connected to actual "Watch Together" buttons
        function openWatchTogetherModal() {
            watchTogetherModal.classList.remove('hidden');
        }
        
        function closeWatchTogetherModalFunc() {
            watchTogetherModal.classList.add('hidden');
        }
        
        closeWatchTogetherModal.addEventListener('click', closeWatchTogetherModalFunc);
        
        copyLinkBtn.addEventListener('click', () => {
            const linkInput = document.getElementById('watch-together-link');
            linkInput.select();
            document.execCommand('copy');
            
            // Show copied feedback
            const originalText = copyLinkBtn.innerHTML;
            copyLinkBtn.innerHTML = '<i class="fas fa-check"></i> Copiado!';
            setTimeout(() => {
                copyLinkBtn.innerHTML = originalText;
            }, 2000);
        });
        
        // Simulate clicking on a "Watch Together" button
        document.querySelectorAll('.movie-card .play-icon').forEach(button => {
            button.addEventListener('click', () => {
                openWatchTogetherModal();
            });
        });
        
        // Simulate clicking on the "Assistir em Grupo" button in hero section
        document.querySelector('.bg-gray-700.hover\\:bg-gray-600.flex.items-center').addEventListener('click', (e) => {
            e.preventDefault();
            openWatchTogetherModal();
        });
        
        // Movie card hover effect
        document.querySelectorAll('.movie-card').forEach(card => {
            card.addEventListener('mouseenter', () => {
                const playIcon = card.querySelector('.play-icon');
                playIcon.style.opacity = '1';
                playIcon.style.transform = 'translate(-50%, -50%) scale(1)';
            });
            
            card.addEventListener('mouseleave', () => {
                const playIcon = card.querySelector('.play-icon');
                playIcon.style.opacity = '0';
                playIcon.style.transform = 'translate(-50%, -50%) scale(0.5)';
            });
        });
    </script>
</body>
</html>
