<template>
  <q-page class="q-pa-lg">

    <div class="text-center q-mb-xl hero-title-box">
      <div class="text-h3 text-primary text-weight-bold">
        Acerca del SENA
      </div>

      <p class="text-h6 text-grey-9">
        Conoce nuestro SENA y el que desarrolló esta aplicación.
      </p>
    </div>

    <q-img
      src="https://github.com/joymarricardopintoortiz/fotos/blob/main/WhatsApp%20Image%202026-09-14%20at%2012.20.07%20PM.jpeg?raw=true"
      class="hero-banner"
      :ratio="30/9"
      fit="cover"
    />

    <div class="row items-center q-gutter-sm q-mt-lg q-mb-md">
      <q-icon name="info" color="primary" size="28px" />
      <div class="text-h5 text-primary">
        Información del centro
      </div>
    </div>

    <q-card bordered class="shadow-2 q-mb-lg">
      <q-card-section>

        <p class="text-body1">
          El Centro Agroturistico del SENA, ubicado en San Gil, Santander,
          es una sede enfocada en la formacion tecnica y tecnologica en
          areas agropecuarias y turisticas. Contamos con espacios diseñados
          para que los aprendices desarrollen competencias practicas en un
          entorno rural real, combinando el aprendizaje academico con
          proyectos productivos que fortalecen la region.
        </p>

        <p class="text-body1 q-mt-md">
          Nuestro centro cuenta con diferentes servicios destinados a
          apoyar el bienestar, la salud, el aprendizaje y el desarrollo
          integral de toda la comunidad educativa. Esta aplicación fue
          diseñada para facilitar el acceso a la informacion de cada
          servicio, permitiendo a los aprendices, instructores y
          visitantes conocer de forma rapida y clara lo que ofrece
          cada area del centro.
        </p>

        <p class="text-body1 q-mt-md">
          Desde esta plataforma los usuarios pueden consultar horarios
          de atencion, informacion de contacto, ubicacion y descripcion
          de cada servicio, asi como conocer a los encargados responsables
          de brindar atencion en enfermeria, bienestar, biblioteca,
          cafeteria y coordinacion academica.
        </p>

      </q-card-section>
    </q-card>

    <div class="row items-center q-gutter-sm q-mb-md">
      <q-icon name="groups" color="primary" size="28px" />
      <div class="text-h5 text-primary">
        Equipo desarrollador
      </div>
    </div>

    <div class="row q-col-gutter-lg">
      <div class="col-12 col-md-4">
        <q-card bordered class="shadow-2">
          <q-card-section class="text-center">

            <q-avatar id="icono_perfil" square>
              <img src="https://github.com/joymarricardopintoortiz/fotos/blob/main/WhatsApp%20Image%202026-09-07%20at%2012.49.14%20PM.jpeg?raw=true">
            </q-avatar>

            <div class="text-h6 q-mt-md">
              Joymar Ricardo
            </div>

            <div class="text-subtitle1 text-primary">
              Desarrollador y Diseñador
            </div>

          </q-card-section>
        </q-card>
      </div>
    </div>
  </q-page>
</template>

<style scoped>
.hero-banner {
    margin: -24px -24px 0 -24px;
    width: calc(100% + 48px);
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.35);
}

.hero-title-box {
  background: rgba(255, 255, 255, 0.92);
  border-radius: 16px;
  padding: 24px 32px;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.15);
}
</style>