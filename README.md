- 👋 Hi, I’m @Dulantha123
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
- <a href="">deploy<a>
<a href="#" class="button">
            <span class="button__text">
                play
            </span>
            <img src="assets/img/cone.png" alt="" class="button__cone">
            <img src="assets/img/torus.png" alt="" class="button__torus">
            <img src="assets/img/icosahedron.png" alt="" class="button__icosahedron">
            <img src="assets/img/sphere.png" alt="" class="button__sphere">
        </a>
        <style>
        /*=============== GOOGLE FONTS ===============*/
@import url("https://fonts.googleapis.com/css2?family=Montserrat+Alternates:wght@700&display=swap");

/*=============== VARIABLES CSS ===============*/
:root {
  /*========== Colors ==========*/
  --first-color: hsl(217, 75%, 80%);
  --body-color: hsl(211, 100%, 95%);
  
  /*========== Font and typography ==========*/
  --body-font: 'Montserrat Alternates', sans-serif;
  --normal-font-size: 1.25rem;
}

/*=============== BASE ===============*/
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

body {
  height: 100vh;
  display: grid;
  place-items: center;
  background-color: var(--body-color);
  font-family: var(--body-font);
  font-size: var(--normal-font-size);
}

a {
  text-decoration: none;
}

/*=============== MAGIC BUTTON ===============*/
.button {
  position: relative;
  background-color: var(--first-color);
  color: #fff;
  padding: .9rem 2.20rem;
  border-radius: 3rem;
  transition: .4s;
}

.button::after {
  content: '';
  width: 80%;
  height: 40%;
  background: linear-gradient(80deg, 
            hsl(217, 80%, 80%) 10%, 
            hsl(217, 85%, 70%) 48%);
  position: absolute;
  left: 0;
  right: 0;
  bottom: -4px;
  margin: 0 auto;
  border-radius: 3rem;
  filter: blur(12px);
  z-index: -1;
  opacity: 0;
  transition: opacity .4s;
}

.button__text {
  position: relative;
  z-index: 10;
}

.button img {
  position: absolute;
  inset: 0;
  margin: auto;
  pointer-events: none;
  transition: .6s;
  opacity: 0;
}

/* Move 3D geometric elements */
.button__cone {
  width: 18px;
  transform: translate(-25px, -6px) rotate(55deg);
  filter: blur(.5px);
}

.button__torus {
  width: 38px;
  transform: translate(7px, -14px) rotate(80deg);
}

.button__icosahedron {
  width: 36px;
  transform: translate(34px, -4px) rotate(-45deg);
  filter: blur(.9px);
}

.button__sphere {
  width: 30px;
  transform: translate(-5px, 15px) rotate(40deg);
}

/* View shadow gradient */
.button:hover::after {
  opacity: 1;
}

/* Button scale */
.button:hover {
  transform: scale(1.3);
}

/* View 3D geometric elements */
.button:hover img {
  opacity: 1;
}

.button:hover .button__cone {
  transform: translate(-38px, -10px) scale(1.2);
}

.button:hover .button__torus {
  transform: translate(7px, -32px) scale(1.1);
}

.button:hover .button__icosahedron {
  transform: translate(50px, -20px) scale(1.1);
}

.button:hover .button__sphere {
  transform: translate(-14px, 20px) scale(1.1);
}
        </style>
<!---
Dulantha123/Dulantha123 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
