# web-portofolio-Muhammad-Farhan
```html
<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Muhammad Farhan - Interactive Portfolio & CV</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts: Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        navy: {
                            800: '#1E293B',
                            900: '#0F172A',
                            950: '#020617',
                        },
                        amber: {
                            500: '#F59E0B',
                            600: '#D97706',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        /* Custom scrollbar styling */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #F1F5F9;
        }
        ::-webkit-scrollbar-thumb {
            background: #CBD5E1;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #94A3B8;
        }
    </style>
</head>
<body class="font-sans bg-slate-50 text-slate-800 antialiased selection:bg-amber-500 selection:text-white">

    <!-- Navigation Header -->
    <header class="sticky top-0 z-50 bg-white/90 backdrop-blur-md border-b border-slate-200">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 h-16 flex items-center justify-between">
            <a href="#" class="font-extrabold text-xl text-navy-900 tracking-tight flex items-center gap-2">
                <span class="bg-gradient-to-r from-navy-900 to-blue-900 text-amber-500 w-8 h-8 rounded-lg flex items-center justify-center font-black">MF</span>
                <span>M. FARHAN</span>
            </a>
            
            <!-- Desktop Navigation -->
            <nav class="hidden md:flex items-center space-x-8 text-sm font-semibold text-slate-600">
                <a href="#about" class="hover:text-amber-600 transition-colors">Tentang Saya</a>
                <a href="#experience" class="hover:text-amber-600 transition-colors">Pengalaman</a>
                <a href="#skills" class="hover:text-amber-600 transition-colors">Keahlian</a>
                <a href="#organization" class="hover:text-amber-600 transition-colors">Organisasi</a>
                <a href="#contact" class="px-4 py-2 bg-navy-900 text-white rounded-lg hover:bg-slate-800 transition-colors shadow-sm">Hubungi Saya</a>
            </nav>

            <!-- Mobile Menu Button -->
            <button id="mobile-menu-btn" class="md:hidden p-2 text-slate-600 hover:text-navy-900 focus:outline-none" aria-label="Toggle menu">
                <i class="fa-solid fa-bars text-xl" id="menu-icon"></i>
            </button>
        </div>

        <!-- Mobile Navigation Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-b border-slate-200 px-4 pt-2 pb-6 space-y-3 font-medium text-slate-600">
            <a href="#about" class="block py-2 hover:text-amber-600">Tentang Saya</a>
            <a href="#experience" class="block py-2 hover:text-amber-600">Pengalaman</a>
            <a href="#skills" class="block py-2 hover:text-amber-600">Keahlian</a>
            <a href="#organization" class="block py-2 hover:text-amber-600">Organisasi</a>
            <a href="#contact" class="block py-2 text-amber-600 font-semibold">Hubungi Saya</a>
        </div>
    </header>

    <main>
        <!-- Hero Section -->
        <section class="relative bg-gradient-to-b from-white via-slate-50 to-slate-100 pt-16 pb-20 md:pt-24 md:pb-32 overflow-hidden">
            <!-- Decorative Background Elements -->
            <div class="absolute top-0 right-0 -mr-20 -mt-20 w-96 h-96 bg-amber-500/10 rounded-full blur-3xl pointer-events-none"></div>
            <div class="absolute bottom-0 left-0 -ml-20 -mb-20 w-96 h-96 bg-blue-600/10 rounded-full blur-3xl pointer-events-none"></div>

            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
                <div class="grid md:grid-cols-12 gap-12 items-center">
                    
                    <div class="md:col-span-7 space-y-6 text-left">
                        <div class="inline-flex items-center gap-2 px-3 py-1.5 rounded-full bg-amber-100 text-amber-800 text-xs sm:text-sm font-semibold border border-amber-200">
                            <span class="w-2 h-2 rounded-full bg-amber-500 animate-pulse"></span>
                            Siap Ditempatkan Di Mana Saja & Posisi Apa Saja
                        </div>
                        
                        <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold text-navy-900 tracking-tight leading-tight">
                            Operator Produksi <br>
                            <span class="text-transparent bg-clip-text bg-gradient-to-r from-amber-600 to-amber-500">Multitalenta & Andal</span>
                        </h1>
                        
                        <p class="text-base sm:text-lg text-slate-600 max-w-2xl leading-relaxed">
                            Pengalaman 3.5+ tahun di manufaktur otomotif, pengelasan robotik/spot, pengemasan presisi, hingga kontrol kualitas. Memiliki fisik prima, kedisiplinan tinggi, dan daya tangkap cepat.
                        </p>

                        <!-- CTA Buttons -->
                        <div class="flex flex-wrap gap-4 pt-2">
                            <a href="#contact" class="px-6 py-3.5 bg-navy-900 hover:bg-slate-800 text-white font-semibold rounded-xl shadow-lg shadow-navy-900/20 transition-all transform hover:-translate-y-0.5 flex items-center gap-2">
                                <i class="fa-solid fa-paper-plane"></i>
                                Rekrut Saya
                            </a>
                            <a href="#experience" class="px-6 py-3.5 bg-white border border-slate-300 hover:border-slate-400 text-slate-700 font-semibold rounded-xl shadow-sm transition-all flex items-center gap-2">
                                <i class="fa-solid fa-briefcase text-amber-600"></i>
                                Lihat Pengalaman
                            </a>
                        </div>

                        <!-- Quick Badges -->
                        <div class="grid grid-cols-3 gap-4 pt-6 border-t border-slate-200">
                            <div>
                                <p class="text-2xl sm:text-3xl font-extrabold text-navy-900">3.5+</p>
                                <p class="text-xs sm:text-sm text-slate-500 font-medium">Tahun Pengalaman</p>
                            </div>
                            <div>
                                <p class="text-2xl sm:text-3xl font-extrabold text-amber-600">99.2%</p>
                                <p class="text-xs sm:text-sm text-slate-500 font-medium">Akurasi Defect-Free</p>
                            </div>
                            <div>
                                <p class="text-2xl sm:text-3xl font-extrabold text-navy-900">100%</p>
                                <p class="text-xs sm:text-sm text-slate-500 font-medium">Kesiapan Kerja Shift</p>
                            </div>
                        </div>
                    </div>

                    <!-- Hero Visual Card -->
                    <div class="md:col-span-5 flex justify-center">
                        <div class="relative w-full max-w-md bg-white p-6 sm:p-8 rounded-3xl shadow-xl border border-slate-100">
                            <!-- Avatar Placeholder Icon -->
                            <div class="w-24 h-24 mx-auto mb-6 bg-slate-100 rounded-full flex items-center justify-center text-slate-400 border-4 border-white shadow-inner">
                                <i class="fa-solid fa-user-gear text-4xl text-navy-900"></i>
                            </div>

                            <div class="text-center space-y-2">
                                <h3 class="text-xl font-bold text-navy-900">Muhammad Farhan</h3>
                                <p class="text-xs font-semibold text-amber-600 uppercase tracking-wider">Bekasi, Jawa Barat</p>
                                <p class="text-xs text-slate-500">Lulusan SMK Technical Computer & Network (TKJ)</p>
                            </div>

                            <div class="mt-6 space-y-3 text-sm">
                                <div class="flex items-center gap-3 p-3 bg-slate-50 rounded-xl">
                                    <i class="fa-solid fa-robot text-amber-600 w-5 text-center"></i>
                                    <span class="font-medium text-slate-700">Welding Robot & Spot Operator</span>
                                </div>
                                <div class="flex items-center gap-3 p-3 bg-slate-50 rounded-xl">
                                    <i class="fa-solid fa-box text-amber-600 w-5 text-center"></i>
                                    <span class="font-medium text-slate-700">Packing & Quality Control</span>
                                </div>
                                <div class="flex items-center gap-3 p-3 bg-slate-50 rounded-xl">
                                    <i class="fa-solid fa-shield-halved text-amber-600 w-5 text-center"></i>
                                    <span class="font-medium text-slate-700">Penerap Standar K3 & 5S</span>
                                </div>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- About Me Section -->
        <section id="about" class="py-16 bg-white border-y border-slate-200">
            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="max-w-3xl mx-auto text-center space-y-4">
                    <h2 class="text-xs font-extrabold uppercase tracking-widest text-amber-600">Professional Summary</h2>
                    <h3 class="text-3xl font-extrabold text-navy-900">Siap Memberikan Kontribusi Terbaik</h3>
                    <div class="w-16 h-1 bg-amber-500 mx-auto rounded-full"></div>
                </div>

                <div class="mt-10 max-w-4xl mx-auto bg-slate-50 p-6 sm:p-8 rounded-2xl border border-slate-200 shadow-sm leading-relaxed text-slate-700 space-y-4">
                    <p>
                        Saya adalah <strong>Production Operator</strong> yang adaptif, pekerja keras, dan berorientasi pada hasil dengan total pengalaman lapangan lebih dari <strong>3.5 tahun</strong>. Pengalaman saya mencakup operasional pengelasan robotik/spot di industri manufaktur komponen otomotif, kontrol kualitas packaging produk konsumen, fabrikasi logam, hingga pemeliharaan fasilitas (housekeeping).
                    </p>
                    <p>
                        Memiliki latar belakang pendidikan Teknik Komputer & Jaringan (TKJ), yang membekali saya dengan pemikiran logis, ketelitian teknis, dan kemampuan cepat beradaptasi dengan mesin operasional modern. <strong>Saya sangat amat siap untuk ditempatkan di posisi mana pun</strong> (Operator Welding, Packing, QC, Assembly, atau Helper Produksi) dan fleksibel bekerja dalam sistem shift.
                    </p>
                </div>
            </div>
        </section>

        <!-- Experience Section (XYZ Method Grid Cards) -->
        <section id="experience" class="py-20 bg-slate-50">
            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center space-y-3 mb-16">
                    <h2 class="text-xs font-extrabold uppercase tracking-widest text-amber-600">Track Record</h2>
                    <h3 class="text-3xl sm:text-4xl font-extrabold text-navy-900">Pengalaman Kerja</h3>
                    <p class="text-slate-600 max-w-xl mx-auto">Daftar rekam jejak profesional dengan hasil kerja terukur (Metode XYZ).</p>
                </div>

                <div class="grid md:grid-cols-2 gap-8">
                    
                    <!-- Card 1: PT Ito Seisakusho Armada -->
                    <div class="bg-white p-6 sm:p-8 rounded-2xl shadow-sm border border-slate-200 hover:shadow-md transition-shadow relative flex flex-col justify-between">
                        <div>
                            <div class="flex items-start justify-between gap-4 mb-4">
                                <div>
                                    <span class="text-xs font-bold text-amber-600 uppercase tracking-wide">Juni 2022 – Juni 2024 (2 Tahun)</span>
                                    <h4 class="text-xl font-bold text-navy-900 mt-1">Robotic & Spot Welding Operator</h4>
                                    <p class="text-sm font-semibold text-slate-500">PT Ito Seisakusho Armada • Bekasi</p>
                                </div>
                                <div class="p-3 bg-amber-50 rounded-xl text-amber-600">
                                    <i class="fa-solid fa-fire-flame-curved text-xl"></i>
                                </div>
                            </div>
                            <ul class="space-y-3 text-sm text-slate-600 list-disc list-inside">
                                <li><strong>Mengoperasikan mesin welding robot & spot manual</strong> untuk perakitan komponen otomotif, mencapai tingkat bebas cacat (defect-free) <strong>99.2%</strong> selama 2 tahun.</li>
                                <li><strong>Inspeksi hasil lasan</strong> sesuai rancangan cetak biru (blueprint) teknik, menurunkan tingkat pengerjaan ulang (rework) hingga <strong>15%</strong>.</li>
                                <li><strong>Menerapkan rutin perawatan 5S</strong> pada lengan robot & fixture, mengurangi waktu henti mesin (downtime) sebesar <strong>20%</strong>.</li>
                            </ul>
                        </div>
                    </div>

                    <!-- Card 2: PT Berdikari Metal Steel Engineering -->
                    <div class="bg-white p-6 sm:p-8 rounded-2xl shadow-sm border border-slate-200 hover:shadow-md transition-shadow relative flex flex-col justify-between">
                        <div>
                            <div class="flex items-start justify-between gap-4 mb-4">
                                <div>
                                    <span class="text-xs font-bold text-amber-600 uppercase tracking-wide">Mei 2021 – Mei 2022 (1 Tahun)</span>
                                    <h4 class="text-xl font-bold text-navy-900 mt-1">Production & Fabrication Operator</h4>
                                    <p class="text-sm font-semibold text-slate-500">PT Berdikari Metal Steel Engineering • Bekasi</p>
                                </div>
                                <div class="p-3 bg-slate-100 rounded-xl text-navy-900">
                                    <i class="fa-solid fa-industry text-xl"></i>
                                </div>
                            </div>
                            <ul class="space-y-3 text-sm text-slate-600 list-disc list-inside">
                                <li><strong>Membantu operasional pemotongan metal & stamping</strong>, meningkatkan output harian sebesar <strong>10%</strong> pada masa puncak produksi.</li>
                                <li><strong>Mengatur pemuatan bahan baku</strong> serta penyusunan barang jadi untuk transportasi aman di dalam area manufaktur.</li>
                                <li><strong>Mematuhi secara ketat standar K3</strong>, mencatatkan rekor <strong>Zero Accident (0 kecelakaan kerja)</strong> selama 12 bulan.</li>
                            </ul>
                        </div>
                    </div>

                    <!-- Card 3: PT Audy Dental -->
                    <div class="bg-white p-6 sm:p-8 rounded-2xl shadow-sm border border-slate-200 hover:shadow-md transition-shadow relative flex flex-col justify-between">
                        <div>
                            <div class="flex items-start justify-between gap-4 mb-4">
                                <div>
                                    <span class="text-xs font-bold text-amber-600 uppercase tracking-wide">Nov 2020 – Apr 2021 (6 Bulan)</span>
                                    <h4 class="text-xl font-bold text-navy-900 mt-1">Facility Care & Housekeeping</h4>
                                    <p class="text-sm font-semibold text-slate-500">PT Audy Dental • Jakarta</p>
                                </div>
                                <div class="p-3 bg-slate-100 rounded-xl text-navy-900">
                                    <i class="fa-solid fa-broom text-xl"></i>
                                </div>
                            </div>
                            <ul class="space-y-3 text-sm text-slate-600 list-disc list-inside">
                                <li><strong>Melakukan sanitasi & sterilisasi fasilitas klinik</strong>, mencapai tingkat kepatuhan <strong>100%</strong> dalam audit higiene internal.</li>
                                <li><strong>Mengelola inventaris alat kebersihan</strong> dan protokol pembuangan limbah tanpa mengganggu kelancaran operasional medis.</li>
                            </ul>
                        </div>
                    </div>

                    <!-- Card 4: PT Prakarsa Alam Segar -->
                    <div class="bg-white p-6 sm:p-8 rounded-2xl shadow-sm border border-slate-200 hover:shadow-md transition-shadow relative flex flex-col justify-between">
                        <div>
                            <div class="flex items-start justify-between gap-4 mb-4">
                                <div>
                                    <span class="text-xs font-bold text-amber-600 uppercase tracking-wide">Juli 2020 – Okt 2020 (3 Bulan)</span>
                                    <h4 class="text-xl font-bold text-navy-900 mt-1">Packaging & Quality Control Operator</h4>
                                    <p class="text-sm font-semibold text-slate-500">PT Prakarsa Alam Segar • Bekasi</p>
                                </div>
                                <div class="p-3 bg-slate-100 rounded-xl text-navy-900">
                                    <i class="fa-solid fa-boxes-packing text-xl"></i>
                                </div>
                            </div>
                            <ul class="space-y-3 text-sm text-slate-600 list-disc list-inside">
                                <li><strong>Melakukan pengemasan & pelabelan produk</strong> dengan kecepatan <strong>1,200+ unit/shift</strong> sambil memverifikasi kerapatan segel.</li>
                                <li><strong>Inspeksi visual QC</strong> untuk mendeteksi pengemasan cacat, mencegah barang sub-standar masuk ke jalur distribusi.</li>
                            </ul>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- Skills Section -->
        <section id="skills" class="py-20 bg-white border-t border-slate-200">
            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center space-y-3 mb-12">
                    <h2 class="text-xs font-extrabold uppercase tracking-widest text-amber-600">Competencies</h2>
                    <h3 class="text-3xl font-extrabold text-navy-900">Keahlian & Keterampilan</h3>
                </div>

                <div class="grid md:grid-cols-2 gap-8 max-w-4xl mx-auto">
                    <!-- Technical / Hard Skills -->
                    <div class="bg-slate-50 p-6 rounded-2xl border border-slate-200">
                        <h4 class="text-lg font-bold text-navy-900 mb-4 flex items-center gap-2">
                            <i class="fa-solid fa-gears text-amber-600"></i> Hard Skills & Teknis
                        </h4>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3.5 py-2 bg-white text-navy-900 border border-slate-200 text-sm font-medium rounded-xl shadow-sm">Operasional Robot Welding</span>
                            <span class="px-3.5 py-2 bg-white text-navy-900 border border-slate-200 text-sm font-medium rounded-xl shadow-sm">Spot Welding Manual</span>
                            <span class="px-3.5 py-2 bg-white text-navy-900 border border-slate-200 text-sm font-medium rounded-xl shadow-sm">Packaging & Labeling</span>
                            <span class="px-3.5 py-2 bg-white text-navy-900 border border-slate-200 text-sm font-medium rounded-xl shadow-sm">Quality Control (QC)</span>
                            <span class="px-3.5 py-2 bg-white text-navy-900 border border-slate-200 text-sm font-medium rounded-xl shadow-sm">Membaca Blueprint Teknik</span>
                            <span class="px-3.5 py-2 bg-white text-navy-900 border border-slate-200 text-sm font-medium rounded-xl shadow-sm">Penerapan Standar 5S & K3</span>
                            <span class="px-3.5 py-2 bg-white text-navy-900 border border-slate-200 text-sm font-medium rounded-xl shadow-sm">Fabrikasi Logam Dasar</span>
                            <span class="px-3.5 py-2 bg-white text-navy-900 border border-slate-200 text-sm font-medium rounded-xl shadow-sm">Perakitan Industri</span>
                        </div>
                    </div>

                    <!-- Soft Skills & Adaptability -->
                    <div class="bg-slate-50 p-6 rounded-2xl border border-slate-200">
                        <h4 class="text-lg font-bold text-navy-900 mb-4 flex items-center gap-2">
                            <i class="fa-solid fa-user-check text-amber-600"></i> Soft Skills & Karakter
                        </h4>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3.5 py-2 bg-amber-500 text-white text-sm font-semibold rounded-xl shadow-sm">Siap Bekerja di Posisi Apapun</span>
                            <span class="px-3.5 py-2 bg-white text-navy-900 border border-slate-200 text-sm font-medium rounded-xl shadow-sm">Ketahanan Fisik Tinggi</span>
                            <span class="px-3.5 py-2 bg-white text-navy-900 border border-slate-200 text-sm font-medium rounded-xl shadow-sm">Kerjasama Tim & Kepemimpinan</span>
                            <span class="px-3.5 py-2 bg-white text-navy-900 border border-slate-200 text-sm font-medium rounded-xl shadow-sm">Disiplin & Tepat Waktu</span>
                            <span class="px-3.5 py-2 bg-white text-navy-900 border border-slate-200 text-sm font-medium rounded-xl shadow-sm">Penyelesaian Masalah</span>
                            <span class="px-3.5 py-2 bg-white text-navy-900 border border-slate-200 text-sm font-medium rounded-xl shadow-sm">Cepat Belajar (Fast Learner)</span>
                            <span class="px-3.5 py-2 bg-white text-navy-900 border border-slate-200 text-sm font-medium rounded-xl shadow-sm">Fleksibilitas Shift Kerja</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Organization & Social Section -->
        <section id="organization" class="py-16 bg-slate-50 border-t border-slate-200">
            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="max-w-4xl mx-auto bg-white p-8 rounded-2xl border border-slate-200 shadow-sm flex flex-col md:flex-row items-center gap-8">
                    <div class="w-16 h-16 bg-amber-100 text-amber-600 rounded-2xl flex items-center justify-center shrink-0 text-3xl">
                        <i class="fa-solid fa-people-group"></i>
                    </div>
                    <div class="space-y-2 text-center md:text-left">
                        <span class="text-xs font-bold text-amber-600 uppercase tracking-wide">Pengalaman Organisasi • Jan 2021 – Des 2023</span>
                        <h4 class="text-2xl font-bold text-navy-900">Ketua Karang Taruna RT</h4>
                        <p class="text-sm text-slate-600 leading-relaxed">
                            Memimpin tim yang terdiri dari 15 pemuda untuk merencanakan dan mengeksekusi program bakti sosial serta kegiatan kemasyarakatan yang berdampak langsung pada 200+ keluarga. Mengasah kemampuan kepemimpinan, komunikasi publik, dan penyelesaian konflik.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Education Section -->
        <section class="py-16 bg-white border-t border-slate-200">
            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <h2 class="text-xs font-extrabold uppercase tracking-widest text-amber-600 mb-2">Pendidikan</h2>
                <h3 class="text-2xl font-bold text-navy-900">SMK Bina Siswa Utama Bekasi</h3>
                <p class="text-slate-600 mt-1">Jurusan Teknik Komputer dan Jaringan (TKJ) • Lulus Tahun 2020</p>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="py-20 bg-navy-900 text-white relative">
            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
                <div class="text-center space-y-3 mb-12">
                    <h2 class="text-xs font-extrabold uppercase tracking-widest text-amber-500">Contact & Placement</h2>
                    <h3 class="text-3xl sm:text-4xl font-extrabold text-white">Siap Bekerja Sekarang</h3>
                    <p class="text-slate-400 max-w-xl mx-auto">Silakan hubungi saya melalui kontak di bawah ini untuk proses wawancara atau rekrutmen langsung.</p>
                </div>

                <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-6 max-w-4xl mx-auto">
                    <!-- Email Card -->
                    <div class="bg-slate-800/80 p-6 rounded-2xl border border-slate-700 text-center hover:border-amber-500 transition-colors">
                        <div class="w-12 h-12 bg-amber-500/20 text-amber-500 rounded-xl flex items-center justify-center mx-auto mb-4 text-xl">
                            <i class="fa-solid fa-envelope"></i>
                        </div>
                        <h4 class="text-sm text-slate-400 font-medium">Email Utama</h4>
                        <p class="text-base font-bold text-white mt-1">m.farhan190602@gmail.com</p>
                        <button onclick="copyToClipboard('m.farhan190602@gmail.com')" class="mt-4 text-xs font-semibold text-amber-500 hover:underline">
                            <i class="fa-regular fa-copy"></i> Salin Email
                        </button>
                    </div>

                    <!-- Phone Card -->
                    <div class="bg-slate-800/80 p-6 rounded-2xl border border-slate-700 text-center hover:border-amber-500 transition-colors">
                        <div class="w-12 h-12 bg-amber-500/20 text-amber-500 rounded-xl flex items-center justify-center mx-auto mb-4 text-xl">
                            <i class="fa-solid fa-phone"></i>
                        </div>
                        <h4 class="text-sm text-slate-400 font-medium">Telepon / WhatsApp</h4>
                        <p class="text-base font-bold text-white mt-1">+62 858-8682-5218</p>
                        <a href="https://wa.me/6285886825218" target="_blank" rel="noopener noreferrer" class="inline-block mt-4 text-xs font-semibold text-amber-500 hover:underline">
                            <i class="fa-brands fa-whatsapp"></i> Chat WhatsApp
                        </a>
                    </div>

                    <!-- Location Card -->
                    <div class="bg-slate-800/80 p-6 rounded-2xl border border-slate-700 text-center hover:border-amber-500 transition-colors sm:col-span-2 lg:col-span-1">
                        <div class="w-12 h-12 bg-amber-500/20 text-amber-500 rounded-xl flex items-center justify-center mx-auto mb-4 text-xl">
                            <i class="fa-solid fa-location-dot"></i>
                        </div>
                        <h4 class="text-sm text-slate-400 font-medium">Domisili</h4>
                        <p class="text-base font-bold text-white mt-1">Bekasi, Jawa Barat</p>
                        <span class="inline-block mt-4 text-xs text-slate-400">Siap Relokasi jika Diperlukan</span>
                    </div>
                </div>

                <!-- Toast Notification Box -->
                <div id="toast" class="hidden fixed bottom-6 right-6 bg-slate-800 text-white px-5 py-3 rounded-xl border border-amber-500 shadow-xl flex items-center gap-3 z-50">
                    <i class="fa-solid fa-circle-check text-amber-500"></i>
                    <span id="toast-message" class="text-sm font-medium">Teks berhasil disalin!</span>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-navy-950 text-slate-500 py-8 text-center text-xs border-t border-slate-900">
        <div class="max-w-6xl mx-auto px-4">
            <p>© 2026 Muhammad Farhan. All rights reserved.</p>
        </div>
    </footer>

    <!-- Interactive JavaScript -->
    <script>
        // Mobile menu toggle
        const menuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        const menuIcon = document.getElementById('menu-icon');

        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
            if (mobileMenu.classList.contains('hidden')) {
                menuIcon.classList.remove('fa-xmark');
                menuIcon.classList.add('fa-bars');
            } else {
                menuIcon.classList.remove('fa-bars');
                menuIcon.classList.add('fa-xmark');
            }
        });

        // Close menu on link click
        document.querySelectorAll('#mobile-menu a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
                menuIcon.classList.remove('fa-xmark');
                menuIcon.classList.add('fa-bars');
            });
        });

        // Clipboard Copy function with toast message
        function copyToClipboard(text) {
            const textarea = document.createElement('textarea');
            textarea.value = text;
            document.body.appendChild(textarea);
            textarea.select();
            document.execCommand('copy');
            document.body.removeChild(textarea);

            const toast = document.getElementById('toast');
            const toastMsg = document.getElementById('toast-message');
            toastMsg.innerText = 'Email disalin: ' + text;
            toast.classList.remove('hidden');

            setTimeout(() => {
                toast.classList.add('hidden');
            }, 3000);
        }
    </script>
</body>
</html>
```