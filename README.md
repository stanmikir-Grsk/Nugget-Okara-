<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nugget Okara - Gurih & Lembut</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;800&family=Nunito:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #0a0a0a;
            color: #f0f0f0;
            min-height: 100vh;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
    </style>
</head>
<body>
    <div class="background-texture"></div>
    <div class="wood-overlay"></div>
    
    <div class="container">
        <!-- Konten akan ditambahkan di bagian berikutnya -->
    </div>
    
    <!-- Modal untuk input password -->
    <div class="password-modal" id="passwordModal">
        <div class="password-form">
            <h3><i class="fas fa-lock"></i> Unggah Foto Nugget Anda</h3>
            <p>Masukkan sandi untuk mengunggah foto nugget Anda sendiri:</p>
            <input type="password" class="password-input" id="passwordInput" placeholder="Masukkan sandi...">
            <button class="password-submit" id="passwordSubmit">Unggah Foto</button>
            <p style="margin-top: 15px; font-size: 0.9rem; color: #8899aa;">Sandi: nugget66</p>
        </div>
    </div>
    
    <script>
        // JavaScript akan ditambahkan di bagian akhir
    </script>
</body>
</html>
<style>
    /* Background dengan tekstur kayu hitam ke abu-abuan */
    .background-texture {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: 
            radial-gradient(circle at 15% 15%, rgba(50, 50, 50, 0.15) 2px, transparent 2px),
            radial-gradient(circle at 85% 85%, rgba(60, 60, 60, 0.1) 2px, transparent 2px),
            linear-gradient(135deg, #0f0f0f 0%, #1a1a1a 50%, #0f0f0f 100%);
        background-size: 80px 80px, 80px 80px, 100% 100%;
        z-index: -2;
    }
    
    .wood-overlay {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: 
            linear-gradient(rgba(15, 15, 15, 0.85), rgba(8, 8, 8, 0.92)),
            url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="200" height="200" viewBox="0 0 200 200"><path d="M0,0 L200,0 L200,200 L0,200 Z" fill="none" stroke="%23222" stroke-width="1"/><path d="M20,0 L20,200 M40,0 L40,200 M60,0 L60,200 M80,0 L80,200 M100,0 L100,200 M120,0 L120,200 M140,0 L140,200 M160,0 L160,200 M180,0 L180,200" stroke="%23333" stroke-width="0.5"/></svg>');
        background-size: 200px 200px;
        opacity: 0.95;
        z-index: -1;
    }
</style>
<header class="main-header">
    <div class="logo-container">
        <div class="penguin-icon">
            <i class="fas fa-fish"></i>
            <div class="penguin-eye"></div>
        </div>
        <h1 class="main-title">NUGGET OKARA</h1>
        <p class="subtitle">Rasa Premium, Harga Bersahabat</p>
    </div>
</header>

<style>
    .main-header {
        text-align: center;
        padding: 60px 0 40px;
        position: relative;
    }
    
    .logo-container {
        position: relative;
        display: inline-block;
        margin-bottom: 30px;
    }
    
    .penguin-icon {
        position: absolute;
        top: -40px;
        right: -60px;
        width: 80px;
        height: 80px;
        background: linear-gradient(135deg, #0a1929, #1a3a5f);
        border-radius: 50% 50% 45% 45%;
        display: flex;
        align-items: center;
        justify-content: center;
        color: #a0e7ff;
        font-size: 40px;
        transform: rotate(-10deg);
        box-shadow: 0 10px 25px rgba(0, 0, 0, 0.5), 0 0 20px rgba(42, 157, 255, 0.3);
        animation: float 3s ease-in-out infinite;
        z-index: 10;
        overflow: hidden;
    }
    
    .penguin-icon::before {
        content: '';
        position: absolute;
        top: 15px;
        left: 25px;
        width: 20px;
        height: 20px;
        background: white;
        border-radius: 50%;
        opacity: 0.9;
    }
    
    .penguin-eye {
        position: absolute;
        top: 20px;
        left: 30px;
        width: 10px;
        height: 10px;
        background: #0a1929;
        border-radius: 50%;
        z-index: 2;
    }
    
    @keyframes float {
        0%, 100% { 
            transform: translateY(0) rotate(-10deg) scale(1); 
        }
        50% { 
            transform: translateY(-20px) rotate(5deg) scale(1.05); 
        }
    }
    
    .main-title {
        font-size: 5rem;
        font-weight: 800;
        letter-spacing: 4px;
        background: linear-gradient(135deg, 
            #a0e7ff 0%, 
            #6bc8ff 20%, 
            #2a9dff 40%, 
            #0066cc 60%, 
            #003d99 80%, 
            #001f4d 100%);
        -webkit-background-clip: text;
        background-clip: text;
        color: transparent;
        text-shadow: 
            0 5px 15px rgba(42, 157, 255, 0.2),
            0 0 40px rgba(42, 157, 255, 0.1);
        padding: 15px 0;
        position: relative;
        display: inline-block;
        font-family: 'Nunito', sans-serif;
    }
    
    .main-title::after {
        content: '';
        position: absolute;
        bottom: 0;
        left: 5%;
        width: 90%;
        height: 4px;
        background: linear-gradient(90deg, 
            transparent, 
            #2a9dff 20%, 
            #6bc8ff 50%, 
            #2a9dff 80%, 
            transparent);
        border-radius: 2px;
    }
    
    .subtitle {
        font-size: 1.5rem;
        color: #d0f0ff;
        margin-top: 20px;
        font-weight: 300;
        letter-spacing: 2px;
        opacity: 0.9;
    }
    
    @media (max-width: 768px) {
        .main-title {
            font-size: 3.5rem;
            letter-spacing: 2px;
        }
        
        .penguin-icon {
            top: -30px;
            right: -40px;
            width: 60px;
            height: 60px;
            font-size: 30px;
        }
    }
</style>
<section class="nugget-images">
    <h2 class="section-title">Kesempurnaan Rasa dalam Setiap Gigitan</h2>
    <div class="image-grid">
        <div class="image-card" id="nugget1">
            <div class="image-wrapper">
                <img src="https://images.unsplash.com/photo-1613564834361-9436948817d1?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" 
                     alt="Nugget Okara Crispy" class="nugget-img" id="img1">
                <div class="image-overlay">
                    <i class="fas fa-camera"></i>
                    <span>Klik untuk upload foto Anda</span>
                </div>
            </div>
            <p class="image-label">Nugget Okara Crispy</p>
        </div>
        
        <div class="image-card" id="nugget2">
            <div class="image-wrapper">
                <img src="https://images.unsplash.com/photo-1563379926898-05f4575a45d8?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" 
                     alt="Nugget Okara Lembut" class="nugget-img" id="img2">
                <div class="image-overlay">
                    <i class="fas fa-camera"></i>
                    <span>Klik untuk upload foto Anda</span>
                </div>
            </div>
            <p class="image-label">Nugget Okara Lembut</p>
        </div>
    </div>
    <p class="upload-note">
        <i class="fas fa-key"></i> Password: nugget66
    </p>
</section>

<style>
    .nugget-images {
        margin: 60px 0;
        text-align: center;
    }
    
    .section-title {
        font-size: 2.2rem;
        color: #a0e7ff;
        margin-bottom: 40px;
        font-weight: 600;
        text-shadow: 0 0 10px rgba(160, 231, 255, 0.3);
    }
    
    .image-grid {
        display: flex;
        justify-content: center;
        gap: 40px;
        flex-wrap: wrap;
        margin-bottom: 20px;
    }
    
    .image-card {
        width: 350px;
        cursor: pointer;
        transition: transform 0.4s;
    }
    
    .image-card:hover {
        transform: translateY(-10px);
    }
    
    .image-wrapper {
        position: relative;
        width: 100%;
        height: 300px;
        border-radius: 20px;
        overflow: hidden;
        box-shadow: 
            0 15px 35px rgba(0, 0, 0, 0.4),
            0 0 30px rgba(42, 157, 255, 0.2);
        border: 3px solid rgba(160, 231, 255, 0.15);
    }
    
    .nugget-img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        transition: transform 0.6s;
    }
    
    .image-card:hover .nugget-img {
        transform: scale(1.08);
    }
    
    .image-overlay {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: linear-gradient(135deg, 
            rgba(42, 157, 255, 0.1), 
            rgba(0, 102, 204, 0.2));
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        opacity: 0;
        transition: opacity 0.4s;
        color: white;
        font-size: 1.2rem;
    }
    
    .image-card:hover .image-overlay {
        opacity: 1;
    }
    
    .image-overlay i {
        font-size: 3rem;
        margin-bottom: 15px;
        color: #a0e7ff;
    }
    
    .image-label {
        margin-top: 20px;
        font-size: 1.4rem;
        color: #d0f0ff;
        font-weight: 500;
    }
    
    .upload-note {
        color: #6bc8ff;
        font-size: 1.1rem;
        margin-top: 10px;
        font-style: italic;
    }
</style>
<section class="composition-section">
    <h2 class="section-title">🍽️ Komposisi Premium</h2>
    <div class="composition-container">
        <div class="ingredient-list">
            <div class="ingredient-item">
                <div class="ingredient-icon">🥛</div>
                <div class="ingredient-content">
                    <h3>Okara (Ampas Kedelai)</h3>
                    <p>Sumber protein nabati berkualitas tinggi</p>
                </div>
            </div>
            
            <div class="ingredient-item">
                <div class="ingredient-icon">🍗</div>
                <div class="ingredient-content">
                    <h3>Ayam Giling</h3>
                    <p>Daging ayam pilihan yang digiling halus</p>
                </div>
            </div>
            
            <div class="ingredient-item">
                <div class="ingredient-icon">🥚</div>
                <div class="ingredient-content">
                    <h3>Telur</h3>
                    <p>Pengikat alami dan sumber nutrisi</p>
                </div>
            </div>
            
            <div class="ingredient-item">
                <div class="ingredient-icon">💧</div>
                <div class="ingredient-content">
                    <h3>Air</h3>
                    <p>Keseimbangan tekstur yang sempurna</p>
                </div>
            </div>
            
            <div class="ingredient-item">
                <div class="ingredient-icon">🧂</div>
                <div class="ingredient-content">
                    <h3>Garam</h3>
                    <p>Penyeimbang rasa alami</p>
                </div>
            </div>
            
            <div class="ingredient-item">
                <div class="ingredient-icon">🌽</div>
                <div class="ingredient-content">
                    <h3>Tepung Maizena</h3>
                    <p>Memberikan kerenyahan maksimal</p>
                </div>
            </div>
            
            <div class="ingredient-item">
                <div class="ingredient-icon">🍠</div>
                <div class="ingredient-content">
                    <h3>Tepung Tapioka</h3>
                    <p>Tekstur kenyal yang menyenangkan</p>
                </div>
            </div>
            
            <div class="ingredient-item">
                <div class="ingredient-icon">🍞</div>
                <div class="ingredient-content">
                    <h3>Tepung Roti (Panir)</h3>
                    <p>Lapisan crispy golden brown</p>
                </div>
            </div>
            
            <div class="ingredient-item">
                <div class="ingredient-icon">✨</div>
                <div class="ingredient-content">
                    <h3>MSG (Penguat Rasa)</h3>
                    <p>Sedikit saja untuk kesempurnaan rasa</p>
                </div>
            </div>
        </div>
        
        <div class="composition-fact">
            <div class="fact-card">
                <div class="fact-icon">👨‍🍳</div>
                <h3>Dioles dengan Cinta</h3>
                <p>Setiap nugget dibuat dengan perhatian khusus untuk memastikan kualitas terbaik</p>
            </div>
            
            <div class="fact-card">
                <div class="fact-icon">🚫</div>
                <h3>Tanpa Pengawet</h3>
                <p>100% bahan alami tanpa tambahan pengawet kimia</p>
            </div>
        </div>
    </div>
</section>

<style>
    .composition-section {
        margin: 80px 0;
        padding: 40px;
        background: rgba(20, 30, 50, 0.3);
        border-radius: 30px;
        border: 2px solid rgba(160, 231, 255, 0.1);
        box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
    }
    
    .composition-container {
        display: flex;
        gap: 40px;
        flex-wrap: wrap;
        justify-content: center;
    }
    
    .ingredient-list {
        flex: 1;
        min-width: 300px;
        max-width: 600px;
    }
    
    .ingredient-item {
        display: flex;
        align-items: center;
        background: rgba(255, 255, 255, 0.05);
        padding: 20px;
        margin-bottom: 15px;
        border-radius: 15px;
        transition: all 0.3s;
        border-left: 4px solid #2a9dff;
    }
    
    .ingredient-item:hover {
        background: rgba(42, 157, 255, 0.1);
        transform: translateX(10px);
        box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
    }
    
    .ingredient-icon {
        font-size: 2.5rem;
        margin-right: 20px;
        min-width: 60px;
        text-align: center;
    }
    
    .ingredient-content h3 {
        color: #a0e7ff;
        font-size: 1.3rem;
        margin-bottom: 5px;
    }
    
    .ingredient-content p {
        color: #b0c0d0;
        font-size: 0.95rem;
        opacity: 0.8;
    }
    
    .composition-fact {
        flex: 1;
        min-width: 300px;
        max-width: 400px;
    }
    
    .fact-card {
        background: rgba(30, 40, 60, 0.5);
        padding: 30px;
        border-radius: 20px;
        margin-bottom: 20px;
        text-align: center;
        border: 2px solid rgba(160, 231, 255, 0.2);
        transition: all 0.3s;
    }
    
    .fact-card:hover {
        transform: translateY(-10px);
        box-shadow: 0 15px 30px rgba(0, 0, 0, 0.4);
        border-color: #2a9dff;
    }
    
    .fact-icon {
        font-size: 3.5rem;
        margin-bottom: 15px;
    }
    
    .fact-card h3 {
        color: #6bc8ff;
        margin-bottom: 10px;
        font-size: 1.5rem;
    }
    
    .fact-card p {
        color: #d0e0f0;
        line-height: 1.6;
    }
</style>
<section class="sticker-section">
    <div class="sticker-container">
        <div class="penguin-animation">
            <div class="penguin-body">
                <div class="penguin-face">
                    <div class="eye left"></div>
                    <div class="eye right"></div>
                    <div class="beak"></div>
                </div>
                <div class="penguin-arm left"></div>
                <div class="penguin-arm right"></div>
                <div class="penguin-feet"></div>
                <div class="fish">🐟</div>
            </div>
        </div>
        
        <div class="tagline-container">
            <div class="tagline-card">
                <div class="tagline-icon">🔥</div>
                <h3>Gurih di Luar, Lembut di Dalam</h3>
                <p>Kombinasi sempurna antara crispy luar dan lembut dalam</p>
            </div>
            
            <div class="tagline-card">
                <div class="tagline-icon">💰</div>
                <h3>Enak + Hemat</h3>
                <p>Rasa premium dengan harga yang bersahabat untuk semua</p>
            </div>
            
            <div class="tagline-card">
                <div class="tagline-icon">❄️</div>
                <h3>Frozen - Praktis tinggal goreng</h3>
                <p>Simpan beku, goreng kapan saja. Praktis untuk segala situasi!</p>
            </div>
        </div>
    </div>
</section>

<style>
    .sticker-section {
        margin: 100px 0;
        position: relative;
    }
    
    .sticker-container {
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 60px;
        flex-wrap: wrap;
    }
    
    .penguin-animation {
        position: relative;
        width: 300px;
        height: 350px;
    }
    
    .penguin-body {
        position: absolute;
        width: 200px;
        height: 280px;
        background: linear-gradient(135deg, #0a1929, #1a3a5f);
        border-radius: 100px 100px 90px 90px;
        top: 0;
        left: 50px;
        animation: penguin-dance 4s infinite alternate;
        box-shadow: 
            0 20px 40px rgba(0, 0, 0, 0.4),
            0 0 30px rgba(42, 157, 255, 0.2);
    }
    
    @keyframes penguin-dance {
        0%, 100% { 
            transform: translateY(0) rotate(0); 
        }
        25% { 
            transform: translateY(-20px) rotate(-5deg); 
        }
        50% { 
            transform: translateY(-10px) rotate(5deg); 
        }
        75% { 
            transform: translateY(-15px) rotate(-3deg); 
        }
    }
    
    .penguin-face {
        position: absolute;
        top: 50px;
        left: 50%;
        transform: translateX(-50%);
        width: 120px;
        height: 100px;
    }
    
    .eye {
        position: absolute;
        width: 25px;
        height: 25px;
        background: white;
        border-radius: 50%;
        top: 20px;
    }
    
    .eye.left {
        left: 20px;
    }
    
    .eye.right {
        right: 20px;
    }
    
    .eye::after {
        content: '';
        position: absolute;
        width: 10px;
        height: 10px;
        background: #0a1929;
        border-radius: 50%;
        top: 7px;
        left: 7px;
    }
    
    .beak {
        position: absolute;
        width: 40px;
        height: 20px;
        background: #FFA500;
        border-radius: 50%;
        top: 60px;
        left: 50%;
        transform: translateX(-50%);
    }
    
    .penguin-arm {
        position: absolute;
        width: 40px;
        height: 100px;
        background: #0a1929;
        border-radius: 20px;
        top: 100px;
    }
    
    .penguin-arm.left {
        left: -20px;
        transform: rotate(30deg);
        animation: arm-wave-left 3s infinite alternate;
    }
    
    .penguin-arm.right {
        right: -20px;
        transform: rotate(-30deg);
        animation: arm-wave-right 3s infinite alternate 0.5s;
    }
    
    @keyframes arm-wave-left {
        0%, 100% { transform: rotate(30deg); }
        50% { transform: rotate(10deg); }
    }
    
    @keyframes arm-wave-right {
        0%, 100% { transform: rotate(-30deg); }
        50% { transform: rotate(-10deg); }
    }
    
    .penguin-feet {
        position: absolute;
        width: 120px;
        height: 30px;
        background: #FFA500;
        border-radius: 50%;
        bottom: 10px;
        left: 50%;
        transform: translateX(-50%);
    }
    
    .fish {
        position: absolute;
        font-size: 40px;
        top: 100px;
        right: -40px;
        animation: fish-float 3s infinite alternate;
    }
    
    @keyframes fish-float {
        0%, 100% { transform: translateY(0) rotate(0); }
        50% { transform: translateY(-20px) rotate(20deg); }
    }
    
    .tagline-container {
        flex: 1;
        min-width: 300px;
        max-width: 500px;
    }
    
    .tagline-card {
        background: rgba(30, 40, 60, 0.6);
        padding: 25px;
        margin-bottom: 25px;
        border-radius: 20px;
        border-left: 5px solid #2a9dff;
        transition: all 0.3s;
        box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
    }
    
    .tagline-card:hover {
        transform: translateX(15px);
        background: rgba(42, 157, 255, 0.1);
        box-shadow: 0 15px 35px rgba(0, 0, 0, 0.4);
    }
    
    .tagline-icon {
        font-size: 2.5rem;
        margin-bottom: 15px;
    }
    
    .tagline-card h3 {
        color: #a0e7ff;
        font-size: 1.6rem;
        margin-bottom: 10px;
    }
    
    .tagline-card p {
        color: #d0e0f0;
        line-height: 1.6;
        opacity: 0.9;
    }
</style>
<section class="price-section">
    <div class="price-container">
        <div class="price-header">
            <h2 class="price-title">💵 Harga Terjangkau</h2>
            <p class="price-subtitle">Kualitas premium dengan harga yang membuat Anda tersenyum</p>
        </div>
        
        <div class="price-display">
            <div class="price-main">
                <span class="currency">Rp</span>
                <span class="amount">3K</span>
                <span class="separator">-</span>
                <span class="amount">5K</span>
            </div>
            <p class="price-note">Mulai dari per porsi</p>
        </div>
        
        <div class="price-features">
            <div class="feature">
                <i class="fas fa-box-open"></i>
                <span>Packaging Higienis</span>
            </div>
            <div class="feature">
                <i class="fas fa-shipping-fast"></i>
                <span>Bisa Dikirim</span>
            </div>
            <div class="feature">
                <i class="fas fa-store"></i>
                <span>Tersedia Frozen</span>
            </div>
        </div>
    </div>
</section>

<style>
    .price-section {
        margin: 80px 0;
        position: relative;
    }
    
    .price-container {
        background: linear-gradient(135deg, 
            rgba(20, 30, 50, 0.8), 
            rgba(10, 20, 40, 0.9));
        padding: 50px 40px;
        border-radius: 30px;
        text-align: center;
        border: 3px solid rgba(42, 157, 255, 0.3);
        box-shadow: 
            0 25px 50px rgba(0, 0, 0, 0.4),
            0 0 50px rgba(42, 157, 255, 0.1);
        position: relative;
        overflow: hidden;
    }
    
    .price-container::before {
        content: '';
        position: absolute;
        top: -50%;
        left: -50%;
        width: 200%;
        height: 200%;
        background: linear-gradient(45deg, 
            transparent 20%, 
            rgba(42, 157, 255, 0.05) 50%, 
            transparent 80%);
        animation: shine 8s infinite linear;
        z-index: 0;
    }
    
    @keyframes shine {
        0% { transform: rotate(0deg); }
        100% { transform: rotate(360deg); }
    }
    
    .price-header {
        position: relative;
        z-index: 1;
        margin-bottom: 40px;
    }
    
    .price-title {
        font-size: 3rem;
        color: #a0e7ff;
        margin-bottom: 15px;
        text-shadow: 0 0 20px rgba(160, 231, 255, 0.5);
    }
    
    .price-subtitle {
        font-size: 1.3rem;
        color: #b0c0d0;
        max-width: 600px;
        margin: 0 auto;
    }
    
    .price-display {
        position: relative;
        z-index: 1;
        margin: 40px 0;
    }
    
    .price-main {
        font-size: 6rem;
        font-weight: 800;
        background: linear-gradient(135deg, 
            #a0e7ff 0%, 
            #6bc8ff 25%, 
            #2a9dff 50%, 
            #0066cc 75%);
        -webkit-background-clip: text;
        background-clip: text;
        color: transparent;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-wrap: wrap;
        gap: 10px;
        text-shadow: 0 0 40px rgba(42, 157, 255, 0.3);
    }
    
    .currency {
        font-size: 3rem;
        align-self: flex-start;
        margin-top: 15px;
    }
    
    .separator {
        font-size: 5rem;
        color: #6bc8ff;
    }
    
    .price-note {
        color: #d0e0f0;
        font-size: 1.2rem;
        margin-top: 15px;
        font-style: italic;
    }
    
    .price-features {
        display: flex;
        justify-content: center;
        gap: 40px;
        flex-wrap: wrap;
        margin-top: 50px;
        position: relative;
        z-index: 1;
    }
    
    .price-features .feature {
        display: flex;
        align-items: center;
        gap: 15px;
        background: rgba(255, 255, 255, 0.05);
        padding: 20px 30px;
        border-radius: 15px;
        transition: all 0.3s;
    }
    
    .price-features .feature:hover {
        background: rgba(42, 157, 255, 0.15);
        transform: translateY(-5px);
        box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
    }
    
    .price-features .feature i {
        font-size: 1.8rem;
        color: #6bc8ff;
    }
    
    .price-features .feature span {
        font-size: 1.2rem;
        color: #d0e0f0;
        font-weight: 500;
    }
    
    @media (max-width: 768px) {
        .price-main {
            font-size: 4rem;
        }
        
        .price-title {
            font-size: 2.5rem;
        }
    }
</style>
<section class="contact-section">
    <h2 class="section-title">📞 Pesan Sekarang!</h2>
    <p class="contact-subtitle">Hubungi kami via WhatsApp atau kunjungi Instagram untuk informasi lebih lanjut</p>
    
    <div class="contact-buttons">
        <a href="https://wa.me/6282142442134?text=Halo,%20saya%20tertarik%20dengan%20Nugget%20Okara!" 
           target="_blank" 
           class="contact-btn whatsapp-btn">
            <div class="btn-icon">
                <i class="fab fa-whatsapp"></i>
            </div>
            <div class="btn-content">
                <h3>WhatsApp</h3>
                <p>+62 821 4244 2134</p>
                <span class="btn-action">Klik untuk Chat</span>
            </div>
        </a>
        
        <a href="https://www.instagram.com/stan_mikir?igsh=cnpnMm90NzRpcnZ2" 
           target="_blank" 
           class="contact-btn instagram-btn">
            <div class="btn-icon">
                <i class="fab fa-instagram"></i>
            </div>
            <div class="btn-content">
                <h3>Instagram</h3>
                <p>@stan_mikir</p>
                <span class="btn-action">Klik untuk Follow</span>
            </div>
        </a>
    </div>
    
    <div class="contact-info">
        <div class="info-card">
            <i class="fas fa-clock"></i>
            <h4>Waktu Respon Cepat</h4>
            <p>Biasanya merespon dalam beberapa menit</p>
        </div>
        
        <div class="info-card">
            <i class="fas fa-concierge-bell"></i>
            <h4>Layanan Ramah</h4>
            <p>Siap membantu dengan senang hati</p>
        </div>
        
        <div class="info-card">
            <i class="fas fa-truck"></i>
            <h4>Bisa Dikirim</h4>
            <p>Tersedia pengiriman sesuai area</p>
        </div>
    </div>
</section>

<style>
    .contact-section {
        margin: 100px 0 60px;
        text-align: center;
    }
    
    .contact-subtitle {
        font-size: 1.3rem;
        color: #b0c0d0;
        max-width: 700px;
        margin: 20px auto 50px;
        line-height: 1.6;
    }
    
    .contact-buttons {
        display: flex;
        justify-content: center;
        gap: 40px;
        flex-wrap: wrap;
        margin-bottom: 60px;
    }
    
    .contact-btn {
        width: 350px;
        text-decoration: none;
        border-radius: 25px;
        padding: 30px;
        display: flex;
        align-items: center;
        gap: 25px;
        transition: all 0.4s;
        position: relative;
        overflow: hidden;
        box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
    }
    
    .contact-btn::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: linear-gradient(135deg, 
            rgba(255, 255, 255, 0.1), 
            transparent 30%);
        z-index: 1;
    }
    
    .whatsapp-btn {
        background: linear-gradient(135deg, #25D366, #128C7E);
    }
    
    .instagram-btn {
        background: linear-gradient(135deg, #E4405F, #833AB4);
    }
    
    .contact-btn:hover {
        transform: translateY(-15px) scale(1.03);
        box-shadow: 
            0 30px 60px rgba(0, 0, 0, 0.4),
            0 0 40px rgba(255, 255, 255, 0.1);
    }
    
    .btn-icon {
        font-size: 3.5rem;
        color: white;
        z-index: 2;
        flex-shrink: 0;
    }
    
    .btn-content {
        text-align: left;
        z-index: 2;
        flex-grow: 1;
    }
    
    .btn-content h3 {
        font-size: 1.8rem;
        color: white;
        margin-bottom: 5px;
    }
    
    .btn-content p {
        font-size: 1.2rem;
        color: rgba(255, 255, 255, 0.9);
        margin-bottom: 10px;
    }
    
    .btn-action {
        display: inline-block;
        background: rgba(255, 255, 255, 0.2);
        padding: 8px 15px;
        border-radius: 20px;
        font-size: 0.9rem;
        color: white;
        font-weight: 600;
        transition: all 0.3s;
    }
    
    .contact-btn:hover .btn-action {
        background: rgba(255, 255, 255, 0.3);
        transform: translateX(10px);
    }
    
    .contact-info {
        display: flex;
        justify-content: center;
        gap: 30px;
        flex-wrap: wrap;
        margin-top: 50px;
    }
    
    .info-card {
        background: rgba(30, 40, 60, 0.5);
        padding: 25px;
        border-radius: 20px;
        width: 250px;
        transition: all 0.3s;
        border: 2px solid rgba(160, 231, 255, 0.1);
    }
    
    .info-card:hover {
        transform: translateY(-10px);
        background: rgba(42, 157, 255, 0.1);
        border-color: #2a9dff;
        box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3);
    }
    
    .info-card i {
        font-size: 2.5rem;
        color: #6bc8ff;
        margin-bottom: 15px;
    }
    
    .info-card h4 {
        color: #a0e7ff;
        margin-bottom: 10px;
        font-size: 1.3rem;
    }
    
    .info-card p {
        color: #d0e0f0;
        font-size: 0.95rem;
        line-height: 1.5;
    }
</style>
<footer class="main-footer">
    <div class="footer-content">
        <div class="footer-logo">
            <div class="footer-penguin">🐧</div>
            <h2>NUGGET OKARA</h2>
            <p>Gurih di Luar, Lembut di Dalam</p>
        </div>
        
        <div class="footer-info">
            <div class="info-column">
                <h3>Kontak</h3>
                <p><i class="fas fa-phone"></i> WA: +62 821 4244 2134</p>
                <p><i class="fab fa-instagram"></i> IG: @stan_mikir</p>
            </div>
            
            <div class="info-column">
                <h3>Fitur</h3>
                <p>✓ Enak + Hemat</p>
                <p>✓ Frozen - Praktis</p>
                <p>✓ Harga Terjangkau</p>
            </div>
        </div>
    </div>
    
    <div class="footer-bottom">
        <p>&copy; 2023 Nugget Okara. Semua Hak Dilindungi. | Website dibuat dengan ❤️ untuk pecinta nugget</p>
    </div>
</footer>

<style>
    .main-footer {
        margin-top: 80px;
        padding-top: 60px;
        border-top: 2px solid rgba(160, 231, 255, 0.1);
        background: rgba(10, 15, 25, 0.5);
    }
    
    .footer-content {
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
        gap: 40px;
        max-width: 1200px;
        margin: 0 auto;
        padding: 0 20px;
    }
    
    .footer-logo {
        text-align: center;
    }
    
    .footer-penguin {
        font-size: 4rem;
        margin-bottom: 15px;
        animation: footer-penguin 3s infinite alternate;
    }
    
    @keyframes footer-penguin {
        0% { transform: rotate(0deg) scale(1); }
        100% { transform: rotate(10deg) scale(1.1); }
    }
    
    .footer-logo h2 {
        font-size: 2rem;
        color: #a0e7ff;
        margin-bottom: 10px;
    }
    
    .footer-logo p {
        color: #b0c0d0;
        font-size: 1.1rem;
    }
    
    .footer-info {
        display: flex;
        gap: 60px;
        flex-wrap: wrap;
    }
    
    .info-column h3 {
        color: #6bc8ff;
        font-size: 1.5rem;
        margin-bottom: 20px;
    }
    
    .info-column p {
        color: #d0e0f0;
        margin-bottom: 10px;
        display: flex;
        align-items: center;
        gap: 10px;
    }
    
    .info-column i {
        color: #2a9dff;
        width: 20px;
    }
    
    .footer-bottom {
        text-align: center;
        padding: 30px;
        margin-top: 40px;
        border-top: 1px solid rgba(160, 231, 255, 0.05);
        color: #8899aa;
        font-size: 0.9rem;
    }
    
    /* Modal Password Styles */
    .password-modal {
        display: none;
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(0, 0, 0, 0.95);
        z-index: 1000;
        justify-content: center;
        align-items: center;
    }
    
    .password-form {
        background: linear-gradient(135deg, 
            rgba(20, 30, 50, 0.95), 
            rgba(10, 20, 40, 0.98));
        padding: 50px;
        border-radius: 25px;
        text-align: center;
        width: 90%;
        max-width: 500px;
        border: 3px solid rgba(42, 157, 255, 0.4);
        box-shadow: 
            0 25px 50px rgba(0, 0, 0, 0.5),
            0 0 60px rgba(42, 157, 255, 0.3);
        position: relative;
        overflow: hidden;
    }
    
    .password-form::before {
        content: '';
        position: absolute;
        top: -10px;
        left: -10px;
        right: -10px;
        bottom: -10px;
        background: linear-gradient(45deg, 
            #2a9dff, 
            #0066cc, 
            #2a9dff);
        z-index: -1;
        filter: blur(20px);
        opacity: 0.3;
    }
    
    .password-form h3 {
        color: #a0e7ff;
        margin-bottom: 20px;
        font-size: 1.8rem;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 10px;
    }
    
    .password-form p {
        color: #d0e0f0;
        margin-bottom: 30px;
        line-height: 1.6;
    }
    
    .password-input {
        width: 100%;
        padding: 18px;
        margin: 20px 0;
        border-radius: 12px;
        border: 2px solid rgba(42, 157, 255, 0.6);
        background: rgba(10, 15, 25, 0.8);
        color: white;
        font-size: 1.2rem;
        text-align: center;
        transition: all 0.3s;
    }
    
    .password-input:focus {
        outline: none;
        border-color: #2a9dff;
        box-shadow: 0 0 20px rgba(42, 157, 255, 0.4);
    }
    
    .password-submit {
        background: linear-gradient(135deg, #2a9dff, #0066cc);
        color: white;
        border: none;
        padding: 18px 40px;
        border-radius: 12px;
        font-size: 1.2rem;
        font-weight: 600;
        cursor: pointer;
        transition: all 0.3s;
        width: 100%;
        margin-top: 10px;
    }
    
    .password-submit:hover {
        background: linear-gradient(135deg, #6bc8ff, #2a9dff);
        transform: translateY(-3px);
        box-shadow: 0 10px 25px rgba(42, 157, 255, 0.4);
    }
</style>
<script>
    // Inisialisasi variabel
    const nugget1 = document.getElementById('nugget1');
    const nugget2 = document.getElementById('nugget2');
    const passwordModal = document.getElementById('passwordModal');
    const passwordInput = document.getElementById('passwordInput');
    const passwordSubmit = document.getElementById('passwordSubmit');
    
    let currentImageId = null;
    
    // Fungsi untuk membuka modal password
    function openPasswordModal(imageId) {
        currentImageId = imageId;
        passwordModal.style.display = 'flex';
        passwordInput.focus();
    }
    
    // Event listener untuk gambar nugget
    nugget1.addEventListener('click', () => openPasswordModal('img1'));
    nugget2.addEventListener('click', () => openPasswordModal('img2'));
    
    // Event listener untuk submit password
    passwordSubmit.addEventListener('click', handlePasswordSubmit);
    
    // Event listener untuk tombol Enter di input password
    passwordInput.addEventListener('keypress', (e) => {
        if (e.key === 'Enter') {
            handlePasswordSubmit();
        }
    });
    
    // Fungsi untuk menangani submit password
    function handlePasswordSubmit() {
        if (passwordInput.value === 'nugget66') {
            // Membuat input file untuk upload gambar
            const fileInput = document.createElement('input');
            fileInput.type = 'file';
            fileInput.accept = 'image/*';
            fileInput.style.display = 'none';
            
            fileInput.onchange = function(e) {
                const file = e.target.files[0];
                if (file && file.type.startsWith('image/')) {
                    const reader = new FileReader();
                    
                    reader.onload = function(event) {
                        const imgElement = document.getElementById(currentImageId);
                        imgElement.src = event.target.result;
                        imgElement.alt = "Foto Nugget Okara Anda";
                        
                        // Efek konfirmasi upload
                        showUploadConfirmation();
                        
                        // Tutup modal
                        passwordModal.style.display = 'none';
                        passwordInput.value = '';
                    };
                    
                    reader.readAsDataURL(file);
                } else {
                    alert('Mohon pilih file gambar yang valid!');
                }
            };
            
            document.body.appendChild(fileInput);
            fileInput.click();
            document.body.removeChild(fileInput);
        } else {
            // Efek shake jika password salah
            passwordInput.style.borderColor = '#ff4444';
            passwordInput.style.boxShadow = '0 0 15px rgba(255, 68, 68, 0.5)';
            passwordInput.value = '';
            
            setTimeout(() => {
                passwordInput.style.borderColor = 'rgba(42, 157, 255, 0.6)';
                passwordInput.style.boxShadow = 'none';
            }, 1000);
            
            alert('Password salah! Coba lagi dengan password: nugget66');
        }
    }
    
    // Fungsi untuk menampilkan konfirmasi upload
    function showUploadConfirmation() {
        const confirmation = document.createElement('div');
        confirmation.innerHTML = `
            <div style="
                position: fixed;
                top: 20px;
                right: 20px;
                background: rgba(42, 157, 255, 0.9);
                color: white;
                padding: 15px 25px;
                border-radius: 10px;
                z-index: 1001;
                box-shadow: 0 10px 25px rgba(0,0,0,0.3);
                animation: slideIn 0.5s ease-out;
            ">
                <i class="fas fa-check-circle"></i> Foto berhasil diunggah!
            </div>
        `;
        
        document.body.appendChild(confirmation);
        
        setTimeout(() => {
            confirmation.style.animation = 'slideOut 0.5s ease-out';
            setTimeout(() => {
                document.body.removeChild(confirmation);
            }, 500);
        }, 3000);
    }
    
    // Menutup modal jika klik di luar form
    passwordModal.addEventListener('click', (e) => {
        if (e.target === passwordModal) {
            passwordModal.style.display = 'none';
            passwordInput.value = '';
        }
    });
    
    // Animasi saat scroll
    window.addEventListener('scroll', () => {
        const scrolled = window.pageYOffset;
        const parallaxElements = document.querySelectorAll('.image-card, .ingredient-item, .tagline-card, .info-card');
        
        parallaxElements.forEach((element, index) => {
            const speed = 0.05 + (index * 0.01);
            const yPos = -(scrolled * speed);
            element.style.transform = `translateY(${yPos}px)`;
        });
    });
    
    // Inisialisasi animasi saat halaman dimuat
    document.addEventListener('DOMContentLoaded', () => {
        // Animasi masuk untuk semua elemen
        const animatedElements = [
            '.main-title', '.subtitle', 
            '.image-card', '.section-title',
            '.ingredient-item', '.fact-card',
            '.tagline-card', '.price-container',
            '.contact-btn', '.info-card'
        ];
        
        animatedElements.forEach((selector, index) => {
            const elements = document.querySelectorAll(selector);
            elements.forEach((el, elIndex) => {
                el.style.opacity = '0';
                el.style.transform = 'translateY(40px)';
                
                setTimeout(() => {
                    el.style.transition = 'opacity 0.8s, transform 0.8s';
                    el.style.opacity = '1';
                    el.style.transform = 'translateY(0)';
                }, 100 * (index + elIndex));
            });
        });
        
        // Efek hover untuk semua tombol
        const buttons = document.querySelectorAll('.contact-btn, .password-submit');
        buttons.forEach(button => {
            button.addEventListener('mouseenter', function() {
                this.style.transform = 'translateY(-5px) scale(1.02)';
            });
            
            button.addEventListener('mouseleave', function() {
                this.style.transform = 'translateY(0) scale(1)';
            });
        });
        
        // Tambahkan style untuk animasi notifikasi
        const style = document.createElement('style');
        style.textContent = `
            @keyframes slideIn {
                from {
                    transform: translateX(100%);
                    opacity: 0;
                }
                to {
                    transform: translateX(0);
                    opacity: 1;
                }
            }
            
            @keyframes slideOut {
                from {
                    transform: translateX(0);
                    opacity: 1;
                }
                to {
                    transform: translateX(100%);
                    opacity: 0;
                }
            }
        `;
        document.head.appendChild(style);
    });
    
    // Efek hover untuk ingredient items
    document.querySelectorAll('.ingredient-item').forEach(item => {
        item.addEventListener('mouseenter', function() {
            const icon = this.querySelector('.ingredient-icon');
            icon.style.transform = 'scale(1.3) rotate(10deg)';
            icon.style.transition = 'transform 0.3s';
        });
        
        item.addEventListener('mouseleave', function() {
            const icon = this.querySelector('.ingredient-icon');
            icon.style.transform = 'scale(1) rotate(0deg)';
        });
    });
</script>
