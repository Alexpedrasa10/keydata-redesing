<template>
  <div class="mt-5" style="background:#F2F2F2">
    <section class="Home">
      <div class="container">
        <h1 class="title"><span style="color:#FFF">Soluciones simples</span> <br> para problemas complejos</h1>
        <h3 class="sub-title">"Los problemas complejos se resuelven con la suma de pequeñas y simples soluciones."</h3>
        <div class="buttons">
          <a class="btn" id="btn-servicios" to="/">Servicios</a>
          <a class="btn m-2" id="btn-contacto" to="/">Contactanos</a>
        </div>
      </div>
    </section>
    <section class="Service">
      <div class="container">
        <b-row>
          <b-col>
            <h2 class="title-service">¿Qué ofrecemos?</h2>
            <p>
              Desde nuestra base operativa en la ciudad de Córdoba, Argentina, ofrecemos nuestras soluciones a todo el mundo, garantizando la disminución de costos operativos y optimizando el manejo de la información, disminuyendo sustancialmente el riesgo de errores.
              Para ello, definimos las estrategias e identificamos los problemas operativos crónicos de nuestros clientes.
              Diseñamos y construimos las soluciones, que luego serán transferidas a la nube para su operación.
            </p>
          </b-col>
          <b-col>
            <img src="../assets/img-home.jpg" alt="" class="img">
          </b-col>
        </b-row>
      </div>
    </section>
    <section class="Service" style="background:#FCFFF5">
      <div class="container">
        <b-row>
          <b-col>
            <img src="../assets/img-home2.jpg" alt="" class="img">
          </b-col>
           <b-col>
            <h2 class="title-service">¿Quienes somos?</h2>
            <p>
              Somos un equipo Argentino, que nos especializamos en ofrecer servicios que resuelven problemas crónicos.
              En la toma de decisiones está la esencia de los negocios. Gerenciar es tomar decisiones, muchas veces bajo presión, con información limitada y mucha incertidumbre. Un aspecto básico es entender y analizar la información, organizar los datos para facilitar su posterior uso y toma de decisiones. Por supuesto, hay muchas otras dimensiones que entran en juego, como el comportamiento de las personas, anticipar estas respuestas, pensar estratégicamente, pero el primer paso es formular bien el problema, estructurarlo, procesar la información.
            </p>
          </b-col>
        </b-row>
      </div>
    </section>
  </div>
</template>


<style>
.Home{
  background: #11998e;
  background: -webkit-linear-gradient(to right, #38ef7d, #11998e);  
  background: linear-gradient(to right, #38ef7d, #11998e);
  padding: 5rem;
  animation-duration: 3s;
  animation-name: slidein;
}

.Service{
  margin-top: 4rem;
  margin-bottom: 4rem;
  padding: 1rem;
}

.title{
  text-transform: uppercase;
  font-weight: 800;
  font-size: 3.5rem;
}

.sub-title{
  text-transform: uppercase;
  font-weight: 400;
}

#btn-servicios{
  background: #044D29;
  color: #FFF;
  font-weight: 650;
  font-size: .85rem;
  cursor: pointer;
  text-transform: uppercase;
  padding: 1rem;
}

#btn-contacto{
  background: none;
  border-color: #044D29;
  cursor: pointer;
  font-weight: 650;
  font-size: .85rem;
  text-transform: uppercase;
  color: #2c3e50;
  padding: 1rem;
}

.title-service{
  text-transform: uppercase;
  font-weight: 800;
  padding: 1rem;
  text-align: center;
}

.img{
  width: 30rem;
  height: 20rem;
}

@keyframes slidein {
  0% {
    opacity: 0;
    left: -50%;
  }

  100% {
    opacity: 100%;
    left: 0%;
  }
}
</style>
