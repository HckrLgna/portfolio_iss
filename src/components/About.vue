<template>
  <div class="bg-green-50 page-section pt-5 -mb-5">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 py-3 wow zoomIn">
          <div class="img-place text-center hidden lg:flex">
            <lottie-player
              src="https://assets2.lottiefiles.com/packages/lf20_qhrndegx.json"
              background="transparent"
              speed="1"
              style="max-width: 500px; max-height: 500px"
              autoplay></lottie-player>
          </div>
        </div>

        <div class="col-lg-6 p-4">
          <h2 class="title-section text-2xl">
            Todo acerca
            <span class="marked">De nosotros</span>
          </h2>
          <div class="divider"></div>

          <div>
            <p>
              Somos un grupo de desarrolladores apasionados 
              por la innovacion trabajamos con tecnologias 
              a la vanguardia creando soluciones a la talla
              de cualquier necesidad, llevamos mas de un año
              trabajando con soluciones que conllevan inteligencia
              artificial.
            </p>
          </div>

          <div>
            <p>
              I'm a well organized person, problem solver, independent employee
              with high attention to detail. Fan of Football and Boxing, outdoor
              activities with my friends, TV series and English literature.
              Actually, I have been living in South Korea for 5 years, I So i'm
              also good in Korean.
            </p>
          </div>

          <div>
            <p class="hidden lg:flex">
              And I'm interested in the entire creative frontend spectrum and
              working on ambitious projects with positive people.
            </p>
          </div>

          <div class="img-place mb-3"></div>
          <a href="#" class="btn btn-primary">More Details</a>
          <a href="#" class="btn btn-outline border ml-2">Success Stories</a>
        </div>
      </div>
    </div>
    <!-- .container -->
  </div>
  <!-- .page-section -->

  <div class="bg-green-50 page-section">
    <div class="container mt-5 w-50">
      <h2 class="title-section text-2xl">
            Contactanos a traves de este 
            <span class="marked">formulario</span>
          </h2>
          <div class="divider"></div>

          <form :action="formAction" method="POST" >
            <div class="mb-3">
              <label for="name" class="form-label">Nombre:</label>
              <input v-model="formData.name" type="text" class="form-control" id="name" name="name" required>
            </div>
            <div class="mb-3">
              <label for="email" class="form-label">Correo Electrónico:</label>
              <input v-model="formData.email" type="email" class="form-control" id="email" name="email" required>
            </div>
            <div class="mb-3">
              <label for="message" class="form-label">Mensaje:</label>
              <textarea v-model="formData.message" class="form-control" id="message" rows="4" name="comments" required></textarea>
            </div>
            <button type="submit" class="btn bg-success">Enviar Mensaje</button>
            <input type="hidden" name="_next" value="http://localhost:8080">
            <input type="hidden" name="_captcha" value="false">
          </form>
    </div>
    <!-- .container -->
  </div> 
  
</template>

<script>

export default {
  data() {
    return {
      scrollPosition: 0,
      formData: {
        name: "",
        email: "",
        message: "",
      },
      formAction: 'https://formsubmit.co/e8d618d0a818dfb00b77846d97b231bc',
    };
  },

  methods: {
    submitForm() {
      // Aquí puedes manejar la lógica de envío del formulario
      console.log('Formulario enviado:', this.formData);
      try {
      } catch (error) {
        console.error(error)
      }
    },
    handleScroll(e) {
      this.scrollPosition = e.target.scrollTop;

      if (this.scrollPosition > 100) {
        console.log("UP");
      } else {
        console.log("DOWN");
      }
    },
  },
};
</script>
