<template>
  <q-page class="q-pa-md">

    <q-img
      src="https://github.com/joymarricardopintoortiz/fotos/blob/main/WhatsApp%20Image%202026-09-04%20at%204.47.17%20PM.jpeg?raw=true"
      class="banner"
      :ratio="30/9"
      fit="cover"
    />

    <div class="q-mt-lg">
      <div class="text-h3 text-primary text-weight-bold">
        Biblioteca
      </div>

      <p class="text-body1 q-mt-md">
        La Biblioteca del Centro Agroturístico del SENA ofrece servicios de
        consulta, préstamo de libros y acceso a recursos digitales para la comunidad académica.
        Cuenta con una colección especializada en áreas agropecuarias, turismo, gestión y tecnología,
        así como espacios silenciosos para el estudio individual y la investigación. Dispone de
        equipos informáticos y conexión a internet para la búsqueda en bases de datos institucionales.
        Asimismo, brinda orientación e inducción en el manejo de catálogos en línea y repositorios.
        El espacio está acondicionado con puestos de lectura cómodos e iluminados para el desarrollo
        de actividades formativas. Se promueven talleres de competencia informacional y promoción
        de la lectura. Su propósito principal es respaldar los procesos de aprendizaje e innovación,
        proporcionando información actualizada y un entorno propicio para la gestión del conocimiento
      </p>
    </div>

    <div class="row q-col-gutter-lg q-mt-lg">
      <div class="col-12 col-md-6">
        <q-card bordered class="shadow-2">
          <q-card-section>
            <div class="text-h5 text-primary">
              Encargado de atención
            </div>
          </q-card-section>

          <q-card-section class="row items-center q-gutter-md">
            <q-avatar id="icono_perfil" square>
              <img src="https://github.com/joymarricardopintoortiz/CENTROAGROTURISTICO/blob/main/WhatsApp%20Image%202026-09-11%20at%204.17.48%20PM%20(1).jpeg?raw=true">
            </q-avatar>

            <div class="col">
              <div class="text-h6">
                Yudith Milagros Martínez Bautista
              </div>

              <div class="text-subtitle1">
                Bibliotecaria
              </div>

              <div class="q-mt-sm">
                ✉ ymmartinez@sena.edu.co
              </div>
            </div>
          </q-card-section>

          <q-card-section>
            <q-card bordered flat>
              <q-item>
                <q-item-section avatar>
                  <q-icon name="phone" color="primary" size="md" />
                </q-item-section>

                <q-item-section>
                  <q-item-label caption>
                    Teléfono
                  </q-item-label>
                  <q-item-label class="text-h6">
                    +57 3125848032
                  </q-item-label>
                </q-item-section>
              </q-item>
            </q-card>
          </q-card-section>
        </q-card>
      </div>

      <div class="col-12 col-md-6">
        <q-card bordered class="shadow-2">
          <q-card-section>
            <div class="text-h5 text-primary">
              Horarios de atención
            </div>
          </q-card-section>

          <q-card-section>
            <q-list separator>
              <q-item v-for="dia in horarios" :key="dia.dia">
                <q-item-section>
                  <q-item-label class="text-weight-medium">
                    {{ dia.dia }}
                  </q-item-label>
                </q-item-section>

                <q-item-section side>
                  <q-chip color="primary" text-color="white" dense square>
                    {{ dia.hora }}
                  </q-chip>
                </q-item-section>
              </q-item>
            </q-list>
          </q-card-section>
        </q-card>
      </div>
    </div>

  </q-page>
</template>

<script setup>
const horarios = [
    { dia: 'Lunes', hora: '7:00AM - 10:00PM'},
    { dia: 'Martes', hora: '7:00AM - 10:00PM'},
    { dia: 'Miercoles', hora: '7:00AM - 10:00PM'},
    { dia: 'Jueves', hora: '7:00AM - 10:00PM'},
    { dia: 'Viernes', hora: '7:00AM - 10:00PM'}
]
</script>

<style scoped>
.banner {
    margin: -24px -24px 0 -24px;
    width: calc(100% + 48px);
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.35);
}
</style>