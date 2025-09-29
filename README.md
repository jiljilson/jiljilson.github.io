

<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>  Football Dreamer</title>
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: repeating-linear-gradient(
        to bottom,
        #1e7c1e,
        #1e7c1e 50px,
        #2fa42f 50px,
        #2fa42f 100px
      );
      color: #fff;
      scroll-behavior: smooth;
      overflow-x: hidden;
    }
    header {
      text-align: center;
      padding: 50px 20px;
      position: relative;
      z-index: 2;
    }
    header img {
      width: 180px;
      height: 180px;
      border-radius: 50%;
      border: 5px solid #fff;
      box-shadow: 0px 0px 20px rgba(255,255,255,0.7);
    }
    header h1 {
      font-size: 2.8em;
      margin-top: 20px;
      color: #fff;
      text-shadow: 2px 2px 4px #000;
    }
    header p {
      font-size: 1.2em;
      color: #f0f0f0;
    }
    section {
      max-width: 900px;
      margin: 60px auto;
      padding: 20px;
      text-align: center;
      position: relative;
      z-index: 2;
      background: rgba(0, 0, 0, 0.4);
      border-radius: 15px;
      box-shadow: 0px 0px 15px rgba(0,0,0,0.6);
    }
    section h2 {
      font-size: 2em;
      margin-bottom: 20px;
      color: #ffdf00;
      border-bottom: 2px solid #fff;
      display: inline-block;
      padding-bottom: 10px;
      text-shadow: 1px 1px 3px #000;
    }
    section p {
      font-size: 1.1em;
      line-height: 1.8em;
      color: #eee;
    }
    .video-container {
      margin-top: 30px;
      position: relative;
      padding-bottom: 56.25%;
      height: 0;
      overflow: hidden;
      border: 3px solid #fff;
      border-radius: 10px;
    }
    .video-container iframe {
      position: absolute;
      top: 0; left: 0;
      width: 100%; height: 100%;
      border: none;
    }
    footer {
      text-align: center;
      padding: 20px;
      font-size: 0.9em;
      background: rgba(0, 0, 0, 0.8);
      color: #ddd;
      position: relative;
      z-index: 2;
    }

    /* Football animation */
    .football {
      position: fixed;
      top: -100px;
      width: 50px;
      height: 50px;
      background: url('https://upload.wikimedia.org/wikipedia/commons/d/d3/Soccerball.svg') no-repeat center;
      background-size: contain;
      animation: fall linear infinite;
      z-index: 1;
      opacity: 0.85;
    }

    @keyframes fall {
      0% { transform: translateY(-100px) rotate(0deg); }
      100% { transform: translateY(110vh) rotate(360deg); }
    }
  </style>
</head>
<body>
  <header>
    <!-- Replace profile.jpg with your DP file -->
    <img src="WhatsApp Image 2025-09-29 at 21.15.32_a9479d6e.jpg" alt="Jilson Johnson">
    <h1>Jilson Johnson</h1>
    <p>Dreaming Footballer | AI & Data Science Student</p>
  </header>

  <section id="about">
    <h2>About Me</h2>
    <p>
      Hi, I’m <strong>Jilson Johnson</strong> — a footballer in my dreams, 
      and a student of <strong>Artificial Intelligence & Data Science</strong> 
      at Rajagiri School of Engineering and Technology.  
      When I’m not studying or coding, you’ll find me immersed in the world of football, 
      playing <strong>eFootball</strong> (sometimes even sneaking in a little “creative cheating” 
      to keep the game interesting with friends!).
    </p>
  </section>

  <section id="motivation">
    <h2>Football & Motivation</h2>
    <p>
      Football is more than a sport — it’s a philosophy.  
      It teaches us to fight for every goal, to never give up even when the score is against us, 
      and to always believe that the next kick could change everything.  
    </p>
    <p><em>“In football, as in life, the dreamers are the ones who score the impossible goals.”</em></p>
  </section>

  <section id="skills">
    <h2>My Football Gaming Skills</h2>
    <p>
      Here’s a quick glimpse of my virtual football journey.  
      Check out my YouTube video where I showcase my eFootball skills!
    </p>
    <div class="video-container">
      <!-- Replace YT_VIDEO_ID with your YouTube video ID -->
      <video src="Jilson Johnson (amazing skills)2018-19 - Professional Nightfury (720p, h264).mp4 " autoplay controls height="500" > MY AMAZING SKILLS</video>
    </div>
  </section>

  <footer>
    <p>⚽ Made with passion by Jilson Johnson | Keep chasing the dream ⚽</p>
  </footer>

  <script>
    // Generate random falling footballs
    function createFootball() {
      const football = document.createElement("div");
      football.classList.add("football");
      football.style.left = Math.random() * window.innerWidth + "px";
      football.style.animationDuration = (3 + Math.random() * 3) + "s"; // fall speed
      football.style.width = football.style.height = (30 + Math.random() * 40) + "px"; // random size
      document.body.appendChild(football);

      setTimeout(() => {
        football.remove();
      }, 6000);
    }

    setInterval(createFootball, 700); // every 0.7s a football drops
  </script>
</body>
</html>
```
