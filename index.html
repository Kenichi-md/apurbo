import makeWASocket, {
  useMultiFileAuthState,
  fetchLatestBaileysVersion
} from "@whiskeysockets/baileys"
import Pino from "pino"
import readline from "readline"

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout
})

async function startBot() {
  const { state, saveCreds } = await useMultiFileAuthState("./auth")
  const { version } = await fetchLatestBaileysVersion()

  const sock = makeWASocket({
    logger: Pino({ level: "silent" }),
    auth: state,
    version,
    printQRInTerminal: false
  })

  if (!state.creds.registered) {
    rl.question("📞 WhatsApp number (+91XXXXXXXXXX): ", async (num) => {
      const code = await sock.requestPairingCode(num.trim())
      console.log("🔐 PAIR CODE:", code)
    })
  }

  sock.ev.on("creds.update", saveCreds)

  sock.ev.on("connection.update", (update) => {
    if (update.connection === "open") {
      console.log("✅ WhatsApp Bot Connected (Pair Code)")
    }
    if (update.connection === "close") {
      startBot()
    }
  })

  sock.ev.on("messages.upsert", async ({ messages }) => {
    const msg = messages[0]
    if (!msg.message || msg.key.fromMe) return

    const text =
      msg.message.conversation ||
      msg.message.extendedTextMessage?.text ||
      ""

    const from = msg.key.remoteJid

    if (/hi|hello/i.test(text)) {
      await sock.sendMessage(from, {
        text: "👋 Hi! Pair-Code WhatsApp Bot Ready 🤖"
      })
    }

    if (/menu/i.test(text)) {
      await sock.sendMessage(from, {
        text: `📜 *MENU*
1️⃣ hi
2️⃣ menu
3️⃣ owner`
      })
    }
  })
}

