<!-- 极点 SVG Logo - 飞鸟聚集主题 -->
<div class="logo-container animate__animated animate__fadeInDown">
  <svg class="pole-logo" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
    <!-- 中心极点 -->
    <circle cx="50" cy="50" r="4" fill="#42b983">
      <animate attributeName="r" values="3;5;3" dur="2s" repeatCount="indefinite" />
    </circle>
    <!-- 环绕飞鸟 -->
    <g class="birds">
      <path class="bird" d="M45,20 L50,25 L55,20 L50,22 Z" fill="#42b983" />
      <path class="bird" d="M80,45 L75,50 L80,55 L78,50 Z" fill="#42b983" />
      <path class="bird" d="M55,80 L50,75 L45,80 L50,78 Z" fill="#42b983" />
      <path class="bird" d="M20,55 L25,50 L20,45 L22,50 Z" fill="#42b983" />
    </g>
    <!-- 辅助线条 -->
    <circle cx="50" cy="50" r="35" fill="none" stroke="#42b983" stroke-width="0.5" stroke-dasharray="2,4" opacity="0.3" />
  </svg>
  <h1 class="animated-title">
    <span class="title-text">极点</span>
    <span class="title-en">(Pole)</span>
  </h1>
</div>

<blockquote class="animate__animated animate__fadeInUp animate__delay-1s">资源的终极汇聚点</blockquote>

<p class="animate__animated animate__fadeIn animate__delay-2s">精选开发者与设计师的最佳工具、资源及灵感，助力每一次高效创作。</p>

<div class="cover-buttons animate__animated animate__zoomIn animate__delay-3s">
  <a href="#/README" class="btn-primary" data-tilt>立即开启</a>
  <a href="https://github.com" target="_blank" class="btn-secondary" data-tilt>GitHub</a>
</div>

<!-- 封面专用样式 -->
<style>
  section.cover {
    background: transparent !important;
  }

  section.cover .cover-main {
    margin: 0 auto;
    position: relative;
    z-index: 10;
  }

  .logo-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 1rem;
  }

  .pole-logo {
    width: 120px;
    height: 120px;
    margin-bottom: 1.5rem;
    filter: drop-shadow(0 0 15px rgba(66, 185, 131, 0.3));
  }

  .bird {
    transform-origin: 50% 50%;
    animation: bird-float 4s ease-in-out infinite;
  }

  .bird:nth-child(2) { animation-delay: -1s; }
  .bird:nth-child(3) { animation-delay: -2s; }
  .bird:nth-child(4) { animation-delay: -3s; }

  @keyframes bird-float {
    0%, 100% { transform: translate(0, 0) rotate(0deg); }
    50% { transform: translate(2px, -5px) rotate(5deg); }
  }

  .birds {
    animation: rotate-birds 20s linear infinite;
    transform-origin: 50% 50%;
  }

  @keyframes rotate-birds {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
  }

  section.cover h1.animated-title {
    font-size: 4rem;
    font-weight: 800;
    margin-bottom: 1rem;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 0.5rem;
    overflow: hidden;
  }

  .title-text {
    background: linear-gradient(135deg, #42b983 0%, #23d5ab 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    animation: titleSlideIn 1s ease-out, gradientShift 4s ease-in-out infinite;
    background-size: 200% 200%;
    position: relative;
  }

  .title-text::after {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255,255,255,0.6), transparent);
    animation: shimmer 3s infinite;
  }

  .title-en {
    color: rgba(66, 185, 131, 0.6);
    font-size: 0.7em;
    font-weight: 600;
    animation: fadeInScale 1s ease-out 0.3s both;
  }

  @keyframes titleSlideIn {
    from {
      transform: translateY(-50px);
      opacity: 0;
    }
    to {
      transform: translateY(0);
      opacity: 1;
    }
  }

  @keyframes gradientShift {
    0%, 100% {
      background-position: 0% 50%;
    }
    50% {
      background-position: 100% 50%;
    }
  }

  @keyframes shimmer {
    0% {
      left: -100%;
    }
    100% {
      left: 100%;
    }
  }

  @keyframes fadeInScale {
    from {
      transform: scale(0.8);
      opacity: 0;
    }
    to {
      transform: scale(1);
      opacity: 1;
    }
  }

  section.cover blockquote {
    font-size: 1.8rem;
    color: #42b983;
    font-weight: 600;
    border: none;
    margin-bottom: 2rem;
  }

  section.cover p {
    max-width: 600px;
    margin: 0 auto 2rem;
    line-height: 1.8;
    color: #444;
    font-size: 1.1rem;
  }

  .cover-buttons {
    display: flex;
    gap: 1.5rem;
    justify-content: center;
    margin-top: 2.5rem;
  }

  .btn-primary, .btn-secondary {
    padding: 1rem 3rem;
    border-radius: 12px;
    font-weight: 600;
    transition: all 0.3s;
    text-decoration: none !important;
    font-size: 1.2rem;
    transform-style: preserve-3d;
  }

  .btn-primary {
    background: #42b983;
    color: white !important;
    box-shadow: 0 10px 20px rgba(66, 185, 131, 0.2);
  }

  .btn-secondary {
    background: rgba(255, 255, 255, 0.4);
    color: #333 !important;
    backdrop-filter: blur(15px);
    border: 1px solid rgba(255,255,255,0.4);
    box-shadow: 0 10px 20px rgba(0,0,0,0.05);
  }
</style>
