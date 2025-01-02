<div class="sky">
	<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 1000" preserveAspectRatio="none">
		<!-- Small clouds -->
		<path
			class="cloud cloud-small cloud-1"
			d="M120,100 Q140,85 160,95 Q180,80 200,90 Q220,85 240,90 L240,110 L120,110 Z"
			transform="translate(50, 100) scale(0.5)"
		/>
		<path
			class="cloud cloud-small cloud-2"
			d="M120,100 Q135,88 150,98 Q165,78 180,88 Q195,83 210,88 L210,108 L120,108 Z"
			transform="translate(250, 200) scale(0.5)"
		/>
		<path
			class="cloud cloud-small cloud-3"
			d="M120,100 Q135,88 150,98 Q165,78 180,88 Q195,83 210,88 L210,108 L120,108 Z"
			transform="translate(450, 150) scale(0.5)"
		/>
		<path
			class="cloud cloud-small cloud-9"
			d="M120,100 Q140,85 160,95 Q180,80 200,90 Q220,85 240,90 L240,110 L120,110 Z"
			transform="translate(150, 50) scale(0.4)"
		/>
		<path
			class="cloud cloud-small cloud-10"
			d="M120,100 Q135,88 150,98 Q165,78 180,88 Q195,83 210,88 L210,108 L120,108 Z"
			transform="translate(350, 120) scale(0.45)"
		/>
		<path
			class="cloud cloud-small cloud-11"
			d="M120,100 Q135,88 150,98 Q165,78 180,88 Q195,83 210,88 L210,108 L120,108 Z"
			transform="translate(550, 180) scale(0.35)"
		/>
		<path
			class="cloud cloud-small cloud-12"
			d="M120,100 Q140,85 160,95 Q180,80 200,90 Q220,85 240,90 L240,110 L120,110 Z"
			transform="translate(750, 90) scale(0.5)"
		/>

		<!-- Medium clouds -->
		<path
			class="cloud cloud-medium cloud-4"
			d="M120,100 Q155,85 190,95 Q215,80 240,90 Q265,85 290,90 L290,115 L120,115 Z"
			transform="translate(150, 300) scale(0.8)"
		/>
		<path
			class="cloud cloud-medium cloud-5"
			d="M120,100 Q145,88 170,98 Q195,78 220,88 Q245,83 270,88 L270,112 L120,112 Z"
			transform="translate(350, 250) scale(0.8)"
		/>
		<path
			class="cloud cloud-medium cloud-6"
			d="M120,100 Q150,87 180,97 Q205,77 230,87 Q255,82 280,87 L280,113 L120,113 Z"
			transform="translate(650, 180) scale(0.8)"
		/>
		<path
			class="cloud cloud-medium cloud-13"
			d="M120,100 Q155,85 190,95 Q215,80 240,90 Q265,85 290,90 L290,115 L120,115 Z"
			transform="translate(250, 400) scale(0.7)"
		/>
		<path
			class="cloud cloud-medium cloud-14"
			d="M120,100 Q145,88 170,98 Q195,78 220,88 Q245,83 270,88 L270,112 L120,112 Z"
			transform="translate(450, 350) scale(0.75)"
		/>
		<path
			class="cloud cloud-medium cloud-15"
			d="M120,100 Q150,87 180,97 Q205,77 230,87 Q255,82 280,87 L280,113 L120,113 Z"
			transform="translate(700, 280) scale(0.85)"
		/>

		<!-- Large clouds -->
		<path
			class="cloud cloud-large cloud-7"
			d="M120,100 Q160,80 200,100 Q220,70 260,85 Q290,70 320,85 Q350,70 380,85 L380,130 L120,130 Z"
			transform="translate(550, 80) scale(1.2)"
		/>
		<path
			class="cloud cloud-large cloud-8"
			d="M120,100 Q170,80 220,100 Q250,65 300,85 Q330,65 360,85 Q390,70 420,85 L420,135 L120,135 Z"
			transform="translate(750, 220) scale(1.2)"
		/>
		<path
			class="cloud cloud-large cloud-16"
			d="M120,100 Q160,80 200,100 Q220,70 260,85 Q290,70 320,85 Q350,70 380,85 L380,130 L120,130 Z"
			transform="translate(50, 450) scale(1.1)"
		/>
		<path
			class="cloud cloud-large cloud-17"
			d="M120,100 Q170,80 220,100 Q250,65 300,85 Q330,65 360,85 Q390,70 420,85 L420,135 L120,135 Z"
			transform="translate(400, 500) scale(1.3)"
		/>
		<path
			class="cloud cloud-large cloud-18"
			d="M120,100 Q160,80 200,100 Q220,70 260,85 Q290,70 320,85 Q350,70 380,85 L380,130 L120,130 Z"
			transform="translate(800, 400) scale(1.15)"
		/>
	</svg>