startBot()    @keyframes shine {
      0% { transform: translateX(-100%) rotate(45deg); }
      100% { transform: translateX(100%) rotate(45deg); }
    }
    
    .box:hover {
      transform: perspective(1000px) rotateY(5deg);
      box-shadow: 
        0 15px 35px rgba(0, 0, 0, 0.4),
        inset 0 1px 0 rgba(255, 255, 255, 0.1),
        0 0 15px rgba(138, 43, 226, 0.3);
    }
    
    .logo {
      margin-bottom: 20px;
      display: flex;
      justify-content: center;
    }
    
    .logo-text {
      font-family: 'Orbitron', sans-serif;
      font-size: 28px;
      font-weight: 700;
      background: linear-gradient(45deg, var(--primary), var(--secondary));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      text-shadow: 0 0 10px rgba(138, 43, 226, 0.5);
      letter-spacing: 2px;
    }
    
    .centered-text {
      text-align: center;
      margin-bottom: 20px;
    }
    
    h3 {
      font-family: 'Orbitron', sans-serif;
      font-size: 18px;
      font-weight: 500;
      color: var(--secondary);
      text-shadow: 0 0 5px rgba(0, 247, 255, 0.7);
      margin-bottom: 5px;
      letter-spacing: 1px;
    }
    
    h6 {
      font-size: 14px;
      font-weight: 400;
      color: rgba(255, 255, 255, 0.7);
      margin-bottom: 25px;
    }
    
    .input-container {
      display: flex;
      background: rgba(0, 0, 0, 0.2);
      border-radius: 12px;
      padding: 4px;
      gap: 4px;
      width: 100%;
      margin-bottom: 20px;
      border: 1px solid var(--glass-border);
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    }
    
    .input-container input {
      border-radius: 8px 0 0 8px;
      background: rgba(0, 0, 0, 0.3);
      width: 100%;
      flex-basis: 75%;
      padding: 15px;
      border: none;
      border-right: 1px solid rgba(138, 43, 226, 0.3);
      color: white;
      font-family: 'Rajdhani', sans-serif;
      font-size: 16px;
      font-weight: 500;
      transition: all 0.3s ease;
    }
    
    .input-container input:focus {
      outline: none;
      background: rgba(0, 0, 0, 0.4);
      box-shadow: 0 0 10px rgba(138, 43, 226, 0.3);
    }
    
    .input-container input::placeholder {
      color: rgba(255, 255, 255, 0.4);
    }
    
    .input-container button {
      flex-basis: 25%;
      padding: 15px;
      background: linear-gradient(135deg, var(--primary) 0%, #6a11cb 100%);
      font-family: 'Orbitron', sans-serif;
      font-weight: 600;
      letter-spacing: 1px;
      text-transform: uppercase;
      color: white;
      border: none;
      border-radius: 0 8px 8px 0;
      transition: all 0.3s ease;
      cursor: pointer;
      position: relative;
      overflow: hidden;
    }
    
    .input-container button::before {
      content: '';
      position: absolute;
      top: 0;
      left: -100%;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
      transition: 0.5s;
    }
    
    .input-container button:hover::before {
      left: 100%;
    }
    
    .input-container button:hover {
      background: linear-gradient(135deg, var(--accent) 0%, #ff2a6d 100%);
      box-shadow: 0 0 15px rgba(255, 42, 109, 0.5);
    }
    
    #waiting-message {
      display: none;
      color: var(--secondary);
      font-family: 'Orbitron', sans-serif;
      margin: 15px 0;
      text-shadow: 0 0 5px rgba(0, 247, 255, 0.7);
    }
    
    #pair {
      min-height: 60px;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-top: 10px;
    }
    
    .code-display {
      font-family: 'Orbitron', sans-serif;
      font-size: 22px;
      background: rgba(0, 0, 0, 0.3);
      padding: 12px 20px;
      border-radius: 8px;
      border: 1px solid var(--glass-border);
      cursor: pointer;
      transition: all 0.3s ease;
      display: flex;
      align-items: center;
      gap: 10px;
    }
    
    .code-display:hover {
      background: rgba(0, 0, 0, 0.4);
      box-shadow: 0 0 15px rgba(138, 43, 226, 0.3);
      transform: translateY(-2px);
    }
    
    .code-text {
      color: white;
      font-weight: 500;
    }
    
    .code-value {
      color: var(--secondary);
      font-weight: 700;
      text-shadow: 0 0 5px rgba(0, 247, 255, 0.7);
    }
    
    .pulse {
      animation: pulse 2s infinite;
    }
    
    @keyframes pulse {
      0% { box-shadow: 0 0 0 0 rgba(0, 247, 255, 0.4); }
      70% { box-shadow: 0 0 0 10px rgba(0, 247, 255, 0); }
      100% { box-shadow: 0 0 0 0 rgba(0, 247, 255, 0); }
    }
    
    @media (max-width: 500px) {
      .input-container {
        flex-direction: column;
      }
      
      .input-container input {
        border-radius: 8px;
        border-right: none;
        border-bottom: 1px solid rgba(138, 43, 226, 0.3);
      }
      
      .input-container button {
        padding: 12px;
        border-radius: 8px;
      }
      
      .box {
        padding: 25px 20px;
      }
    }
    
    /* Effets de particules futuristes */
    .particles {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      overflow: hidden;
      z-index: -1;
    }
    
    .particle {
      position: absolute;
      background: rgba(138, 43, 226, 0.3);
      border-radius: 50%;
      animation: float 15s infinite linear;
    }
    
    @keyframes float {
      0% { transform: translateY(100vh) rotate(0deg); opacity: 0; }
      10% { opacity: 1; }
      90% { opacity: 1; }
      100% { transform: translateY(-100px) rotate(360deg); opacity: 0; }
    }
  </style>
