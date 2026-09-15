<template>
  <q-page class="q-pa-md">

    <q-img
      src="https://github.com/joymarricardopintoortiz/fotos/blob/main/WhatsApp%20Image%202026-09-04%20at%204.47.15%20PM.jpeg?raw=true"
      class="banner"
      :ratio="30/9"
      fit="cover"
    />

    <div class="q-mt-lg">
      <div class="text-h3 text-primary text-weight-bold">
        Cafetería
      </div>

      <p class="text-body1 q-mt-md">
        El Servicio de Cafetería del Centro Agroturístico del SENA ofrece
        una opción de alimentación variada y accesible para aprendices, instructores
        y personal administrativo. Ofrece menús diarios, desayunos, almuerzos y refrigerios
        preparados bajo estrictos controles de higiene, manipulación y conservación de alimentos.
        Cuenta con un área amplia de comedor dotada de mesas y sillas para el consumo cómodo
        durante los recesos de las jornadas lectivas. Asimismo, coordina los horarios de atención
        para garantizar un despacho rápido y ordenado que no interfiera con las clases.
        Se mantienen al día las revisiones sanitarias y el mantenimiento de los equipos de cocina
        para asegurar la salubridad en todo momento. Su objetivo principal es brindar un espacio
        agradable que contribuya al bienestar y la permanencia de la comunidad académica.
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
              <img src="https://github.com/joymarricardopintoortiz/CENTROAGROTURISTICO/blob/main/WhatsApp%20Image%202026-09-11%20at%204.17.48%20PM.jpeg?raw=true">
            </q-avatar>

            <div class="col">
              <div class="text-h6">
                Luisa Carreño
              </div>

              <div class="text-subtitle1">
                Coordinadora de cafetería
              </div>

              <div class="q-mt-sm">
                ✉ Icarreno@sena.edu.com
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
                    +57 3223038451
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
                  <div class="row q-gutter-xs justify-end">
                    <q-chip
                      v-for="(jornada, i) in dia.hora"
                      :key="i"
                      color="primary"
                      text-color="white"
                      dense
                      square
                    >
                      {{ jornada }}
                    </q-chip>
                  </div>
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
    { dia: 'Lunes', hora: ['7:00AM - 12:00PM', '1:00PM - 5:30PM', '7:00PM - 9:30PM'] },
    { dia: 'Martes', hora: ['7:00AM - 12:00PM', '1:00PM - 5:30PM', '7:00PM - 9:30PM'] },
    { dia: 'Miercoles', hora: ['7:00AM - 12:00PM', '1:00PM - 5:30PM', '7:00PM - 9:30PM'] },
    { dia: 'Jueves', hora: ['7:00AM - 12:00PM', '1:00PM - 5:30PM', '7:00PM - 9:30PM'] },
    { dia: 'Viernes', hora: ['7:00AM - 12:00PM', '1:00PM - 5:30PM', '7:00PM - 9:30PM'] },
    { dia: 'Sábados', hora: ['7:30AM - 12:00PM'] }
]
</script>

<style scoped>
.banner {
  margin: -24px -24px 0 -24px;
  width: calc(100% + 48px);
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.35);
}
</style>