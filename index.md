<!DOCTYPE html>
<html lang="en-US"><head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">

<!-- Begin Jekyll SEO tag v2.8.0 -->
<title>Student Blog | CompSci HEHEHEHEHEHEHE</title>
<meta name="generator" content="Jekyll v3.9.3" />
<meta property="og:title" content="Student Blog" />
<meta property="og:locale" content="en_US" />
<meta name="description" content="August 2023 to June 2024" />
<meta property="og:description" content="August 2023 to June 2024" />
<link rel="canonical" href="http://0.0.0.0:4200/CSPBlog/" />
<meta property="og:url" content="http://0.0.0.0:4200/CSPBlog/" />
<meta property="og:site_name" content="CompSci Blogs" />
<meta property="og:type" content="website" />
<meta name="twitter:card" content="summary" />
<meta property="twitter:title" content="Student Blog" />
<script type="application/ld+json">
{"@context":"https://schema.org","@type":"WebSite","description":"August 2023 to June 2024","headline":"Student Blog","name":"CompSci Blogs","url":"http://0.0.0.0:4200/CSPBlog/"}</script>
<!-- End Jekyll SEO tag -->

  <link rel="stylesheet" href="/CSPBlog/assets/css/style.css?v=e858f5ae7d6f0cd2eb2f5306de04b620a0886a94">
  <script src="https://code.jquery.com/jquery-1.12.4.min.js" integrity="sha256-ZosEbRLbNQzLpnKIkEdrPv7lOy9C27hHQ+Xp8a4MxAQ=" crossorigin="anonymous"></script>

    
  <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no">
  <!-- start custom head snippets, customize with your own _includes/head-custom.html file -->

<!-- Setup theme-color -->
<!-- start theme color meta headers -->
<meta name="theme-color" content="#151515">
<meta name="msapplication-navbutton-color" content="#151515">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
<!-- end theme color meta headers -->


<!-- Setup Google Analytics -->



<!-- You can set your favicon here -->
<!-- link rel="shortcut icon" type="image/x-icon" href="/CSPBlog/favicon.ico" -->

<!-- end custom head snippets -->

</head><body>

  <div class="wrapper">
    <header><header class="site-header">

  <div id="header">
    <nav>
      <ul>
        <li class="fork"><a href="/CSPBlog/">Home</a></li>
        <li class="fork"><a href="/CSPBlog/csse">CSSE</a></li>
        <li class="fork"><a href="/CSPBlog/csp">CSP</a></li>
        <li class="fork"><a href="/CSPBlog/csa">CSA</a></li>
        <li class="fork"><a href="/CSPBlog/blogs">Blogs</a></li>
        <li class="title"><a href="https://github.com/Gurbop/CSPBlog#readme">View On GitHub</a></li>
      </ul>
    </nav>
  </div><!-- end header -->
</header></header>


    <section>
      <h2 id="gurshawns-page">Gurshawn’s Page</h2>
<p><img src="/CSPBlog/images/CSPAboutME.png" alt="AboutMe" /></p>
<h2 id="overview-of-hacks-study-and-tangibles">Overview of Hacks, Study and Tangibles</h2>
<p>1. make sure everything is working after each step.
   2. make sure all progmrams are updated
   3. get help from others who have encountered similair problems
   4. You have to use your github url to be able to commit. If you just clone the teacher sample you can only make changes onto  a local host. 
</p>
<p>
  Errors:
  Commit didn't work: To fix this I had to create an ssh key to push changes through the terminal.
  Image didn't work: When entering the picture, I learned I have to use the full file path, so the computer knows where to pull from. 
</p>
<p>While I was setting up my enviornment for class I encountered many problems. Often times when I didn’t understand a command or where to locate a file or folder, I was able to rely on my teammates to explain it to me.</p>

