<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>This is my website so hello</title>
    <!-- Load Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Configure custom colors and font -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'primary-dark': '#4F46E5', // Indigo-600
                        'primary-light': '#93C5FD', // Sky-300
                        'bg-light': '#F3F4F6', // Gray-100
                        'text-dark': '#1F2937', // Gray-800
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style>
        /* Custom styles for the interactive element (minimal) */
        .qa-answer {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-in-out, padding 0.3s ease-in-out;
        }
        .qa-answer.open {
            max-height: 200px; /* Adjust height based on content */
            padding-top: 0.75rem;
            padding-bottom: 0.75rem;
        }
        .qa-question:hover {
            cursor: pointer;
        }
    </style>
</head>
<body class="bg-bg-light font-sans text-text-dark min-h-screen flex flex-col">

   
    <header class="sticky top-0 z-10 bg-primary-dark shadow-xl">
        <div class="container mx-auto px-4 py-4 flex justify-between items-center">
         
            <div class="flex items-center space-x-2">
                
                <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-white" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                    <path d="M4 17l4-4 4 4M20 7l-4 4-4-4"/>
                    <path d="M12 19V5"/>
                </svg>
                <span class="text-2xl font-extrabold text-white">My Space</span>
            </div>
            
            
            <nav class="hidden md:flex space-x-8 text-white text-lg font-medium">
                <a href="#about" class="hover:text-primary-light transition duration-200">About Me</a>
                <a href="#projects" class="hover:text-primary-light transition duration-200">Projects</a>
                <a href="#interests" class="hover:text-primary-light transition duration-200">Interests</a>
                <a href="#contact" class="hover:text-primary-light transition duration-200">Connect</a>
            </nav>
            
            
            <div class="md:hidden">
                <button class="text-white focus:outline-none">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
                </button>
            </div>
        </div>
    </header>

   
    <main class="flex-grow container mx-auto px-4 py-12">
        
        <!-- Hero/Intro Section Container -->
        <section id="about" class="mb-16 p-8 bg-white shadow-2xl rounded-xl border-l-8 border-primary-dark md:flex items-center">
            
            <!-- Text Content Container -->
            <div class="md:w-3/4">
                <h1 class="text-5xl font-extrabold text-primary-dark mb-4">Hello! I'm rohan the goat.</h1>
                <p class="text-xl text-gray-600 mb-6">I'm a high school student learning about design, coding, and the world around me. Welcome to my home.</p>
                <a href="#projects" class="inline-block bg-primary-dark text-white font-semibold py-3 px-6 rounded-full shadow-lg hover:bg-indigo-700 transition duration-300">
                    See My Latest Work
                </a>
            </div>

            <!-- Profile Image Placeholder (Using a simple SVG for compliance) -->
            <div class="hidden md:block md:w-1/4 p-4 text-center">
                <svg xmlns="http://www.w3.org/2000/svg" class="w-32 h-32 mx-auto text-primary-light" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round">
                    <path d="M19 21v-2a4 4 0 0 0-4-4H9a4 4 0 0 0-4 4v2"></path>
                    <circle cx="12" cy="7" r="4"></circle>
                </svg>
                <p class="mt-2 text-sm text-gray-500">Profile Placeholder</p>
            </div>
        </section>

       
        <section id="projects" class="mb-16">
            <h2 class="text-4xl font-extrabold text-text-dark mb-8 border-b-4 border-primary-light pb-2">What the goat has created:</h2>
            
            <div class="grid md:grid-cols-3 gap-8">

                
                <div class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition duration-300 border-t-4 border-sky-400">
                    <h3 class="text-2xl font-bold mb-3 text-primary-dark">Baby goat creation</h3>
                    <p class="text-gray-700">A simple text-based adventure game built to learn basic programming logic and loops. Planning to add graphics next!</p>
                    <a href="#" class="text-sky-500 hover:text-sky-700 font-semibold mt-3 inline-block text-sm">View Details &rarr;</a>
                </div>

                <!-- Project Card 2 Container -->
                <div class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition duration-300 border-t-4 border-sky-400">
                    <h3 class="text-2xl font-bold mb-3 text-primary-dark">Extensive goat creation</h3>
                    <p class="text-gray-700">Research project on the oldest building in my town. Used primary sources to trace its history back 100 years. Great for my history class!</p>
                    <a href="#" class="text-sky-500 hover:text-sky-700 font-semibold mt-3 inline-block text-sm">View Details &rarr;</a>
                </div>

               
                <div class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition duration-300 border-t-4 border-sky-400">
                    <h3 class="text-2xl font-bold mb-3 text-primary-dark">Volunteer App Design</h3>
                    <p class="text-gray-700">A concept for a mobile app connecting student volunteers with local community opportunities. Designed the wireframes and user flow.</p>
                    <a href="#" class="text-sky-500 hover:text-sky-700 font-semibold mt-3 inline-block text-sm">View Details &rarr;</a>
                </div>
            </div>
        </section>
        
        <!-- Feature 2: Interactive Interests Q&A Section Container (Accordion) -->
        <section id="interests" class="mb-16 p-8 bg-white shadow-xl rounded-2xl">
            <h2 class="text-4xl font-extrabold text-text-dark mb-6 border-b pb-2">My Interests Q&A</h2>

            <!-- Q&A Item 1 Container -->
            <div class="mb-4 border-b border-gray-200">
                <button class="qa-question w-full flex justify-between items-center py-4 text-left font-semibold text-lg text-text-dark hover:text-primary-dark transition duration-200">
                    <span>What's your favorite school subject?</span>
                    <span class="qa-icon text-2xl font-light text-primary-dark">+</span>
                </button>
                <div class="qa-answer bg-bg-light rounded-b-lg px-4 text-gray-700">
                    <p>I really enjoy **Computer Science** because it feels like solving puzzles all day. I'm currently working through online courses on web development!</p>
                </div>
            </div>

            <!-- Q&A Item 2 Container -->
            <div class="mb-4 border-b border-gray-200">
                <button class="qa-question w-full flex justify-between items-center py-4 text-left font-semibold text-lg text-text-dark hover:text-primary-dark transition duration-200">
                    <span>What do you do in your free time?</span>
                    <span class="qa-icon text-2xl font-light text-primary-dark">+</span>
                </button>
                <div class="qa-answer bg-bg-light rounded-b-lg px-4 text-gray-700">
                    <p>I love reading science fiction and fantasy books! I'm also teaching myself guitar, which is a lot of fun but definitely takes practice.</p>
                </div>
            </div>

            <!-- Q&A Item 3 Container -->
            <div class="mb-4">
                <button class="qa-question w-full flex justify-between items-center py-4 text-left font-semibold text-lg text-text-dark hover:text-primary-dark transition duration-200">
                    <span>What's your biggest goal this year?</span>
                    <span class="qa-icon text-2xl font-light text-primary-dark">+</span>
                </button>
                <div class="qa-answer bg-bg-light rounded-b-lg px-4 text-gray-700">
                    <p>My biggest goal is to finish building a fully functional budgeting tool using HTML, CSS, and JavaScript before the end of the school year.</p>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer Container -->
    <footer id="contact" class="bg-primary-dark text-white py-8 mt-auto">
        <div class="container mx-auto px-4 text-center">
            <p class="mb-4">&copy; Personal Website. Designed with Tailwind CSS.</p>
            
            <!-- Contact/Social Container -->
            <div class="flex justify-center space-x-6 text-2xl">
                <!-- Placeholder Icons for Contact -->
                <a href="#" class="hover:text-primary-light transition duration-200" title="Email Placeholder"></a>
                <a href="#" class="hover:text-primary-light transition duration-200" title="GitHub Placeholder"></a>
                <a href="#" class="hover:text-primary-light transition duration-200" title="Social Media Placeholder"></a>
            </div>
        </div>
    </footer>

    <!-- Minimal JavaScript for Q&A Toggle -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const qaButtons = document.querySelectorAll('.qa-question');

            qaButtons.forEach(button => {
                button.addEventListener('click', () => {
                    // Find the answer and icon corresponding to the clicked button
                    const answer = button.nextElementSibling;
                    const icon = button.querySelector('.qa-icon');

                    // Close all other open answers
                    qaButtons.forEach(otherButton => {
                        if (otherButton !== button) {
                            const otherAnswer = otherButton.nextElementSibling;
                            const otherIcon = otherButton.querySelector('.qa-icon');
                            if (otherAnswer.classList.contains('open')) {
                                otherAnswer.classList.remove('open');
                                otherIcon.textContent = '+';
                            }
                        }
                    });

                    // Toggle the clicked answer
                    if (answer.classList.contains('open')) {
                        answer.classList.remove('open');
                        icon.textContent = '+';
                    } else {
                        answer.classList.add('open');
                        icon.textContent = '-';
                    }
                });
            });
        });
    </script>
</body>
</html>
