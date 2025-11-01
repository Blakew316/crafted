<!DOCTYPE html>

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Crafted - Tailored Software Solutions</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

```
    body {
        font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
        color: #1d1d1f;
        line-height: 1.6;
        background: #ffffff;
        overflow-x: hidden;
    }

    /* Navigation */
    nav {
        position: fixed;
        top: 0;
        width: 100%;
        background: rgba(255, 255, 255, 0.85);
        backdrop-filter: saturate(180%) blur(20px);
        z-index: 1000;
        box-shadow: 0 1px 3px rgba(0, 0, 0, 0.05);
    }

    .nav-container {
        max-width: 1400px;
        margin: 0 auto;
        padding: 24px 60px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .logo-container {
        display: flex;
        align-items: center;
        gap: 16px;
    }

    .logo-mini {
        width: 40px;
        height: 40px;
    }

    .logo-text {
        font-size: 22px;
        font-weight: 600;
        letter-spacing: 3px;
        color: #1d1d1f;
    }

    .nav-links {
        display: flex;
        gap: 48px;
        list-style: none;
    }

    .nav-links a {
        text-decoration: none;
        color: #1d1d1f;
        font-size: 15px;
        font-weight: 500;
        transition: all 0.3s;
        position: relative;
    }

    .nav-links a::after {
        content: '';
        position: absolute;
        bottom: -4px;
        left: 0;
        width: 0;
        height: 2px;
        background: #0071e3;
        transition: width 0.3s;
    }

    .nav-links a:hover::after {
        width: 100%;
    }

    /* Hero Section */
    .hero {
        padding: 200px 60px 140px;
        text-align: center;
        background: linear-gradient(180deg, #fafafa 0%, #ffffff 100%);
        position: relative;
        overflow: hidden;
    }

    .hero::before {
        content: '';
        position: absolute;
        top: 0;
        left: 50%;
        transform: translateX(-50%);
        width: 1200px;
        height: 1200px;
        background: radial-gradient(circle, rgba(168, 213, 226, 0.15) 0%, transparent 70%);
        border-radius: 50%;
        z-index: 0;
    }

    .hero-content {
        position: relative;
        z-index: 1;
    }

    .hero-logo {
        width: 140px;
        height: 140px;
        margin: 0 auto 50px;
        filter: drop-shadow(0 20px 40px rgba(0, 0, 0, 0.08));
    }

    .hero h1 {
        font-size: 80px;
        font-weight: 700;
        letter-spacing: 10px;
        margin-bottom: 24px;
        color: #1d1d1f;
        background: linear-gradient(135deg, #1d1d1f 0%, #4a4a4a 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
    }

    .hero-subtitle {
        font-size: 32px;
        font-weight: 400;
        color: #6e6e73;
        margin-bottom: 36px;
        letter-spacing: 2px;
    }

    .hero-description {
        font-size: 24px;
        color: #1d1d1f;
        max-width: 900px;
        margin: 0 auto 60px;
        line-height: 1.6;
        font-weight: 300;
    }

    .cta-primary {
        display: inline-block;
        padding: 18px 56px;
        background: linear-gradient(135deg, #0071e3 0%, #0077ed 100%);
        color: white;
        text-decoration: none;
        border-radius: 50px;
        font-size: 18px;
        font-weight: 600;
        transition: all 0.3s;
        border: none;
        cursor: pointer;
        box-shadow: 0 10px 30px rgba(0, 113, 227, 0.3);
        margin-right: 20px;
    }

    .cta-primary:hover {
        transform: translateY(-3px);
        box-shadow: 0 15px 40px rgba(0, 113, 227, 0.4);
    }

    .cta-secondary {
        display: inline-block;
        padding: 18px 56px;
        background: transparent;
        color: #0071e3;
        text-decoration: none;
        border-radius: 50px;
        font-size: 18px;
        font-weight: 600;
        transition: all 0.3s;
        border: 2px solid #0071e3;
        cursor: pointer;
    }

    .cta-secondary:hover {
        background: rgba(0, 113, 227, 0.05);
        transform: translateY(-3px);
    }

    /* Services Section */
    .services {
        padding: 140px 60px;
        max-width: 1400px;
        margin: 0 auto;
        background: white;
    }

    .section-header {
        text-align: center;
        margin-bottom: 100px;
    }

    .section-label {
        font-size: 16px;
        font-weight: 600;
        color: #0071e3;
        letter-spacing: 2px;
        text-transform: uppercase;
        margin-bottom: 16px;
    }

    .section-title {
        font-size: 56px;
        font-weight: 700;
        color: #1d1d1f;
        margin-bottom: 24px;
        line-height: 1.1;
    }

    .section-description {
        font-size: 21px;
        color: #6e6e73;
        max-width: 700px;
        margin: 0 auto;
        line-height: 1.5;
    }

    .service-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(380px, 1fr));
        gap: 40px;
    }

    .service-card {
        background: linear-gradient(135deg, #fafafa 0%, #ffffff 100%);
        border-radius: 24px;
        padding: 60px 40px;
        text-align: center;
        transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        border: 1px solid rgba(0, 0, 0, 0.06);
        position: relative;
        overflow: hidden;
    }

    .service-card::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        height: 4px;
        background: linear-gradient(90deg, #0071e3, #00c6ff);
        transform: scaleX(0);
        transition: transform 0.4s;
    }

    .service-card:hover {
        transform: translateY(-12px);
        box-shadow: 0 30px 60px rgba(0, 0, 0, 0.12);
        border-color: rgba(0, 113, 227, 0.2);
    }

    .service-card:hover::before {
        transform: scaleX(1);
    }

    .service-icon {
        width: 100px;
        height: 100px;
        margin: 0 auto 32px;
        background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
        border-radius: 24px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 48px;
        transition: all 0.4s;
    }

    .service-card:hover .service-icon {
        transform: scale(1.1) rotate(5deg);
        background: linear-gradient(135deg, #0071e3 0%, #00c6ff 100%);
    }

    .service-card h3 {
        font-size: 32px;
        font-weight: 600;
        margin-bottom: 24px;
        color: #1d1d1f;
    }

    .service-card p {
        font-size: 18px;
        color: #6e6e73;
        line-height: 1.7;
    }

    /* Support Section */
    .support-section {
        background: linear-gradient(135deg, #1e293b 0%, #0f172a 100%);
        padding: 140px 60px;
        text-align: center;
        position: relative;
        overflow: hidden;
    }

    .support-section::before {
        content: '';
        position: absolute;
        top: -50%;
        right: -10%;
        width: 600px;
        height: 600px;
        background: radial-gradient(circle, rgba(168, 213, 226, 0.06) 0%, transparent 70%);
        border-radius: 50%;
    }

    .support-section::after {
        content: '';
        position: absolute;
        bottom: -50%;
        left: -10%;
        width: 600px;
        height: 600px;
        background: radial-gradient(circle, rgba(168, 213, 226, 0.06) 0%, transparent 70%);
        border-radius: 50%;
    }

    .support-content {
        max-width: 900px;
        margin: 0 auto;
        position: relative;
        z-index: 1;
    }

    .support-icon {
        width: 100px;
        height: 100px;
        margin: 0 auto 40px;
        background: rgba(168, 213, 226, 0.08);
        border: 2px solid rgba(168, 213, 226, 0.2);
        border-radius: 24px;
        display: flex;
        align-items: center;
        justify-content: center;
        backdrop-filter: blur(10px);
    }

    .support-icon svg {
        width: 50px;
        height: 50px;
    }

    .support-section h2 {
        font-size: 56px;
        font-weight: 700;
        margin-bottom: 32px;
        color: #ffffff;
    }

    .support-section p {
        font-size: 24px;
        color: rgba(255, 255, 255, 0.9);
        line-height: 1.6;
        margin-bottom: 24px;
    }

    .support-features {
        display: flex;
        justify-content: center;
        gap: 60px;
        margin-top: 60px;
        flex-wrap: wrap;
    }

    .support-feature {
        text-align: center;
        background: rgba(255, 255, 255, 0.05);
        padding: 40px 30px;
        border-radius: 20px;
        border: 1px solid rgba(255, 255, 255, 0.1);
        transition: all 0.3s;
        backdrop-filter: blur(10px);
        min-width: 200px;
    }

    .support-feature:hover {
        transform: translateY(-8px);
        background: rgba(255, 255, 255, 0.08);
        border-color: rgba(168, 213, 226, 0.3);
        cursor: pointer;
    }

    .support-feature a {
        display: block;
    }

    .support-feature-icon {
        width: 70px;
        height: 70px;
        margin: 0 auto 20px;
        background: rgba(168, 213, 226, 0.12);
        border-radius: 16px;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .support-feature-icon svg {
        width: 32px;
        height: 32px;
    }

    .support-feature h4 {
        font-size: 20px;
        color: #ffffff;
        font-weight: 600;
        margin-bottom: 8px;
    }

    .support-feature p {
        font-size: 16px;
        color: rgba(255, 255, 255, 0.8);
    }

    .support-feature p {
        font-size: 16px;
        color: #6e6e73;
    }

    /* Contact Form Section */
    .contact-section {
        padding: 140px 60px;
        background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
        position: relative;
        overflow: hidden;
    }

    .contact-section::before {
        content: '';
        position: absolute;
        top: -30%;
        right: -10%;
        width: 500px;
        height: 500px;
        background: radial-gradient(circle, rgba(0, 113, 227, 0.03) 0%, transparent 70%);
        border-radius: 50%;
    }

    .contact-section::after {
        content: '';
        position: absolute;
        bottom: -30%;
        left: -10%;
        width: 500px;
        height: 500px;
        background: radial-gradient(circle, rgba(168, 213, 226, 0.05) 0%, transparent 70%);
        border-radius: 50%;
    }

    .contact-wrapper {
        max-width: 1000px;
        margin: 0 auto;
        position: relative;
        z-index: 1;
    }

    .contact-section .section-header {
        margin-bottom: 80px;
    }

    .contact-section .section-label {
        color: #0071e3;
    }

    .contact-section .section-title {
        color: #1d1d1f;
    }

    .contact-section .section-description {
        color: #4a4a4a;
    }

    .form-container {
        background: #ffffff;
        border-radius: 32px;
        padding: 80px 60px;
        border: 1px solid rgba(0, 0, 0, 0.08);
        box-shadow: 0 20px 60px rgba(0, 0, 0, 0.08);
    }

    .form-group {
        margin-bottom: 32px;
    }

    .form-group label {
        display: block;
        font-size: 15px;
        font-weight: 600;
        margin-bottom: 12px;
        color: #1d1d1f;
    }

    .form-group input,
    .form-group textarea,
    .form-group select {
        width: 100%;
        padding: 18px 24px;
        font-size: 17px;
        border: 2px solid #e5e5e7;
        border-radius: 14px;
        background: #ffffff;
        font-family: inherit;
        transition: all 0.3s;
        color: #1d1d1f;
    }

    .form-group input::placeholder,
    .form-group textarea::placeholder {
        color: #a1a1a6;
    }

    .form-group select {
        color: #1d1d1f;
        cursor: pointer;
    }

    .form-group select option {
        background: #ffffff;
        color: #1d1d1f;
    }

    .form-group input:focus,
    .form-group textarea:focus,
    .form-group select:focus {
        outline: none;
        border-color: #0071e3;
        box-shadow: 0 0 0 4px rgba(0, 113, 227, 0.1);
        background: #ffffff;
    }

    .form-group textarea {
        min-height: 150px;
        resize: vertical;
    }

    .form-row {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 24px;
    }

    .submit-button {
        width: 100%;
        padding: 20px;
        background: linear-gradient(135deg, #0071e3 0%, #0077ed 100%);
        color: white;
        border: none;
        border-radius: 14px;
        font-size: 18px;
        font-weight: 600;
        cursor: pointer;
        transition: all 0.3s;
        margin-top: 24px;
        box-shadow: 0 10px 30px rgba(0, 113, 227, 0.3);
    }

    .submit-button:hover {
        transform: translateY(-3px);
        box-shadow: 0 15px 40px rgba(0, 113, 227, 0.4);
        background: linear-gradient(135deg, #0077ed 0%, #0084ff 100%);
    }

    /* Footer */
    footer {
        background: #1d1d1f;
        padding: 80px 60px 40px;
        color: #a1a1a6;
    }

    .footer-content {
        max-width: 1400px;
        margin: 0 auto;
        display: grid;
        grid-template-columns: 2fr 1fr 1fr 1fr;
        gap: 60px;
        margin-bottom: 60px;
    }

    .footer-section h4 {
        color: white;
        font-size: 18px;
        font-weight: 600;
        margin-bottom: 20px;
    }

    .footer-section p {
        font-size: 15px;
        line-height: 1.6;
        margin-bottom: 20px;
    }

    .footer-links {
        list-style: none;
    }

    .footer-links li {
        margin-bottom: 12px;
    }

    .footer-links a {
        color: #a1a1a6;
        text-decoration: none;
        font-size: 15px;
        transition: color 0.3s;
    }

    .footer-links a:hover {
        color: white;
    }

    .footer-bottom {
        text-align: center;
        padding-top: 40px;
        border-top: 1px solid rgba(255, 255, 255, 0.1);
        font-size: 14px;
    }

    /* Animations */
    @keyframes fadeInUp {
        from {
            opacity: 0;
            transform: translateY(30px);
        }
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }

    @keyframes fadeInLeft {
        from {
            opacity: 0;
            transform: translateX(-30px);
        }
        to {
            opacity: 1;
            transform: translateX(0);
        }
    }

    @keyframes fadeInRight {
        from {
            opacity: 0;
            transform: translateX(30px);
        }
        to {
            opacity: 1;
            transform: translateX(0);
        }
    }

    @keyframes fadeIn {
        from {
            opacity: 0;
        }
        to {
            opacity: 1;
        }
    }

    /* Scroll animation classes */
    .scroll-animate {
        opacity: 0;
    }

    .scroll-animate.animated {
        animation-duration: 0.8s;
        animation-fill-mode: forwards;
        animation-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
    }

    .fade-in-up {
        animation-name: fadeInUp;
    }

    .fade-in-left {
        animation-name: fadeInLeft;
    }

    .fade-in-right {
        animation-name: fadeInRight;
    }

    .fade-in {
        animation-name: fadeIn;
    }

    /* Stagger animation delays for multiple elements */
    .scroll-animate:nth-child(1) { animation-delay: 0s; }
    .scroll-animate:nth-child(2) { animation-delay: 0.1s; }
    .scroll-animate:nth-child(3) { animation-delay: 0.2s; }
    .scroll-animate:nth-child(4) { animation-delay: 0.3s; }
    .scroll-animate:nth-child(5) { animation-delay: 0.4s; }
    .scroll-animate:nth-child(6) { animation-delay: 0.5s; }

    /* Responsive */
    @media (max-width: 1024px) {
        .hero h1 {
            font-size: 64px;
            letter-spacing: 6px;
        }

        .service-grid {
            grid-template-columns: 1fr;
        }

        .footer-content {
            grid-template-columns: 1fr 1fr;
        }
    }

    @media (max-width: 768px) {
        .nav-container {
            padding: 20px 30px;
        }

        .nav-links {
            display: none;
        }

        .hero {
            padding: 160px 30px 100px;
        }

        .hero h1 {
            font-size: 48px;
            letter-spacing: 4px;
        }

        .hero-subtitle {
            font-size: 24px;
        }

        .hero-description {
            font-size: 18px;
        }

        .section-title {
            font-size: 40px;
        }

        .services,
        .support-section,
        .contact-section {
            padding: 80px 30px;
        }

        .form-row {
            grid-template-columns: 1fr;
        }

        .form-container {
            padding: 40px 30px;
        }

        .service-grid {
            grid-template-columns: 1fr;
        }

        .support-features {
            flex-direction: column;
            gap: 40px;
        }

        .footer-content {
            grid-template-columns: 1fr;
            gap: 40px;
        }

        .cta-primary,
        .cta-secondary {
            display: block;
            margin: 10px 0;
        }
    }
</style>
```

