<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jamie Toft - Photography</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
      @font-face {
        font-family: 'LucideIcons';
        src: url(https://cdn.jsdelivr.net/npm/lucide-static@latest/font/Lucide.ttf) format('truetype');
      }
      .lucide {
        font-family: 'LucideIcons';
        font-size: 1.25rem; /* Adjust size as needed */
        line-height: 1;
      }
      /* Basic body styling */
      body {
        font-family: 'Inter', sans-serif;
        background-color: #111827; /* Dark background like the reference */
        color: #e5e7eb; /* Light text color */
      }
      /* Simple smooth scroll */
      html {
        scroll-behavior: smooth;
      }
      /* Style for active nav link */
      .nav-active {
        font-weight: 600;
        color: #ffffff;
      }
      /* Style for gallery hover effect */
      .gallery-item:hover .overlay {
        opacity: 1;
      }
    </style>
</head>
<body class="bg-gray-900 text-gray-200">

    <header class="sticky top-0 z-50 bg-gray-900 bg-opacity-90 backdrop-blur-sm">
        <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-2xl font-bold text-white hover:text-gray-300 transition duration-300">Jamie Toft Photography</a>

            <ul class="hidden md:flex space-x-6 items-center">
                <li><a href="#home" class="hover:text-white transition duration-300 nav-active">Home</a></li>
                <li><a href="#portfolio" class="hover:text-white transition duration-300">Portfolio</a></li>
                <li><a href="#about" class="hover:text-white transition duration-300">About</a></li>
                <li><a href="#contact" class="hover:text-white transition duration-300">Contact</a></li>
            </ul>

            <button id="mobile-menu-button" class="md:hidden focus:outline-none">
                <span class="lucide">&#xe96d;</span> </button>
        </nav>

        <div id="mobile-menu" class="hidden md:hidden bg-gray-800">
            <ul class="flex flex-col items-center py-4 space-y-2">
                <li><a href="#home" class="block px-4 py-2 hover:bg-gray-700 rounded nav-active">Home</a></li>
                <li><a href="#portfolio" class="block px-4 py-2 hover:bg-gray-700 rounded">Portfolio</a></li>
                <li><a href="#about" class="block px-4 py-2 hover:bg-gray-700 rounded">About</a></li>
                <li><a href="#contact" class="block px-4 py-2 hover:bg-gray-700 rounded">Contact</a></li>
            </ul>
        </div>
    </header>

    <main>
        <section id="home" class="relative h-screen flex items-center justify-center text-center bg-gray-800">
            <div class="absolute inset-0 bg-black opacity-50 z-0">
                 <img src="https://photos.google.com/photo/AF1QipM6bvpNC4h6Bfkt9QaFyGYd9AB0eTRr2mO_UGk"
                      alt="Placeholder hero image"
                      class="w-full h-full object-cover"
                      onerror="this.onerror=null; this.src='https://placehold.co/1920x1080/2d3748/e2e8f0?text=Image+Error';">
            </div>
            <div class="relative z-10 px-6">
                <h1 class="text-4xl md:text-6xl font-bold text-white mb-4">Capturing Moments, Creating Memories</h1>
                <p class="text-lg md:text-xl text-gray-300 mb-8">Specializing in [Your Photography Niche - e.g., Portraits, Landscapes, Events]</p>
                <a href="#portfolio" class="bg-indigo-600 hover:bg-indigo-700 text-white font-semibold py-3 px-8 rounded-lg transition duration-300">View My Work</a>
            </div>
        </section>

        <section id="portfolio" class="py-16 md:py-24 bg-gray-900">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl md:text-4xl font-bold text-center mb-12">Portfolio</h2>
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 md:gap-8">
                    <div class="relative group aspect-square rounded-lg overflow-hidden shadow-lg gallery-item">
                        <img src="https://placehold.co/600x600/4a5568/e2e8f0?text=Portfolio+1"
                             alt="Portfolio image 1"
                             class="w-full h-full object-cover transition-transform duration-300 group-hover:scale-105"
                             onerror="this.onerror=null; this.src='https://placehold.co/600x600/4a5568/e2e8f0?text=Image+Error';">
                        <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity duration-300 overlay">
                            <p class="text-white text-lg font-semibold">Project Title 1</p>
                        </div>
                    </div>
                    <div class="relative group aspect-square rounded-lg overflow-hidden shadow-lg gallery-item">
                        <img src="https://placehold.co/600x600/718096/e2e8f0?text=Portfolio+2"
                             alt="Portfolio image 2"
                             class="w-full h-full object-cover transition-transform duration-300 group-hover:scale-105"
                             onerror="this.onerror=null; this.src='https://placehold.co/600x600/718096/e2e8f0?text=Image+Error';">
                        <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity duration-300 overlay">
                            <p class="text-white text-lg font-semibold">Project Title 2</p>
                        </div>
                    </div>
                    <div class="relative group aspect-square rounded-lg overflow-hidden shadow-lg gallery-item">
                        <img src="https://placehold.co/600x600/a0aec0/1a202c?text=Portfolio+3"
                             alt="Portfolio image 3"
                             class="w-full h-full object-cover transition-transform duration-300 group-hover:scale-105"
                             onerror="this.onerror=null; this.src='https://placehold.co/600x600/a0aec0/1a202c?text=Image+Error';">
                        <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity duration-300 overlay">
                            <p class="text-white text-lg font-semibold">Project Title 3</p>
                        </div>
                    </div>
                    <div class="relative group aspect-square rounded-lg overflow-hidden shadow-lg gallery-item">
                        <img src="https://placehold.co/600x600/4a5568/e2e8f0?text=Portfolio+4"
                             alt="Portfolio image 4"
                             class="w-full h-full object-cover transition-transform duration-300 group-hover:scale-105"
                             onerror="this.onerror=null; this.src='https://placehold.co/600x600/4a5568/e2e8f0?text=Image+Error';">
                        <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity duration-300 overlay">
                            <p class="text-white text-lg font-semibold">Project Title 4</p>
                        </div>
                    </div>
                     <div class="relative group aspect-square rounded-lg overflow-hidden shadow-lg gallery-item">
                        <img src="https://placehold.co/600x600/718096/e2e8f0?text=Portfolio+5"
                             alt="Portfolio image 5"
                             class="w-full h-full object-cover transition-transform duration-300 group-hover:scale-105"
                             onerror="this.onerror=null; this.src='https://placehold.co/600x600/718096/e2e8f0?text=Image+Error';">
                        <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity duration-300 overlay">
                            <p class="text-white text-lg font-semibold">Project Title 5</p>
                        </div>
                    </div>
                     <div class="relative group aspect-square rounded-lg overflow-hidden shadow-lg gallery-item">
                        <img src="https://placehold.co/600x600/a0aec0/1a202c?text=Portfolio+6"
                             alt="Portfolio image 6"
                             class="w-full h-full object-cover transition-transform duration-300 group-hover:scale-105"
                             onerror="this.onerror=null; this.src='https://placehold.co/600x600/a0aec0/1a202c?text=Image+Error';">
                        <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity duration-300 overlay">
                            <p class="text-white text-lg font-semibold">Project Title 6</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="about" class="py-16 md:py-24 bg-gray-800">
            <div class="container mx-auto px-6 flex flex-col md:flex-row items-center gap-12">
                <div class="md:w-1/3">
                    <img src="https://placehold.co/400x400/2d3748/e2e8f0?text=Your+Portrait"
                         alt="Your portrait placeholder"
                         class="rounded-full shadow-lg mx-auto"
                         onerror="this.onerror=null; this.src='https://placehold.co/400x400/2d3748/e2e8f0?text=Image+Error';">
                </div>
                <div class="md:w-2/3 text-center md:text-left">
                    <h2 class="text-3xl md:text-4xl font-bold mb-6">About Me</h2>
                    <p class="text-lg text-gray-300 mb-4">
                        Hi, I'm [Your Name], a passionate photographer based in [Your Location]. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                    </p>
                    <p class="text-lg text-gray-300">
                        Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                    </p>
                    </div>
            </div>
        </section>

        <section id="contact" class="py-16 md:py-24 bg-gray-900">
            <div class="container mx-auto px-6 max-w-3xl text-center">
                <h2 class="text-3xl md:text-4xl font-bold mb-8">Get In Touch</h2>
                <p class="text-lg text-gray-300 mb-10">
                    Have a project in mind or just want to say hello? Feel free to reach out!
                </p>
                <div class="space-y-4">
                     <p class="text-lg"><span class="font-semibold">Email:</span> <a href="mailto:your.email@example.com" class="text-indigo-400 hover:text-indigo-300">your.email@example.com</a></p>
                     <p class="text-lg"><span class="font-semibold">Phone:</span> (Optional) +1 234 567 890</p>
                     <div class="flex justify-center space-x-6 pt-4">
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300" aria-label="Instagram">
                            <span class="lucide">&#xea0a;</span> </a>
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300" aria-label="Twitter">
                             <span class="lucide">&#xea8b;</span> </a>
                         <a href="#" class="text-gray-400 hover:text-white transition duration-300" aria-label="Facebook">
                             <span class="lucide">&#xe93b;</span> </a>
                     </div>
                </div>
                 </div>
        </section>
    </main>

    <footer class="bg-gray-800 py-8">
        <div class="container mx-auto px-6 text-center text-gray-400">
            <div class="flex justify-center space-x-6 mb-4">
                <a href="#" class="hover:text-white transition duration-300" aria-label="Instagram">
                    <span class="lucide">&#xea0a;</span>
                </a>
                <a href="#" class="hover:text-white transition duration-300" aria-label="Twitter">
                     <span class="lucide">&#xea8b;</span>
                </a>
                 <a href="#" class="hover:text-white transition duration-300" aria-label="Facebook">
                     <span class="lucide">&#xe93b;</span>
                </a>
             </div>
            <p>&copy; <span id="current-year"></span> Your Name Photography. All rights reserved.</p>
            <p class="text-sm mt-2">Website template inspired by jasonvong.com</p>
        </div>
    </footer>

    <script>
        const menuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');
        const menuIcon = menuButton.querySelector('.lucide'); // Get the icon span

        menuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
            // Toggle between menu and close icons (optional)
            if (mobileMenu.classList.contains('hidden')) {
                 menuIcon.innerHTML = '&#xe96d;'; // Menu icon code
            } else {
                 menuIcon.innerHTML = '&#xe9b0;'; // Close icon code (X)
            }
        });

        // Close mobile menu when a link is clicked (optional)
        const mobileLinks = mobileMenu.querySelectorAll('a');
        mobileLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
                menuIcon.innerHTML = '&#xe96d;'; // Reset to menu icon
            });
        });

        // Set current year in footer
        document.getElementById('current-year').textContent = new Date().getFullYear();

        // Simple Active Nav Link Highlighting on Scroll (Basic Implementation)
        const sections = document.querySelectorAll('main section[id]');
        const navLinks = document.querySelectorAll('header nav a');
        const mobileNavLinks = document.querySelectorAll('#mobile-menu a');

        window.addEventListener('scroll', () => {
            let current = '';
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                // Adjust offset as needed based on sticky header height
                const sectionHeight = section.clientHeight;
                 if (pageYOffset >= (sectionTop - 100)) { // 100px offset
                    current = section.getAttribute('id');
                }
            });

             // Function to update active class
            const updateActiveClass = (links) => {
                links.forEach(link => {
                    link.classList.remove('nav-active');
                    if (link.getAttribute('href') === `#${current}`) {
                        link.classList.add('nav-active');
                    }
                    // Handle home separately if no section is active near the top
                    if (!current && link.getAttribute('href') === '#home') {
                         link.classList.add('nav-active');
                    }
                });
            };

            updateActiveClass(navLinks);
            updateActiveClass(mobileNavLinks);
        });

    </script>

</body>
</html>
