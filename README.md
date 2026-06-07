<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Teknoloji ve Tasarım Günlüğüm</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    
    <style>
        ::-webkit-scrollbar { display: none; }
        html { scrollbar-width: none; -ms-overflow-style: none; }
        
        /* Canlı durum ışığının nefes alıp verme animasyonu */
        .ping-animate {
            animation: ping-pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
        }
        @keyframes ping-pulse {
            0%, 100% { opacity: 1; transform: scale(1); }
            50% { opacity: .4; transform: scale(1.1); }
        }
    </style>
</head>
<body class="bg-light" style="overflow-x: hidden;">

    <nav class="navbar navbar-expand-lg navbar-dark bg-dark shadow-sm">
        <div class="container">
            <a class="navbar-brand fw-bold" href="#">Make3D Lab</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link active" href="#">Ana Sayfa</a></li>
                    <li class="nav-item"><a class="nav-link" href="#hakkimda">Hakkımda</a></li>
                    <li class="nav-item"><a class="nav-link" href="#projeler">Çalışmalarım</a></li>
                    <li class="nav-item"><a class="nav-link" href="#gunluk">Lab Günlüğü</a></li>
                    <li class="nav-item"><a class="nav-link" href="#iletisim">İletişim</a></li>
                </ul>
            </div>
        </div>
    </nav>
    <header class="container mt-5 mb-4">
        <div class="p-5 text-center bg-white rounded-4 shadow-sm border border-light position-relative overflow-hidden">
            
            <div class="position-absolute top-0 end-0 m-3 d-inline-flex align-items-center bg-dark text-white px-3 py-1.5 rounded-pill shadow-sm small border border-secondary">
                <span class="d-inline-block bg-success rounded-circle me-2 ping-animate" style="width: 10px; height: 10px;"></span>
                <span class="fw-bold me-1 text-secondary-emphasis" style="font-size: 0.8rem;">Atölye:</span>
                <span id="live-status-text" class="fw-semibold text-success" style="font-size: 0.8rem;">Yükleniyor...</span>
            </div>

            <h1 class="display-4 fw-bold text-dark mt-3">Geleceği Kodluyor ve İnşa Ediyorum</h1>
            <p class="lead text-muted mt-3">
                Algoritmalar, otonom sistemler ve hızlı prototipleme dünyama hoş geldiniz. Burada, vizyoner bir araştırmacı olarak mühendislik serüvenimde edindiğim tecrübeleri, teknik notlarımı ve atölyemdeki heyecan verici projeleri paylaşıyorum.
            </p>
            <div class="d-flex justify-content-center flex-wrap gap-3 mt-4">
                <a href="#projeler" class="btn btn-primary btn-lg px-4 rounded-pill shadow-sm">Sistemleri İncele</a>
                
                <a id="youtube-hero-btn" href="#" target="_blank" rel="noopener noreferrer" class="btn btn-danger btn-lg px-4 rounded-pill shadow-sm d-inline-flex align-items-center gap-2">
                    <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" fill="currentColor" class="bi bi-youtube" viewBox="0 0 16 16">
                        <path d="M8.051 1.999h.089c.822.003 4.987.033 6.11.335a2.01 2.01 0 0 1 1.415 1.42c.101.38.172.883.22 1.402l.01.104.022.26.008.104c.065.914.073 1.77.074 1.957v.075c-.001.194-.01 1.053-.075 1.966l-.01.104-.022.26-.008.104a16.5 16.5 0 0 1-.22 1.401 2.01 2.01 0 0 1-1.415 1.42c-1.123.302-5.288.332-6.11.335H8.05a16.5 16.5 0 0 1-6.112-.335 2.01 2.01 0 0 1-1.415-1.42 16.5 16.5 0 0 1-.22-1.401l-.01-.104-.022.26-.008-.104c-.065-.914-.073-1.77-.074-1.957v-.075c.001-.194.01-1.053.075-1.966l.01-.104.022.26.008-.104a16.5 16.5 0 0 1 .22-1.402 2.01 2.01 0 0 1 1.415-1.42c1.123-.302 5.288-.332 6.11-.335zM6.5 5.201v5.596L11 8 6.5 5.201z"/>
                    </svg>
                    YouTube Kanalım
                </a>

                <a href="#hakkimda" class="btn btn-outline-dark btn-lg px-4 rounded-pill">Benimle Tanış</a>
            </div>
        </div>
    </header>
    <section class="container mb-5">
        <div class="row g-3 text-center" id="stats-container">
            </div>
    </section>
    <section id="hakkimda" class="container py-4 my-4">
        <div class="row justify-content-center">
            <div class="col-lg-8 text-center">
                <h2 class="mb-4 pb-2 border-bottom fw-bold text-dark d-inline-block">Hakkımda</h2>
                <p class="lead text-muted mt-2">
                    Merhaba, ben Sami. Bursa'da yaşayan ve bilim kurguyu mühendisliğe dönüştürmeyi hedefleyen bir araştırmacıyım. TEKNOFEST ve MILSET gibi uluslararası arenalar için otonom sistemler tasarlıyor, Bambu Lab A1 ile fonksiyonel donanımlar modelliyorum. Temel amacım, edindiğim Python tabanlı algoritmik düşünce yeteneğini, yapay zeka entegrasyonları ve robotik prototiplerimle birleştirerek geleceğin teknolojilerini bugünden inşa etmek.
                </p>
            </div>
        </div>
    </section>
    <section id="projeler" class="container py-4 my-4">
        <h2 class="mb-4 pb-2 border-bottom fw-bold text-dark">Donanım ve Yazılım Projelerim</h2>
        <div class="row g-4" id="projects-container">
            </div>
    </section>
    <section id="gunluk" class="container py-5 my-4 bg-white rounded-4 shadow-sm border border-light p-4">
        <div class="d-flex justify-content-between align-items-center mb-4 pb-2 border-bottom">
            <h2 class="fw-bold text-dark mb-0">Laboratuvar Günlüğü</h2>
            <span class="badge bg-primary rounded-pill px-3 py-2">Haftalık Notlar</span>
        </div>
        <div class="row g-4" id="blog-container">
            </div>
    </section>
    <section id="iletisim" class="container py-5 my-4">
        <div class="row justify-content-center">
            <div class="col-lg-8">
                <h2 class="mb-4 pb-2 border-bottom fw-bold text-dark text-center">Benimle İletişime Geç</h2>
                <p class="text-center text-muted mb-4">Projelerim hakkında yorum yapmak, fikir paylaşmak veya birlikte çalışmak için aşağıdaki formu kullanabilirsiniz.</p>
                
                <div class="card border-0 shadow-sm rounded-4 p-4 bg-white">
                    <form action="https://formsubmit.co/0ae4ba60424252eaa58fdfe0bb0a9527" method="POST">
                        <input type="hidden" name="_subject" value="Make3D Lab'dan Yeni Bir Mesaj Var!">
                        <input type="hidden" name="_captcha" value="false">
                        <input type="hidden" name="_template" value="table">

                        <div class="row g-3 mb-3">
                            <div class="col-md-6">
                                <label for="isim" class="form-label fw-bold">Adınız</label>
                                <input type="text" name="isim" class="form-control rounded-pill" id="isim" placeholder="Sisteme nasıl kaydedelim?" required>
                            </div>
                            <div class="col-md-6">
                                <label for="eposta" class="form-label fw-bold">E-Posta (İsteğe Bağlı)</label>
                                <input type="email" name="eposta" class="form-control rounded-pill" id="eposta" placeholder="Size ulaşabilmem için">
                            </div>
                        </div>
                        <div class="mb-4">
                            <label for="mesaj" class="form-label fw-bold">Mesajınız veya Yorumunuz</label>
                            <textarea name="mesaj" class="form-control rounded-4" id="mesaj" rows="4" placeholder="Düşüncelerinizi buraya yazın..." required></textarea>
                        </div>
                        <div class="text-end">
                            <button type="submit" class="btn btn-primary px-5 rounded-pill shadow-sm">Sisteme İlet</button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </section>
    <footer class="bg-dark text-white py-4 mt-auto">
        <div class="container d-flex flex-column flex-md-row justify-content-between align-items-center gap-3">
            <p class="mb-0 fw-light text-secondary text-center text-md-start">
                © 2026 Make3D Lab. Tüm otonom sistemler ve tasarımlar <span class="fw-bold text-primary">Bootstrap 5</span> ile kodlanmıştır.
            </p>
            <a id="youtube-footer-link" href="#" target="_blank" rel="noopener noreferrer" class="text-danger text-decoration-none fw-bold small d-inline-flex align-items-center gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-youtube" viewBox="0 0 16 16">
                    <path d="M8.051 1.999h.089c.822.003 4.987.033 6.11.335a2.01 2.01 0 0 1 1.415 1.42c.101.38.172.883.22 1.402l.01.104.022.26.008.104c.065.914.073 1.77.074 1.957v.075c-.001.194-.01 1.053-.075 1.966l-.01.104-.022.26-.008.104a16.5 16.5 0 0 1-.22 1.401 2.01 2.01 0 0 1-1.415 1.42c-1.123.302-5.288.332-6.11.335H8.05a16.5 16.5 0 0 1-6.112-.335 2.01 2.01 0 0 1-1.415-1.42 16.5 16.5 0 0 1-.22-1.401l-.01-.104-.022.26-.008-.104c-.065-.914-.073-1.77-.074-1.957v-.075c.001-.194.01-1.053.075-1.966l.01-.104.022.26.008-.104a16.5 16.5 0 0 1 .22-1.402 2.01 2.01 0 0 1 1.415-1.42c1.123-.302 5.288-.332 6.11-.335zM6.5 5.201v5.596L11 8 6.5 5.201z"/>
                </svg>
                Make3D Lab’ı YouTube'da Takip Edin
            </a>
        </div>
    </footer>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>

    <script>
        const MAKE3D_LAB_DATA = {
            // 1. SOSYAL MEDYA LİNKLERİ
            youtubeKanalLinki: "https://youtube.com/@make3dlab?si=EDNlSLUv3PYKL7en",

            // 2. CANLI ATÖLYE DURUMU
            atolyeDurumu: "Bambu Lab A1 Boşta",

            // 3. İSTATİSTİKLER PANELİ
            istatistikler: [
                { rakam: "3+", baslik: "Aktif Otonom Sistem", renkSinifi: "text-primary" },
                { rakam: "1000+", baslik: "Saat 3D Baskı Süresi", renkSinifi: "text-success" },
                { rakam: "50+", baslik: "Geliştirilmiş Python Algoritması", renkSinifi: "text-info" }
            ],

            // 4. PROJE KARTLARI VERİ SETİ
            projeler: [
                {
                    kategori: "Robotik & İHA",
                    kategoriRenk: "bg-danger",
                    baslik: "EduGuard Otonom Hexacopter",
                    aciklama: "Okul güvenliği için tasarlanan, YOLOv8 ile otonom görüntü işleme yeteneklerine sahip hexacopter drone sisteminin geliştirme ve raporlama süreçleri."
                },
                {
                    kategori: "Hızlı Prototipleme",
                    kategoriRenk: "bg-success",
                    baslik: "AR Gözlük ve 3D Üretim",
                    aciklama: "Raspberry Pi 4 ve OLED ekranlar kullanılarak optik yolu tasarlanan Artırılmış Gerçeklik gözlüğü prototipi. Fusion 360 tasarımlarım ve Bambu Lab A1 baskı parametreleri."
                },
                {
                    kategori: "Yapay Zeka ve Algoritma",
                    kategoriRenk: "bg-info text-dark",
                    baslik: "Yazılım Geliştirme Eğitimi",
                    aciklama: "Python ile E.L.I.O. entegrasyonları üzerine çalışmalarım, yerel dil modelleri ve ileri düzey Python algoritmaları üzerine sistem tasarımları."
                }
            ],

            // 5. LABORATUVAR GÜNLÜĞÜ (BLOG) YAZILARI
            blogYazilari: [
                {
                    tarih: "7 Haziran 2026",
                    kategori: "Sistem Kurulumu",
                    baslik: "Make3D Lab'ın Dijital Üssü Kuruldu: İlk Kodlar Yayında!",
                    ozet: "Bu hafta atölyemdeki otonom sistemleri, Python tabanlı algoritmaları ve 3D tasarımlarımı dış dünyayla paylaşabilmek adına kişisel portföy sitemin inşasına başladım. Yapay zeka asistanım E.L.I.O. ile birlikte HTML5, Bootstrap 5 ve dinamik bir JavaScript mimarisi kullanarak tek sayfada tüm verilerimi yönetebileceğim bir sistem tasarladık. Firebase Realtime Database entegrasyonu için de ilk adımları atmış bulunuyorum. Testler başarılı, sistem aktif!",
                    resimUrl: "https://images.unsplash.com/photo-1555066931-4365d14bab8c?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80"
                }
            ]
        };

        // DOM Rendering Engine (Verileri HTML şablonuna basan motor)
        document.addEventListener("DOMContentLoaded", function() {
            // Link atamaları
            document.getElementById("youtube-hero-btn").href = MAKE3D_LAB_DATA.youtubeKanalLinki;
            document.getElementById("youtube-footer-link").href = MAKE3D_LAB_DATA.youtubeKanalLinki;

            // Atölye durum güncellemesi
            document.getElementById("live-status-text").innerText = MAKE3D_LAB_DATA.atolyeDurumu;

            // İstatistikleri ekrana bas
            const statsContainer = document.getElementById("stats-container");
            MAKE3D_LAB_DATA.istatistikler.forEach(stat => {
                statsContainer.innerHTML += `
                    <div class="col-md-4">
                        <div class="bg-white p-4 rounded-4 shadow-sm border border-light">
                            <h3 class="display-5 fw-bold ${stat.renkSinifi}">${stat.rakam}</h3>
                            <p class="text-muted mb-0 small fw-medium">${stat.baslik}</p>
                        </div>
                    </div>
                `;
            });

            // Proje kartlarını ekrana bas (Butonlar Kaldırıldı)
            const projectsContainer = document.getElementById("projects-container");
            MAKE3D_LAB_DATA.projeler.forEach(proje => {
                projectsContainer.innerHTML += `
                    <div class="col-md-4">
                        <div class="card h-100 border-0 shadow-sm rounded-4 overflow-hidden">
                            <div class="card-body">
                                <span class="badge ${proje.kategoriRenk} mb-2">${proje.kategori}</span>
                                <h5 class="card-title fw-bold">${proje.baslik}</h5>
                                <p class="card-text text-muted">${proje.aciklama}</p>
                            </div>
                        </div>
                    </div>
                `;
            });

            // Blog yazılarını ekrana dinamik bas (Butonlar Kaldırıldı)
            const blogContainer = document.getElementById("blog-container");
            MAKE3D_LAB_DATA.blogYazilari.forEach(yazi => {
                blogContainer.innerHTML += `
                    <div class="col-md-6 col-lg-4">
                        <div class="card h-100 border-0 shadow-none bg-light rounded-4 overflow-hidden">
                            <img src="${yazi.resimUrl}" class="card-img-top" alt="Blog Görseli" style="height: 180px; object-fit: cover;">
                            <div class="card-body p-4">
                                <div class="d-flex justify-content-between align-items-center mb-3">
                                    <span class="badge bg-secondary-subtle text-secondary border">${yazi.kategori}</span>
                                    <small class="text-muted fw-medium">${yazi.tarih}</small>
                                </div>
                                <h5 class="card-title fw-bold text-dark">${yazi.baslik}</h5>
                                <p class="card-text text-muted small">${yazi.ozet}</p>
                            </div>
                        </div>
                    </div>
                `;
            });
        });
    </script>
</body>
</html>
