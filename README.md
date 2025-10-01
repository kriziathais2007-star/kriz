<!DOCTYPE html>
<!-- saved from url=(0034)http://127.0.0.1:5500/septi30.html -->
<html lang="es"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  
  <title>Día de Hot Wheels 🚗🔥</title>
  <style>
    body {
      margin: 0;
      font-family: "Segoe UI", sans-serif;
      background: url('https://img.freepik.com/free-vector/flat-racing-checkered-flag-background_23-2148973028.jpg?semt=ais_hybrid&w=740&q=80') no-repeat center center fixed;
      background-size: cover;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
    }

    h1 {
      position: absolute;
      top: 20px;
      width: 100%;
      text-align: center;
      font-size: 2.5rem;
      color: #fff;
      text-shadow: 0 0 10px #000;
    }

    .track {
      position: relative;
      width: 100%;
      height: 100%;
    }

    .car {
      position: absolute;
      cursor: pointer;
      animation: floaty 6s ease-in-out infinite;
    }

    .car img {
      width: 180px;
      height: auto;
      transition: transform 0.3s ease;
      filter: drop-shadow(0 4px 15px rgba(0,0,0,0.4));
    }

    .car:hover img {
      transform: scale(1.1) rotate(-5deg);
    }

    @keyframes floaty {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-15px); }
    }

    /* Modal */
    .modal {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(0,0,0,0.7);
      display: none;
      align-items: center;
      justify-content: center;
      z-index: 10;
    }

    .modal-content {
      background: #fff;
      border-radius: 20px;
      padding: 20px;
      text-align: center;
      max-width: 400px;
      box-shadow: 0 4px 25px rgba(0,0,0,0.5);
      animation: pop 0.4s ease;
    }

    @keyframes pop {
      0% { transform: scale(0.7); opacity: 0; }
      100% { transform: scale(1); opacity: 1; }
    }

    .modal-content img {
      width: 150px;
      margin-bottom: 15px;
    }

    .close {
      margin-top: 15px;
      padding: 8px 16px;
      border: none;
      background: #ff6b6b;
      color: white;
      border-radius: 10px;
      cursor: pointer;
      font-weight: bold;
    }
    .close:hover {
      background: #e84118;
    }

    audio {
      display: none;
    }
  </style>
</head>
<body>
  <h1>🚗🔥¡Feliz Día de Hot Wheels!🔥🚗</h1>
  <h2>En este 30 de septiembre solo quiero recordarte <p>lo valiosa que es tu amistad en mi vida</p> </h2>
  <!-- Música de fondo -->
  <audio autoplay="" loop="">
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
    Tu navegador no soporta audio.
  </audio>

  <div class="track">
    <!-- Carritos -->
    <div class="car" style="top:4%; left:2%;" onclick="openModal(0)">
      <img src="https://www.pngmart.com/files/23/Hotwheels-PNG-File.png" alt="Carro 1">
    </div>
    <div class="car" style="top:60%; left:26%;" onclick="openModal(1)">
      <img src="https://www.pngmart.com/files/23/Hotwheels-PNG-Clipart.png" alt="Carro 2">
    </div>
    <div class="car" style="top:25%; left:50%;" onclick="openModal(2)">
      <img src="https://i.pinimg.com/originals/2c/77/b1/2c77b1e46759ca5f0b2add4be3d9ba38.png" alt="Carro 3">
    </div>
    <div class="car" style="top:10%; left:70%;" onclick="openModal(3)">
      <img src="https://png.pngtree.com/png-vector/20241119/ourmid/pngtree-best-hot-wheels-car-sets-png-image_14501400.png" alt="Carro 4">
    </div>
  </div>

  <!-- Modal -->
  <div class="modal" id="carModal" style="display: none;">
    <div class="modal-content">
      <img id="modalImg" src="./Día de Hot Wheels 🚗🔥_files/pngtree-best-hot-wheels-car-sets-png-image_14501400.png" alt="Carro">
      <p id="modalMsg">Gracias por ser el copiloto perfecto en este viaje llamado vida. 🚗💨</p>
      <button class="close" onclick="closeModal()">Cerrar</button>
    </div>
  </div>

  <script>
    const cars = [
      {
        img: "https://www.pngmart.com/files/23/Hotwheels-PNG-File.png",
        msg: "Tu amistad es tan rápida y emocionante como este Hot Wheels. ¡Feliz día!"
      },
      {
        img: "https://www.pngmart.com/files/23/Hotwheels-PNG-Clipart.png",
        msg: "Eres fuerte, único y lleno de estilo. 🚀"
      },
      {
        img: "https://i.pinimg.com/originals/2c/77/b1/2c77b1e46759ca5f0b2add4be3d9ba38.png",
        msg: "Nuestra amistad es como una pista Hot Wheels: llena de giros divertidos. 🔥"
      },
      {
        img: "https://png.pngtree.com/png-vector/20241119/ourmid/pngtree-best-hot-wheels-car-sets-png-image_14501400.png",
        msg: "Gracias por ser el copiloto perfecto en este viaje llamado vida. 🚗💨"
      }
    ];

    function openModal(i) {
      document.getElementById("modalImg").src = cars[i].img;
      document.getElementById("modalMsg").innerText = cars[i].msg;
      document.getElementById("carModal").style.display = "flex";
    }

    function closeModal() {
      document.getElementById("carModal").style.display = "none";
    }
  </script>
<!-- Code injected by live-server -->
<script>
	// <![CDATA[  <-- For SVG support
	if ('WebSocket' in window) {
		(function () {
			function refreshCSS() {
				var sheets = [].slice.call(document.getElementsByTagName("link"));
				var head = document.getElementsByTagName("head")[0];
				for (var i = 0; i < sheets.length; ++i) {
					var elem = sheets[i];
					var parent = elem.parentElement || head;
					parent.removeChild(elem);
					var rel = elem.rel;
					if (elem.href && typeof rel != "string" || rel.length == 0 || rel.toLowerCase() == "stylesheet") {
						var url = elem.href.replace(/(&|\?)_cacheOverride=\d+/, '');
						elem.href = url + (url.indexOf('?') >= 0 ? '&' : '?') + '_cacheOverride=' + (new Date().valueOf());
					}
					parent.appendChild(elem);
				}
			}
			var protocol = window.location.protocol === 'http:' ? 'ws://' : 'wss://';
			var address = protocol + window.location.host + window.location.pathname + '/ws';
			var socket = new WebSocket(address);
			socket.onmessage = function (msg) {
				if (msg.data == 'reload') window.location.reload();
				else if (msg.data == 'refreshcss') refreshCSS();
			};
			if (sessionStorage && !sessionStorage.getItem('IsThisFirstTime_Log_From_LiveServer')) {
				console.log('Live reload enabled.');
				sessionStorage.setItem('IsThisFirstTime_Log_From_LiveServer', true);
			}
		})();
	}
	else {
		console.error('Upgrade your browser. This Browser is NOT supported WebSocket for Live-Reloading.');
	}
	// ]]>
</script>


</body></html>