</div>

<style>
.sky {
  width: 100%;
  height: 100vh;
  background: linear-gradient(to bottom, #87CEEB 0%, #b4e2fa 100%);
  position: fixed;
  top: 0;
  left: 0;
  z-index: -1;
  overflow: hidden;
}
.cloud {
  fill: white;
  filter: drop-shadow(3px 5px 2px rgba(0, 0, 0, 0.1));
}
.cloud-small {
  opacity: 0.7;
}
.cloud-medium {
  opacity: 0.8;
}
.cloud-large {
  opacity: 0.9;
}
@keyframes float {
  0%, 100% {
    transform: translate(var(--tx), var(--ty)) scale(var(--scale));
  }
  50% {
    transform: translate(var(--tx), calc(var(--ty) - 15px)) scale(var(--scale));
  }
}
/* Original clouds */
.cloud-1 { --tx: 50px; --ty: 100px; --scale: 0.5; animation: float 8s ease-in-out infinite; }
.cloud-2 { --tx: 250px; --ty: 200px; --scale: 0.5; animation: float 7s ease-in-out infinite; }
.cloud-3 { --tx: 450px; --ty: 150px; --scale: 0.5; animation: float 9s ease-in-out infinite; }
.cloud-4 { --tx: 150px; --ty: 300px; --scale: 0.8; animation: float 10s ease-in-out infinite; }
.cloud-5 { --tx: 350px; --ty: 250px; --scale: 0.8; animation: float 8.5s ease-in-out infinite; }
.cloud-6 { --tx: 650px; --ty: 180px; --scale: 0.8; animation: float 7.5s ease-in-out infinite; }
.cloud-7 { --tx: 550px; --ty: 80px; --scale: 1.2; animation: float 11s ease-in-out infinite; }
.cloud-8 { --tx: 750px; --ty: 220px; --scale: 1.2; animation: float 9.5s ease-in-out infinite; }

/* New clouds */
.cloud-9 { --tx: 150px; --ty: 50px; --scale: 0.4; animation: float 7.2s ease-in-out infinite; }
.cloud-10 { --tx: 350px; --ty: 120px; --scale: 0.45; animation: float 8.7s ease-in-out infinite; }
.cloud-11 { --tx: 550px; --ty: 180px; --scale: 0.35; animation: float 6.8s ease-in-out infinite; }
.cloud-12 { --tx: 750px; --ty: 90px; --scale: 0.5; animation: float 9.3s ease-in-out infinite; }
.cloud-13 { --tx: 250px; --ty: 400px; --scale: 0.7; animation: float 10.5s ease-in-out infinite; }
.cloud-14 { --tx: 450px; --ty: 350px; --scale: 0.75; animation: float 8.2s ease-in-out infinite; }
.cloud-15 { --tx: 700px; --ty: 280px; --scale: 0.85; animation: float 9.8s ease-in-out infinite; }
.cloud-16 { --tx: 50px; --ty: 450px; --scale: 1.1; animation: float 11.5s ease-in-out infinite; }
.cloud-17 { --tx: 400px; --ty: 500px; --scale: 1.3; animation: float 10.8s ease-in-out infinite; }
.cloud-18 { --tx: 800px; --ty: 400px; --scale: 1.15; animation: float 9.7s ease-in-out infinite; }
</style>
