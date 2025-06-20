<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Rx - Video Editor</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Orbitron:wght@700&family=Raleway:wght@400;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
      color: white;
      font-family: 'Montserrat', sans-serif;
      line-height: 1.6;
    }

    .marquee {
      width: 100%;
      overflow: hidden;
      white-space: nowrap;
      box-sizing: border-box;
      padding: 10px 0;
      background: rgba(255, 255, 255, 0.1);
    }

    .marquee span {
      display: inline-block;
      padding-left: 100%;
      animation: marquee 10s linear infinite;
      font-family: 'Orbitron', sans-serif;
      font-size: 1.5rem;
      color: #00fff7;
    }

    @keyframes marquee {
      0%   { transform: translate(0, 0); }
      100% { transform: translate(-100%, 0); }
    }

    header {
      text-align: center;
      padding: 60px 20px;
    }

    header h1 {
      font-family: 'Orbitron', sans-serif;
      font-size: 3rem;
      color: #00fff7;
    }

    header p {
      font-size: 1.2rem;
      color: #ccc;
    }

    section {
      padding: 40px 20px;
      max-width: 1000px;
      margin: auto;
    }

    h2 {
      text-align: center;
      font-family: 'Raleway', sans-serif;
      font-size: 2rem;
      background: linear-gradient(90deg, #FFD700, #FF8C00);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      margin-bottom: 30px;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .gallery video {
      width: 100%;
      border-radius: 12px;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .gallery video:hover {
      transform: scale(1.05);
      box-shadow: 0 0 20px #00fff7;
    }

    .about {
      background-color: rgba(255, 255, 255, 0.05);
      border-radius: 20px;
      padding: 30px;
      backdrop-filter: blur(6px);
      margin-top: 40px;
    }

    footer {
      text-align: center;
      padding: 15px;
      font-size: 12px;
      color: #D3D3D3;
    }
  </style>
</head>
<body>

  <div class="marquee">
    <span>Welcome to Rx Portfolio — Premium Video & Edit Showcase!</span>
  </div>

  <header>
    <h1>Rx</h1>
    <p>I create premium YouTube reels, shorts, and cinematic edits that grab attention of audience.</p>
  </header>

  <section>
    <h2>My Work</h2>
    <div class="gallery">
      <video controls>
        <source src="videos/video1.mp4" type="video/mp4">
      </video>
      <video controls>
        <source src="videos/video2.mp4" type="video/mp4">
      </video>
      <video controls>
        <source src="videos/video3.mp4" type="video/mp4">
      </video>
      <video controls>
        <source src="videos/video4.mp4" type="video/mp4">
      </video>
    </div>
  </section>

  <section class="about">
    <h2>About Me</h2>
    <p>
      I'm Rx, a passionate video editor who transforms ordinary visuals into scroll-stopping content. I specialize in edits for tech, gaming, motivational, and cinematic content. Tools I use: CapCut, Photopea, Picsart, and other mobile apps.
    </p>
  </section>

  <footer>
    Created by <strong>RSG™</strong> - Rahul Kushwaha
  </footer>

</body>
</html>