</head>
<body>
  <div class="grid"></div>
  <div class="particles" id="particles"></div>
  
  <div class="container">
    <div class="main">
      <div class="box" id="box">
        <div class="logo">
          <div class="logo-text">KENICHI XMD MINI BOT</div>
        </div>
        
        <div id="text">
          <p>
            <h3 class="centered-text">∞ Link with phone number ∞</h3>
            <h6>🌴 Enter Your Number With Country Code 🌴</h6>
            <div class="input-container">
              <input placeholder="+9183xxxxxxxx" type="tel" id="number" name="number">
              <button id="submit">enter</button>
            </div>
           
            <a id="waiting-message" class="centered-text" style="display: none;">Processing...</a>
            <main id="pair"></main>
          </p>
        </div>
      </div>
    </div>
  </div>
  
  <script src="https://cdnjs.cloudflare.com/ajax/libs/axios/1.0.0-alpha.1/axios.min.js"></script>
  <script>
    let a = document.getElementById("pair");
    let b = document.getElementById("submit");
    let c = document.getElementById("number");
    let box = document.getElementById("box");
    let waitingMessage = document.getElementById("waiting-message");

    // Create background particles
    function createParticles() {
      const particlesContainer = document.getElementById('particles');
      const particleCount = 30;
      
      for (let i = 0; i < particleCount; i++) {
        const particle = document.createElement('div');
        particle.classList.add('particle');
        
        const size = Math.random() * 10 + 2;
        const colors = [
          'rgba(138, 43, 226, 0.3)', 
          'rgba(0, 247, 255, 0.3)', 
          'rgba(255, 42, 109, 0.3)'
        ];
        
        particle.style.width = `${size}px`;
        particle.style.height = `${size}px`;
        particle.style.background = colors[Math.floor(Math.random() * colors.length)];
        particle.style.left = `${Math.random() * 100}%`;
        particle.style.animationDuration = `${Math.random() * 20 + 10}s`;
        particle.style.animationDelay = `${Math.random() * 5}s`;
        
        particlesContainer.appendChild(particle);
      }
    }
    
    createParticles();

    async function Copy() {
      let text = document.getElementById("copy-value").innerText;
      let codeDisplay = document.getElementById("code-display");
      await navigator.clipboard.writeText(text);
      
      codeDisplay.innerHTML = '<i class="fas fa-check" style="color:#00ff00; margin-right:8px;"></i> COPIED!';
      codeDisplay.style.background = 'rgba(0, 255, 0, 0.1)';
      codeDisplay.style.border = '1px solid rgba(0, 255, 0, 0.3)';
      
      setTimeout(() => {
        codeDisplay.innerHTML = `
          <i class="fas fa-copy" style="color:var(--secondary);"></i>
          <span class="code-text">CODE:</span>
          <span class="code-value" id="copy-value">${text}</span>
        `;
        codeDisplay.style.background = 'rgba(0, 0, 0, 0.3)';
        codeDisplay.style.border = '1px solid var(--glass-border)';
      }, 2000);
    }

    b.addEventListener("click", async (e) => {
      e.preventDefault();
      if (!c.value) {
        a.innerHTML = '<div style="color:var(--accent);font-weight:500;background:rgba(255,42,109,0.1);padding:10px;border-radius:8px;border:1px solid rgba(255,42,109,0.3)"><i class="fas fa-exclamation-circle"></i> Enter your WhatsApp number with country code.</div>';
      } else if (c.value.replace(/[^0-9]/g, "").length < 11) {
        a.innerHTML = '<div style="color:var(--accent);font-weight:500;background:rgba(255,42,109,0.1);padding:10px;border-radius:8px;border:1px solid rgba(255,42,109,0.3)"><i class="fas fa-times"></i> Invalid number format</div>';
      } else {
        const bc = c.value.replace(/[^0-9]/g, "");
        let bb = "";
        let bbc = "";
        const cc = bc.split('');
        cc.map(a => {
          bbc += a;
          if (bbc.length == 3) {
            bb += " " + a;
          } else if (bbc.length == 8) {
            bb += " " + a;
          } else {
            bb += a;
          }
        });
        c.type = "text";
        c.value = "+" + bb;
        c.style.color = "white";
        waitingMessage.style.display = "block";
        a.innerHTML = '';
        
        try {
          let { data } = await axios(`/code?number=${bc}`);
          let code = data.code || "Service Unavailable";
          waitingMessage.style.display = "none";
          
          a.innerHTML = `
            <div class="code-display pulse" id="code-display" onclick="Copy()">
              <i class="fas fa-copy" style="color:var(--secondary);"></i>
              <span class="code-text">CODE:</span>
              <span class="code-value" id="copy-value">${code}</span>
            </div>
          `;
        } catch (error) {
          waitingMessage.style.display = "none";
          a.innerHTML = '<div style="color:var(--accent);font-weight:500;background:rgba(255,42,109,0.1);padding:10px;border-radius:8px;border:1px solid rgba(255,42,109,0.3)"><i class="fas fa-exclamation-triangle"></i> Service Unavailable</div>';
        }
      }
    });
  </script>
</body>
</html>  }
  !false && setTimeout(function() {
    if (!pageHidden) {
      window.location = protoUrl;
    }
  }, 2000);
}
else if (protoUrl) {
  setTimeout(function() {
    window.location = protoUrl;
  }, 100);
}

var tme_bg = document.getElementById('tgme_background');
if (tme_bg) {
  TWallpaper.init(tme_bg);
  TWallpaper.animate(true);
  window.onfocus = function(){ TWallpaper.update(); };
}
document.body.classList.remove('no_transition');

function toggleTheme(dark) {
  document.documentElement.classList.toggle('theme_dark', dark);
  window.Telegram && Telegram.setWidgetOptions({dark: dark});
}
if (window.matchMedia) {
  var darkMedia = window.matchMedia('(prefers-color-scheme: dark)');
  toggleTheme(darkMedia.matches);
  darkMedia.addListener(function(e) {
    toggleTheme(e.matches);
  });
}

    
    </script>
  </body>
</html>
<!-- page generated in 5.68ms -->