<ul>
  <li>Plans, Lists, <a href="https://clickup.com/blog/scrum-board/">Scrum Boards</a> help you to track key events, show progress and record time.  Effort is a big part of your class grade.  Show plans and time spent!</li>
  <li><a href="https://levelup.gitconnected.com/six-ultimate-daily-hacks-for-every-programmer-60f5f10feae">Hacks(Todo)</a> enable you to stay in focus with key requirements of the class.  Each Hack will produce Tangibles.</li>
  <li>Tangibles or <a href="https://en.wikipedia.org/wiki/Artifact_(software_development)">Tangible Artifacts</a> are things you accumulate as a learner and coder.</li>
</ul>

    </section>

  </div>asf
  <div id="calculator">
    <div style="max-width: 200px; background-color: #3b6fd1; padding: 10px;">
      <input type="text" id="display" disabled>
      <br />
      <button onclick="appendToDisplay('1')">1</button>
      <button onclick="appendToDisplay('2')">2</button>
      <button onclick="appendToDisplay('3')">3</button>
      <button onclick="appendToDisplay('*')">x</button>
      <button onclick="appendToDisplay('+')">+</button>
      <button onclick="appendToDisplay('-')">-</button>
      <br />
      <button onclick="appendToDisplay('4')">4</button>
      <button onclick="appendToDisplay('5')">5</button>
      <button onclick="appendToDisplay('6')">6</button>
      <button onclick="calculate()">=</button>
      <button onclick="appendToDisplay('/')">/</button>
      <button onclick="clearDisplay()">C</button>
      <br />
      <button onclick="appendToDisplay('7')">7</button>
      <button onclick="appendToDisplay('8')">8</button>
      <button onclick="appendToDisplay('9')">9</button>
      <br />
      <button onclick="appendToDisplay('0')">0</button>
    
    </div>
    
    <script>
      let display = document.getElementById('display');
    
      function appendToDisplay(value) {
        display.value += value;
      }
    
      function calculate() {
        try {
          display.value = eval(display.value);
        } catch (error) {
          display.value = 'Error';
        }
      }
    
      function clearDisplay() {
        display.value = '';
      }
    </script>
    
    <head>
      <br />
      <h1 span style="color: yellow; font-size: 20px;">Tic Tac Toe </h1>
      <style>
        .board {
          display: grid;
          grid-template-columns: repeat(3, 100px);
          grid-gap: 2px;
        }
        .cell {
          width: 100px;
          height: 100px;
          border: 1px solid green;
          display: flex;
          align-items: center;
          justify-content: center;
          font-size: 24px;
          cursor: pointer;
        }
      </style>
    </head>
    <body>
      <div class="board" id="board">
        <div class="cell"></div>
        <div class="cell"></div>
        <div class="cell"></div>
        <div class="cell"></div>
        <div class="cell"></div>
        <div class="cell"></div>
        <div class="cell"></div>
        <div class="cell"></div>
        <div class="cell"></div>
      </div>
    
      <script>
        const board = document.getElementById('board');
        const cells = document.querySelectorAll('.cell');
        let currentPlayer = 'X';
        let gameActive = true;
    
        cells.forEach(cell => {
          cell.addEventListener('click', handleCellClick);
        });
    
        function handleCellClick(event) {
          const clickedCell = event.target;
          const clickedIndex = Array.from(cells).indexOf(clickedCell);
    
          if (gameActive && !cells[clickedIndex].textContent) {
            cells[clickedIndex].textContent = currentPlayer;
            checkWin();
            currentPlayer = currentPlayer === 'X' ? 'O' : 'X';
          }
        }
    
        function checkWin() {
          const winCombinations = [
            [0, 1, 2], [3, 4, 5], [6, 7, 8], 
            [0, 3, 6], [1, 4, 7], [2, 5, 8],
            [0, 4, 8], [2, 4, 6]           
          ];
    
          for (const combination of winCombinations) {
            const [a, b, c] = combination;
            if (cells[a].textContent && cells[a].textContent === cells[b].textContent && cells[a].textContent === cells[c].textContent) {
              gameActive = false;
              alert(`${cells[a].textContent} wins!`);
              break;
            }
          }
        }
      </script>
    </body>
</body>


</html>