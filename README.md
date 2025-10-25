<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valetudeo - Excellence in Health. Compassion for Life.</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/alpinejs@3.x.x/dist/cdn.min.js" defer></script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
        }
        .section-title {
            @apply text-3xl md:text-5xl font-extrabold text-gray-900 mb-4 text-center;
        }
        .section-subtitle {
            @apply text-lg text-gray-600 mb-12 text-center max-w-3xl mx-auto;
        }
        .cta-button {
            @apply px-8 py-4 bg-blue-600 text-white font-bold rounded-lg shadow-lg hover:bg-blue-700 transition-all transform hover:scale-105 duration-300;
        }
        .feature-card {
             @apply bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl hover:-translate-y-2 transition-all duration-300;
        }
    </style>
</head>
<body class="bg-gray-50">

    <!-- Header -->
    <header class="bg-white shadow-md sticky top-0 z-50" x-data="{ open: false }">
        <div class="container mx-auto px-6 py-4">
            <div class="flex items-center justify-between">
                <div class="flex items-center">
                    <svg class="w-10 h-10 text-blue-600 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M21 12.792V21a1 1 0 01-1 1H4a1 1 0 01-1-1V5a1 1 0 011-1h8.208M15 3h6v6M11 13L21 3"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M12 4.5v3m-1.5 0h3"></path></svg>
                    <a href="#" class="text-2xl font-bold text-gray-800">Valetudeo</a>
                </div>
                <nav class="hidden md:flex space-x-6 items-center">
                    <a href="#about" class="text-gray-600 hover:text-blue-600 transition">About Us</a>
                    <a href="#services" class="text-gray-600 hover:text-blue-600 transition">Specialities</a>
                    <a href="#find-doctor" class="text-gray-600 hover:text-blue-600 transition">Find a Doctor</a>
                    <a href="#pharmacy" class="text-gray-600 hover:text-blue-600 transition">Pharmacy</a>
                     <a href="#nursing" class="text-gray-600 hover:text-blue-600 transition">Nursing</a>
                    <a href="#contact" class="px-6 py-2 bg-blue-600 text-white rounded-full font-semibold hover:bg-blue-700 transition">Book Appointment</a>
                </nav>
                <button @click="open = !open" class="md:hidden text-gray-700 focus:outline-none">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
                </button>
            </div>
            <!-- Mobile Menu -->
            <div x-show="open" @click.away="open = false" class="md:hidden mt-4">
                 <a href="#about" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-100 rounded">About Us</a>
                 <a href="#services" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-100 rounded">Specialities</a>
                 <a href="#find-doctor" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-100 rounded">Find a Doctor</a>
                 <a href="#pharmacy" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-100 rounded">Pharmacy</a>
                 <a href="#nursing" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-100 rounded">Nursing</a>
                 <a href="#international-patients" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-100 rounded">International Patients</a>
                 <a href="#contact" class="block mt-2 py-2 px-4 text-sm text-center bg-blue-600 text-white rounded-full font-semibold hover:bg-blue-700 transition">Book Appointment</a>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="relative h-[90vh] bg-cover bg-center" style="background-image: url('https://images.unsplash.com/photo-1581091226825-a6a2a5aee158?q=80&w=2070&auto=format&fit=crop');">
        <div class="absolute inset-0 bg-black opacity-60"></div>
        <div class="relative z-10 flex flex-col items-center justify-center h-full text-white text-center px-4">
            <h1 class="text-4xl md:text-7xl font-extrabold leading-tight mb-4">Excellence in Health. Compassion for Life.</h1>
            <p class="text-lg md:text-2xl max-w-4xl mb-8">Fusing AI-driven diagnostics, robotic surgery, and groundbreaking research to redefine global healthcare.</p>
            <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4">
                <a href="#contact" class="cta-button">Request a Consultation</a>
                <a href="#find-doctor" class="px-8 py-4 bg-white text-blue-600 font-bold rounded-lg shadow-lg hover:bg-gray-100 transition-all transform hover:scale-105 duration-300">Find Your Specialist</a>
            </div>
        </div>
    </section>

    <!-- Mission, Vision, Values Section -->
    <section id="mission" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <h2 class="section-title">Our Guiding Philosophy</h2>
            <p class="section-subtitle">Our motto, "Excellence in Health. Compassion for Life," is the bedrock of our institution. It represents our unwavering commitment to pushing the boundaries of medical science while providing deeply human, empathetic care to every person we serve.</p>
            <div class="grid md:grid-cols-3 gap-8 text-left">
                <div class="feature-card">
                    <h3 class="text-2xl font-bold text-blue-600 mb-4">Our Mission</h3>
                    <p class="text-gray-600">To deliver globally accessible, world-class healthcare by integrating advanced medical treatments with a profound sense of compassion. We strive to create a healing ecosystem where every patient feels valued, every treatment is evidence-based, and every outcome contributes to a healthier global community, especially in underserved regions.</p>
                </div>
                <div class="feature-card">
                    <h3 class="text-2xl font-bold text-blue-600 mb-4">Our Vision</h3>
                    <p class="text-gray-600">To be the world's most trusted healthcare institution, recognized for setting new standards in clinical excellence, medical research, and patient-centric care. We aim to build a legacy of health and hope that transcends borders, making superior healthcare a reality for all, not a privilege for few.</p>
                </div>
                <div class="feature-card">
                    <h3 class="text-2xl font-bold text-blue-600 mb-4">Our Core Values</h3>
                    <ul class="text-gray-600 space-y-2">
                        <li><span class="font-semibold">Integrity:</span> Upholding the highest ethical standards.</li>
                        <li><span class="font-semibold">Innovation:</span> Relentlessly pursuing medical breakthroughs.</li>
                        <li><span class="font-semibold">Empathy:</span> Treating every individual with dignity and kindness.</li>
                        <li><span class="font-semibold">Collaboration:</span> Working as one team for the benefit of our patients.</li>
                        <li><span class="font-semibold">Excellence:</span> Striving for the best in all that we do.</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Leadership Section -->
    <section id="about" class="py-20 bg-gray-100">
        <div class="container mx-auto px-6">
            <h2 class="section-title">Visionary Leadership: The Architects of Valetudeo</h2>
            <p class="section-subtitle">Valetudeo was founded on the combined vision of two extraordinary leaders—a pioneering surgeon and a master of pharmaceutical science—united by a common goal to revolutionize global health.</p>
            <div class="grid lg:grid-cols-2 gap-12 items-center">
                <div class="bg-white p-8 rounded-xl shadow-2xl text-center lg:text-left">
                    <img src="https://placehold.co/250x250/BDBDBD/FFFFFF?text=Dr.+Siham+D.+Hassan" alt="Dr. Siham Deq Hassan" class="w-48 h-48 mx-auto lg:mx-0 rounded-full border-4 border-blue-300 shadow-lg mb-6">
                    <h3 class="text-4xl font-bold text-gray-800">Dr. Siham Deq Hassan</h3>
                    <p class="text-blue-600 font-semibold text-xl mt-1">Founder & Chief Surgeon, Valetudeo Hospital</p>
                    <p class="text-gray-500 mt-1">Registered Medical Doctor, Surgeon & Board-Certified Physician</p>
                    <p class="text-gray-600 mt-4">Dr. Hassan is the clinical heart of Valetudeo. A highly respected, board-certified surgeon and physician, her vision was to create a hospital where surgical excellence and clinical innovation were not just ideals, but everyday realities. She leads our multispecialty surgical teams, championing the adoption of minimally invasive techniques and robotic surgery. Her hands-on approach ensures that every patient benefits from the most effective and safest treatment protocols, personally overseeing the synergy between our surgical departments and our research partners to turn scientific discovery into life-saving practice.</p>
                </div>
                <div class="bg-white p-8 rounded-xl shadow-2xl text-center lg:text-left">
                    <img src="https://placehold.co/250x250/BDBDBD/FFFFFF?text=Dr.+Abdullahi+Bain+Oduwo" alt="Dr. Abdullahi Bain Oduwo" class="w-48 h-48 mx-auto lg:mx-0 rounded-full border-4 border-blue-300 shadow-lg mb-6">
                    <h3 class="text-4xl font-bold text-gray-800">Dr. Abdullahi Bain Oduwo</h3>
                    <p class="text-blue-600 font-semibold text-xl mt-1">Chief Research Partner & Founder, DrugD</p>
                    <p class="text-gray-500 mt-1">Doctor & Professor of Drugs, PhD in Pharmaceutics</p>
                    <p class="text-gray-600 mt-4">Dr. Oduwo is the scientific mind driving our therapeutic advancements. As a distinguished medical researcher with a PhD and post-doctorate in Pharmaceutics, he is an authority on the molecular mechanisms of disease. His expertise spans oncology, chronic diseases, virology, and antibiotics. Through our exclusive partnership with his firm, DrugD, Dr. Oduwo guides our holistic treatment philosophy, integrating cutting-edge pharmaceuticals with personalized supplements and evidence-based dietary plans. His work ensures Valetudeo's treatments are not only powerful but also precisely tailored to each patient's unique biological makeup.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Our Medical Specialities Section -->
    <section id="services" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <h2 class="section-title">Our Comprehensive Medical Specialities</h2>
            <p class="section-subtitle">Valetudeo is a fully integrated, multispecialty hospital offering a complete spectrum of medical and surgical care under one roof.</p>
            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
                
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-red-100 text-red-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Cardiology</h4>
                </div>
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-blue-100 text-blue-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14.828 14.828a4 4 0 01-5.656 0M9 10h.01M15 10h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Neurology & Neurosurgery</h4>
                </div>
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-purple-100 text-purple-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15.232 5.232l3.536 3.536m-2.036-5.036a2.5 2.5 0 113.536 3.536L6.5 21.036H3v-3.572L16.732 3.732z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Oncology</h4>
                </div>
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-indigo-100 text-indigo-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 14l9-5-9-5-9 5 9 5z"></path><path d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 14l9-5-9-5-9 5 9 5zm0 0v6"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Orthopaedics & Spine</h4>
                </div>
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-green-100 text-green-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11 5H6a2 2 0 00-2 2v11a2 2 0 002 2h11a2 2 0 002-2v-5m-1.414-9.414a2 2 0 112.828 2.828L11.828 15H9v-2.828l8.586-8.586z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Gastroenterology</h4>
                </div>
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-yellow-100 text-yellow-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6V4m0 2a2 2 0 100 4m0-4a2 2 0 110 4m-6 8a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4m6 6v10m6-2a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Urology & Nephrology</h4>
                </div>
                 <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-pink-100 text-pink-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5.636 18.364a9 9 0 010-12.728m12.728 0a9 9 0 010 12.728m-9.9-2.829a5 5 0 010-7.07m7.07 0a5 5 0 010 7.07"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Pulmonology</h4>
                </div>
                 <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-teal-100 text-teal-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 10l4.553-2.276A1 1 0 0121 8.618v6.764a1 1 0 01-1.447.894L15 14M5 18h8a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v8a2 2 0 002 2z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">ENT (Otolaryngology)</h4>
                </div>
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-orange-100 text-orange-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Dermatology</h4>
                </div>
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-red-100 text-red-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c1.657 0 3-1.343 3-3S13.657 2 12 2 9 3.343 9 5s1.343 3 3 3zm0 2c-2.21 0-4 1.79-4 4v1h8v-1c0-2.21-1.79-4-4-4z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Obstetrics & Gynaecology</h4>
                </div>
                 <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-blue-100 text-blue-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 14l9-5-9-5-9 5 9 5z"></path><path d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Paediatrics & Neonatology</h4>
                </div>
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-purple-100 text-purple-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Endocrinology</h4>
                </div>
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-indigo-100 text-indigo-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 11.5V14m0-2.5v-6a1.5 1.5 0 113 0m-3 6a1.5 1.5 0 00-3 0v2a7.5 7.5 0 0015 0v-5a1.5 1.5 0 00-3 0m-6-3V11m0-5.5v-1a1.5 1.5 0 013 0v1m0 0V11m0-5.5a1.5 1.5 0 013 0v3m0 0V11"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Rheumatology</h4>
                </div>
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-green-100 text-green-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Ophthalmology (Eye Care)</h4>
                </div>
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-yellow-100 text-yellow-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 8V4m0 0h4M4 4l5 5m11-1V4m0 0h-4m4 0l-5 5M4 16v4m0 0h4m-4 0l5-5m11 5v4m0 0h-4m4 0l-5-5"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Dentistry & Maxillofacial</h4>
                </div>
                 <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-red-100 text-red-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4m0 4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Emergency & Trauma</h4>
                </div>

            </div>
        </div>
    </section>
    
    <!-- Find a Doctor Section -->
    <section id="find-doctor" class="py-20 bg-blue-50" x-data="doctorDirectory()">
        <div class="container mx-auto px-6">
            <h2 class="section-title">Meet Our World-Class Specialists</h2>
            <p class="section-subtitle">Our team comprises globally recognized experts, each a leader in their respective field. Use the filters below to find the right specialist for your needs.</p>
            
            <!-- Filter Controls -->
            <div class="max-w-4xl mx-auto flex flex-col md:flex-row gap-4 mb-12">
                <input type="text" x-model="searchQuery" placeholder="Search by doctor's name..." class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 flex-grow">
                <select x-model="selectedSpecialty" class="w-full md:w-1/3 px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 bg-white">
                    <option value="">All Specialties</option>
                    <option value="Cardiology">Cardiology</option>
                    <option value="Orthopaedics">Orthopaedics</option>
                    <option value="Oncology">Oncology</option>
                    <option value="Neurology">Neurology</option>
                </select>
            </div>

            <!-- Doctor Profiles Grid -->
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <template x-for="doctor in filteredDoctors()" :key="doctor.name">
                    <div class="bg-white rounded-lg shadow-lg overflow-hidden text-center transform hover:-translate-y-2 transition-transform duration-300">
                        <img :src="doctor.image" :alt="doctor.name" class="w-full h-64 object-cover object-center">
                        <div class="p-6">
                            <h3 class="text-2xl font-bold text-gray-800" x-text="doctor.name"></h3>
                            <p class="text-blue-600 font-semibold mt-1" x-text="doctor.title"></p>
                            <p class="text-gray-500 text-sm" x-text="doctor.credentials"></p>
                            <p class="text-gray-600 mt-4 text-sm" x-text="doctor.bio"></p>
                            <button class="mt-6 px-6 py-2 border-2 border-blue-600 text-blue-600 font-semibold rounded-full hover:bg-blue-600 hover:text-white transition">View Full Profile</button>
                        </div>
                    </div>
                </template>
            </div>
        </div>
    </section>

    <!-- Pharmacy & Wellness Section -->
    <section id="pharmacy" class="py-20 bg-gray-100">
        <div class="container mx-auto px-6">
            <h2 class="section-title">Valetudeo Pharmacy & Wellness Store</h2>
            <p class="section-subtitle">Our state-of-the-art pharmacy provides comprehensive, specialized services, fully integrated with your clinical care and DrugD's research.</p>
             <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
                <div class="bg-white p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-blue-100 text-blue-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Inpatient Pharmacy</h4>
                </div>
                <div class="bg-white p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-green-100 text-green-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Outpatient Pharmacy</h4>
                </div>
                <div class="bg-white p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-purple-100 text-purple-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19.428 15.428a2 2 0 00-1.022-.547l-2.387-.477a6 6 0 00-3.86.517l-.318.158a6 6 0 01-3.86.517L6.05 15.21a2 2 0 00-1.806.547a2 2 0 00-.547 1.806l.477 2.387a6 6 0 00.517 3.86l.158.318a6 6 0 003.86.517l2.387.477a2 2 0 001.806-.547a2 2 0 00.547-1.806l-.477-2.387a6 6 0 00-.517-3.86l-.158-.318z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14.243 5.757a2 2 0 10-2.828-2.828 2 2 0 002.828 2.828z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Oncology Pharmacy</h4>
                </div>
                 <div class="bg-white p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-yellow-100 text-yellow-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 3v1m0 16v1m9-9h-1M4 12H3m15.364 6.364l-.707-.707M6.343 6.343l-.707-.707m12.728 0l-.707.707M6.343 17.657l-.707.707M16 12a4 4 0 11-8 0 4 4 0 018 0z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Compounding Lab</h4>
                </div>
                 <div class="bg-white p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-red-100 text-red-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Critical Care Pharmacy</h4>
                </div>
                <div class="bg-white p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-indigo-100 text-indigo-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 14l9-5-9-5-9 5 9 5z"></path><path d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Paediatric Pharmacy</h4>
                </div>
                <div class="bg-white p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-pink-100 text-pink-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 3v4M3 5h4M6 17v4m-2-2h4m5-12v4m-2-2h4m5 4v4m-2-2h4M17 3h4m-2 2v4"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Nutritional Support</h4>
                </div>
                <div class="bg-white p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-teal-100 text-teal-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-5m-9 0H3m2 0h5M9 7h1m-1 4h1m4-4h1m-1 4h1m-5 4h5m-5 4h5"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Investigational Drugs</h4>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Nursing Excellence Section -->
    <section id="nursing" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <h2 class="section-title">Nursing Excellence at Valetudeo</h2>
            <p class="section-subtitle">Our nurses are the compassionate backbone of our hospital, providing expert, specialized care with unwavering dedication at every step of the patient journey.</p>
             <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-red-100 text-red-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Cardiac Care Nursing</h4>
                </div>
                 <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-blue-100 text-blue-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Critical Care (ICU) Nursing</h4>
                </div>
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-purple-100 text-purple-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15.232 5.232l3.536 3.536m-2.036-5.036a2.5 2.5 0 113.536 3.536L6.5 21.036H3v-3.572L16.732 3.732z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Oncology Nursing</h4>
                </div>
                <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-red-100 text-red-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c1.657 0 3-1.343 3-3S13.657 2 12 2 9 3.343 9 5s1.343 3 3 3zm0 2c-2.21 0-4 1.79-4 4v1h8v-1c0-2.21-1.79-4-4-4z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Maternity Nursing</h4>
                </div>
                 <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-indigo-100 text-indigo-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 14l9-5-9-5-9 5 9 5z"></path><path d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Paediatric Nursing</h4>
                </div>
                 <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-green-100 text-green-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2m-3 7h3m-3 4h3m-6-4h.01M9 16h.01"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Surgical Nursing</h4>
                </div>
                 <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-yellow-100 text-yellow-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4m0 4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Emergency Nursing</h4>
                </div>
                 <div class="bg-gray-50 p-4 rounded-lg shadow-md hover:shadow-lg hover:scale-105 transition-all duration-300 flex items-center gap-4">
                    <div class="flex-shrink-0 bg-pink-100 text-pink-600 rounded-full p-3"><svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14.752 11.168l-3.197-2.132A1 1 0 0010 9.87v4.263a1 1 0 001.555.832l3.197-2.132a1 1 0 000-1.664z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg></div>
                    <h4 class="font-bold text-gray-800">Rehabilitation Nursing</h4>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section id="testimonials" class="py-20 bg-gray-100">
        <div class="container mx-auto px-6">
            <h2 class="section-title">Stories of Hope & Healing</h2>
            <p class="section-subtitle">We are honored to have been a part of our patients' journeys. Here are a few of their stories.</p>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-white p-8 rounded-xl shadow-lg">
                    <p class="text-gray-600 italic">"The level of care and expertise at Valetudeo is simply unmatched. From the doctors to the nurses, everyone made me feel safe and cared for. I am forever grateful for my successful heart surgery."</p>
                    <div class="flex items-center mt-6">
                        <img src="https://placehold.co/60x60/BDBDBD/FFFFFF?text=AA" alt="Patient" class="w-14 h-14 rounded-full">
                        <div class="ml-4">
                            <p class="font-bold text-gray-800">Amina Ahmed</p>
                            <p class="text-gray-500">Dubai, UAE</p>
                        </div>
                    </div>
                </div>
                <div class="bg-white p-8 rounded-xl shadow-lg">
                    <p class="text-gray-600 italic">"My son received treatment at the neurology institute, and the results have been life-changing. The combination of advanced technology and compassionate care made all the difference."</p>
                     <div class="flex items-center mt-6">
                        <img src="https://placehold.co/60x60/BDBDBD/FFFFFF?text=JB" alt="Patient" class="w-14 h-14 rounded-full">
                        <div class="ml-4">
                            <p class="font-bold text-gray-800">John Baker</p>
                            <p class="text-gray-500">London, UK</p>
                        </div>
                    </div>
                </div>
                <div class="bg-white p-8 rounded-xl shadow-lg">
                     <p class="text-gray-600 italic">"As an international patient, the process was incredibly smooth. The patient services team handled everything from my visa to accommodation. I could focus completely on my recovery."</p>
                     <div class="flex items-center mt-6">
                        <img src="https://placehold.co/60x60/BDBDBD/FFFFFF?text=SC" alt="Patient" class="w-14 h-14 rounded-full">
                        <div class="ml-4">
                            <p class="font-bold text-gray-800">Sofia Costa</p>
                            <p class="text-gray-500">Rio de Janeiro, Brazil</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- International Patient Services -->
    <section id="international-patients" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <h2 class="section-title">Seamless Care for International Patients</h2>
            <p class="section-subtitle">We provide dedicated, end-to-end support to ensure a comfortable and stress-free medical journey for patients and families traveling from across the globe.</p>
            <div class="grid grid-cols-2 md:grid-cols-3 gap-8 text-center">
                <div class="bg-blue-50 p-6 rounded-lg shadow-md">
                    <h4 class="font-bold text-lg text-blue-800">Visa & Travel Assistance</h4>
                </div>
                <div class="bg-blue-50 p-6 rounded-lg shadow-md">
                    <h4 class="font-bold text-lg text-blue-800">Airport Transfers</h4>
                </div>
                <div class="bg-blue-50 p-6 rounded-lg shadow-md">
                    <h4 class="font-bold text-lg text-blue-800">Accommodation Services</h4>
                </div>
                <div class="bg-blue-50 p-6 rounded-lg shadow-md">
                    <h4 class="font-bold text-lg text-blue-800">Multilingual Interpreters</h4>
                </div>
                <div class="bg-blue-50 p-6 rounded-lg shadow-md">
                    <h4 class="font-bold text-lg text-blue-800">Dedicated Care Coordinator</h4>
                </div>
                <div class="bg-blue-50 p-6 rounded-lg shadow-md">
                    <h4 class="font-bold text-lg text-blue-800">Telemedicine Consults</h4>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact and Appointment Section -->
    <section id="contact" class="py-20 bg-blue-50">
        <div class="container mx-auto px-6">
            <h2 class="section-title">Begin Your Journey to Health</h2>
            <p class="section-subtitle">Whether you need a consultation, a second opinion, or wish to schedule a treatment, our global patient services team is here to assist you. </p>
            <div class="max-w-4xl mx-auto bg-white p-8 sm:p-12 rounded-2xl shadow-2xl">
                <form>
                    <div class="grid md:grid-cols-2 gap-6">
                        <input type="text" placeholder="Full Name" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                        <input type="tel" placeholder="Phone Number (+254...)" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                        <input type="email" placeholder="Email Address" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                        <select class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 bg-white text-gray-500">
                            <option>Select a Department or Service</option>
                            <option>Cardiology</option>
                            <option>Orthopaedics</option>
                            <option>Oncology</option>
                            <option>Neurology</option>
                            <option>General Surgery</option>
                            <option>Diagnostics & Imaging</option>
                        </select>
                        <div class="md:col-span-2">
                            <textarea rows="4" placeholder="Briefly describe your medical needs..." class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"></textarea>
                        </div>
                    </div>
                    <div class="text-center mt-8">
                        <button type="submit" class="cta-button w-full sm:w-auto">Submit Request</button>
                    </div>
                </form>
            </div>
        </div>
    </section>
    
    <!-- Footer -->
    <footer class="bg-gray-900 text-white">
        <div class="container mx-auto px-6 py-12">
            <div class="grid md:grid-cols-3 gap-8">
                <div>
                    <h3 class="text-2xl font-bold mb-2">Valetudeo</h3>
                    <p class="text-gray-400">Excellence in Health. Compassion for Life.</p>
                    <p class="text-gray-400 mt-4">Global Headquarters: Gigiri, Nairobi, Kenya</p>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-4">Quick Links</h4>
                    <ul>
                        <li class="mb-2"><a href="#about" class="hover:text-blue-400">About Us</a></li>
                        <li class="mb-2"><a href="#services" class="hover:text-blue-400">Specialities</a></li>
                        <li class="mb-2"><a href="#find-doctor" class="hover:text-blue-400">Find a Doctor</a></li>
                        <li class="mb-2"><a href="#pharmacy" class="hover:text-blue-400">Pharmacy</a></li>
                        <li class="mb-2"><a href="#nursing" class="hover:text-blue-400">Nursing</a></li>
                        <li class="mb-2"><a href="#international-patients" class="hover:text-blue-400">International Patients</a></li>
                        <li class="mb-2"><a href="#contact" class="hover:text-blue-400">Contact Us</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-lg font-semibold mb-4">Contact Information</h4>
                    <p class="text-gray-400 mb-2">Emergency (24/7): +254 799 670506</p>
                    <p class="text-gray-400 mb-2">Appointments: +254 799 670506</p>
                    <p class="text-gray-400">Email: info@valetudeo.com</p>
                </div>
            </div>
            <div class="mt-8 border-t border-gray-700 pt-8 text-center text-gray-400">
                <p>&copy; 2025 Valetudeo Global Hospital. All Rights Reserved.</p>
            </div>
        </div>
    </footer>
    
    <script>
        function doctorDirectory() {
            return {
                searchQuery: '',
                selectedSpecialty: '',
                doctors: [
                    { 
                        name: 'Dr. Siham Deq Hassan', 
                        title: 'Founder & Chief Surgeon', 
                        credentials: 'MD, Board-Certified Physician',
                        specialty: 'Surgery',
                        bio: 'Dr. Hassan is the clinical heart of Valetudeo, championing minimally invasive and robotic surgery.',
                        image: 'https://placehold.co/600x400/BDBDBD/FFFFFF?text=Dr.+Siham'
                    },
                    { 
                        name: 'Dr. Ahmed', 
                        title: 'Chief Cardiologist', 
                        credentials: 'MD, FACC',
                        specialty: 'Cardiology',
                        bio: 'With over 20 years of experience, Dr. Ahmed is a pioneer in interventional cardiology and structural heart diseases.',
                        image: 'https://placehold.co/600x400/90CDF4/2C5282?text=Dr.+Ahmed'
                    },
                    { 
                        name: 'Dr. Ben Carter', 
                        title: 'Head Orthopaedic Surgeon', 
                        credentials: 'MS Ortho',
                        specialty: 'Orthopaedics',
                        bio: 'Dr. Carter specializes in robotic-assisted joint replacement, ensuring precision and rapid patient recovery.',
                        image: 'https://placehold.co/600x400/A5B4FC/312E81?text=Dr.+Carter'
                    },
                    { 
                        name: 'Dr. Khalid Abshir', 
                        title: 'Senior Oncologist', 
                        credentials: 'DM Oncology',
                        specialty: 'Oncology',
                        bio: 'A leader in targeted therapy and cancer research, Dr. Abshir is dedicated to personalized cancer care.',
                        image: 'https://placehold.co/600x400/F9A8D4/831843?text=Dr.+Abshir'
                    },
                    { 
                        name: 'Dr. Evelyn Reed', 
                        title: 'Director of Neurosciences', 
                        credentials: 'PhD, MD',
                        specialty: 'Neurology',
                        bio: 'Dr. Reed is an expert in complex brain and spine disorders, utilizing the latest in neuro-navigation technology.',
                        image: 'https://placehold.co/600x400/FDE68A/713F12?text=Dr.+Reed'
                    },
                     { 
                        name: 'Dr. Maria Flores', 
                        title: 'Lead Gastroenterologist', 
                        credentials: 'MD, FASGE',
                        specialty: 'Gastroenterology',
                        bio: 'Specializing in advanced therapeutic endoscopy and managing complex digestive and liver diseases.',
                        image: 'https://placehold.co/600x400/A7F3D0/065F46?text=Dr.+Flores'
                    }
                ],
                filteredDoctors() {
                    if (this.searchQuery === '' && this.selectedSpecialty === '') {
                        return this.doctors;
                    }
                    return this.doctors.filter(doctor => {
                        const nameMatch = doctor.name.toLowerCase().includes(this.searchQuery.toLowerCase());
                        const specialtyMatch = this.selectedSpecialty === '' || doctor.specialty === this.selectedSpecialty;
                        return nameMatch && specialtyMatch;
                    });
                }
            }
        }
    </script>

</body>
</html>