</head>
<body>
    <!-- Navigation -->
    <nav>
        <div class="nav-container">
            <div class="logo-container">
                <svg class="logo-mini" viewBox="0 0 120 120" xmlns="http://www.w3.org/2000/svg">
                    <rect width="120" height="120" fill="none" stroke="#1d1d1f" stroke-width="8" rx="8"/>
                    <rect x="42" y="42" width="36" height="36" fill="#a8d5e2"/>
                </svg>
                <div class="logo-text">CRAFTED</div>
            </div>
            <ul class="nav-links">
                <li><a href="#services">Services</a></li>
                <li><a href="#support">Support</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

```
<!-- Hero Section -->
<section class="hero">
    <div class="hero-content">
        <svg class="hero-logo scroll-animate fade-in" viewBox="0 0 120 120" xmlns="http://www.w3.org/2000/svg">
            <rect width="120" height="120" fill="none" stroke="#1d1d1f" stroke-width="6" rx="8"/>
            <rect x="42" y="42" width="36" height="36" fill="#a8d5e2"/>
        </svg>
        <h1 class="scroll-animate fade-in-up">CRAFTED</h1>
        <p class="hero-subtitle scroll-animate fade-in-up">Tailored Software Solutions</p>
        <p class="hero-description scroll-animate fade-in-up">
            Transform your business with custom applications designed specifically for your needs. 
            We enhance your Point of Sale systems and create stunning websites that drive results.
        </p>
        <div class="scroll-animate fade-in-up">
            <a href="#contact" class="cta-primary">Get Started</a>
            <a href="#services" class="cta-secondary">Learn More</a>
        </div>
    </div>
</section>

<!-- Services Section -->
<section class="services" id="services">
    <div class="section-header scroll-animate fade-in-up">
        <div class="section-label">What We Do</div>
        <h2 class="section-title">Solutions Built For You</h2>
        <p class="section-description">
            We specialize in creating custom technology that fits your business like a glove. 
            From Point of Sale enhancements to beautiful websites, we've got you covered.
        </p>
    </div>
    <div class="service-grid">
        <div class="service-card scroll-animate fade-in-up">
            <div class="service-icon">📱</div>
            <h3>Custom POS Apps</h3>
            <p>
                Make your Point of Sale system work exactly how you need it to. We develop custom applications 
                that integrate seamlessly with your existing setup, adding powerful features and capabilities 
                that transform the way you do business.
            </p>
        </div>
        
        <div class="service-card scroll-animate fade-in-up">
            <div class="service-icon">🌐</div>
            <h3>Website Design & Development</h3>
            <p>
                Whether you're starting from scratch or looking to elevate your existing site, we create 
                beautiful, responsive websites that capture your brand essence and convert visitors into 
                loyal customers.
            </p>
        </div>
        
        <div class="service-card scroll-animate fade-in-up">
            <div class="service-icon">⚙️</div>
            <h3>System Integration</h3>
            <p>
                Unlock the full potential of your current Point of Sale system. We build custom integrations 
                and add-ons that bridge gaps, streamline workflows, and give you the functionality you've 
                always wished you had.
            </p>
        </div>
    </div>
</section>

<!-- Support Section -->
<section class="support-section" id="support">
    <div class="support-content">
        <div class="support-icon scroll-animate fade-in">
            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M12 2C6.48 2 2 6.48 2 12V17C2 18.66 3.34 20 5 20H6V13H4V12C4 7.66 7.58 4 12 4C16.42 4 20 7.66 20 12V13H18V20H19C20.66 20 22 18.66 22 17V12C22 6.48 17.52 2 12 2Z" stroke="rgba(168, 213, 226, 0.9)" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
            </svg>
        </div>
        <h2 class="scroll-animate fade-in-up">24/7 World-Class Support</h2>
        <p class="scroll-animate fade-in-up">
            Your success is our mission. That's why we offer round-the-clock expert support for your 
            Point of Sale system and all our custom solutions.
        </p>
        <p class="scroll-animate fade-in-up">
            Day or night, weekday or weekend—simply text or call us whenever you need help. 
            Our dedicated team is always ready to get you back up and running in no time.
        </p>
        
        <div class="support-features">
            <div class="support-feature scroll-animate fade-in-left">
                <a href="tel:210-480-6345" style="text-decoration: none; color: inherit;">
                    <div class="support-feature-icon">
                        <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M22 16.92V19.92C22 20.4896 21.5523 20.9574 20.9856 20.9974C20.7094 21.0153 20.4346 21.0243 20.16 21.024C10.576 21.024 2.81004 13.258 2.81004 3.67401C2.81004 3.39938 2.81905 3.12463 2.83696 2.84835C2.877 2.28167 3.34474 1.83398 3.91437 1.83398H6.91437C7.47863 1.83398 7.96218 2.27872 8.01862 2.83878C8.11701 3.72783 8.31659 4.5989 8.61201 5.43663C8.76543 5.86542 8.64628 6.34662 8.31004 6.64899L6.61004 8.23599C8.12014 11.6579 10.92 14.4579 14.342 15.968L15.929 14.268C16.2313 13.9318 16.7125 13.8126 17.1413 13.966C17.9791 14.2614 18.8501 14.461 19.7392 14.5594C20.2992 14.6158 20.744 15.0994 20.744 15.6636V18.6636C20.744 19.2159 20.2963 19.6636 19.744 19.6636H19.24" stroke="rgba(168, 213, 226, 0.9)" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                        </svg>
                    </div>
                    <h4>Call Anytime</h4>
                    <p>210-480-6345</p>
                </a>
            </div>
            <div class="support-feature scroll-animate fade-in-up">
                <a href="sms:210-480-6345" style="text-decoration: none; color: inherit;">
                    <div class="support-feature-icon">
                        <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M21 15C21 15.5304 20.7893 16.0391 20.4142 16.4142C20.0391 16.7893 19.5304 17 19 17H7L3 21V5C3 4.46957 3.21071 3.96086 3.58579 3.58579C3.96086 3.21071 4.46957 3 5 3H19C19.5304 3 20.0391 3.21071 20.4142 3.58579C20.7893 3.96086 21 4.46957 21 5V15Z" stroke="rgba(168, 213, 226, 0.9)" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                        </svg>
                    </div>
                    <h4>Text Support</h4>
                    <p>210-480-6345</p>
                </a>
            </div>
            <div class="support-feature scroll-animate fade-in-right">
                <div class="support-feature-icon">
                    <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M13 2L3 14H12L11 22L21 10H12L13 2Z" stroke="rgba(168, 213, 226, 0.9)" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                    </svg>
                </div>
                <h4>Fast Resolution</h4>
                <p>Minimal downtime guaranteed</p>
            </div>
        </div>
    </div>
</section>

<!-- Contact Form Section -->
<section class="contact-section" id="contact">
    <div class="contact-wrapper">
        <div class="section-header scroll-animate fade-in-up">
            <div class="section-label">Get In Touch</div>
            <h2 class="section-title">Let's Build Something Great</h2>
            <p class="section-description">
                Ready to transform your business? Fill out the form below and we'll reach out to discuss 
                how we can help you achieve your goals.
            </p>
        </div>
        
        <div class="form-container scroll-animate fade-in-up">
            <form id="contactForm">
                <div class="form-row">
                    <div class="form-group">
                        <label for="firstName">First Name *</label>
                        <input type="text" id="firstName" name="firstName" required placeholder="John">
                    </div>
                    <div class="form-group">
                        <label for="lastName">Last Name *</label>
                        <input type="text" id="lastName" name="lastName" required placeholder="Smith">
                    </div>
                </div>
                
                <div class="form-row">
                    <div class="form-group">
                        <label for="email">Email Address *</label>
                        <input type="email" id="email" name="email" required placeholder="john@company.com">
                    </div>
                    <div class="form-group">
                        <label for="phone">Phone Number *</label>
                        <input type="tel" id="phone" name="phone" required placeholder="(555) 123-4567">
                    </div>
                </div>
                
                <div class="form-group">
                    <label for="company">Company Name</label>
                    <input type="text" id="company" name="company" placeholder="Your Company">
                </div>
                
                <div class="form-group">
                    <label for="interest">What are you interested in? *</label>
                    <select id="interest" name="interest" required>
                        <option value="">Select an option</option>
                        <option value="pos-apps">Custom POS Applications</option>
                        <option value="website">Website Design & Development</option>
                        <option value="both">Both POS Apps & Website</option>
                        <option value="support">24/7 Support Services</option>
                        <option value="other">Other</option>
                    </select>
                </div>
                
                <div class="form-group">
                    <label for="message">Tell us about your project *</label>
                    <textarea id="message" name="message" required placeholder="Share details about your business needs and how we can help you succeed..."></textarea>
                </div>
                
                <button type="submit" class="submit-button">Request Information</button>
            </form>
        </div>
    </div>
</section>

<!-- Footer -->
<footer>
    <div class="footer-content">
        <div class="footer-section">
            <h4>CRAFTED</h4>
            <p>Tailored Software Solutions for modern businesses. We transform your vision into powerful, custom technology.</p>
        </div>
        <div class="footer-section">
            <h4>Services</h4>
            <ul class="footer-links">
                <li><a href="#services">Custom POS Apps</a></li>
                <li><a href="#services">Website Design</a></li>
                <li><a href="#services">System Integration</a></li>
                <li><a href="#support">24/7 Support</a></li>
            </ul>
        </div>
        <div class="footer-section">
            <h4>Company</h4>
            <ul class="footer-links">
                <li><a href="#services">About Us</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><a href="#services">Our Work</a></li>
                <li><a href="#support">Support</a></li>
            </ul>
        </div>
        <div class="footer-section">
            <h4>Connect</h4>
            <ul class="footer-links">
                <li><a href="tel:">Call Us</a></li>
                <li><a href="sms:">Text Us</a></li>
                <li><a href="mailto:">Email Us</a></li>
            </ul>
        </div>
    </div>
    <div class="footer-bottom">
        <p>&copy; 2024 Crafted. All rights reserved. | Tailored Software Solutions</p>
    </div>
</footer>

<script>
    // Smooth scrolling for navigation links
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function (e) {
            e.preventDefault();
            const target = document.querySelector(this.getAttribute('href'));
            if (target) {
                const navHeight = document.querySelector('nav').offsetHeight;
                const targetPosition = target.offsetTop - navHeight;
                window.scrollTo({
                    top: targetPosition,
                    behavior: 'smooth'
                });
            }
        });
    });

    // Form submission handler
    document.getElementById('contactForm').addEventListener('submit', function(e) {
        e.preventDefault();
        
        // Get form data
        const formData = new FormData(this);
        const data = Object.fromEntries(formData);
        
        // Display success message
        const button = this.querySelector('.submit-button');
        const originalText = button.textContent;
        button.textContent = '✓ Thank you! We\'ll be in touch soon.';
        button.style.background = 'linear-gradient(135deg, #10b981 0%, #059669 100%)';
        
        // Reset after 3 seconds
        setTimeout(() => {
            this.reset();
            button.textContent = originalText;
            button.style.background = '';
        }, 3000);
        
        // In production, send to your server:
        // fetch('/api/contact', {
        //     method: 'POST',
        //     headers: { 'Content-Type': 'application/json' },
        //     body: JSON.stringify(data)
        // });
    });

    // Intersection Observer for animations
    const observerOptions = {
        threshold: 0.1,
        rootMargin: '0px 0px -100px 0px'
    };

    const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                entry.target.classList.add('animated');
                // Optional: unobserve after animation to improve performance
                // observer.unobserve(entry.target);
            }
        });
    }, observerOptions);

    // Observe all elements with scroll-animate class
    document.addEventListener('DOMContentLoaded', function() {
        const animatedElements = document.querySelectorAll('.scroll-animate');
        animatedElements.forEach(element => {
            observer.observe(element);
        });
    });
</script>
```

</body>
</html>
