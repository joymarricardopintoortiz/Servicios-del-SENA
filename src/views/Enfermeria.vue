<template>
  <q-page class="q-pa-md">

    <q-img
      src="https://github.com/joymarricardopintoortiz/fotos/blob/main/WhatsApp%20Image%202026-09-04%20at%205.14.12%20PM.jpeg?raw=true"
      class="banner"
      :ratio="30/9"
      fit="cover"
    />

    <div class="q-mt-lg">
      <div class="text-h3 text-primary text-weight-bold">
        Enfermería
      </div>

      <p class="text-body1 q-mt-md">
        En un centro donde los aprendices pasan largas jornadas entre
        cultivos, animales, cocinas de práctica y talleres, tener un
        punto de enfermería cerca no es un detalle menor. Aquí se
        atienden desde un corte con una herramienta de campo hasta un
        mareo por el sol después de una jornada larga en los
        invernaderos o en las zonas de producción. También se hace
        seguimiento a quienes manejan alguna condición de salud previa
        y necesitan que alguien esté pendiente durante sus prácticas.
        El servicio no se limita a la urgencia: incluye orientación
        sobre autocuidado, prevención de accidentes propios del trabajo
        agropecuario y turístico, y un espacio de confianza para
        resolver dudas de salud sin tener que salir del centro. La idea
        es simple, que ningún aprendiz o funcionario sienta que está
        solo si algo pasa mientras aprende su oficio.
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
              <img src="https://github.com/joymarricardopintoortiz/CENTROAGROTURISTICO/blob/main/WhatsApp%20Image%202026-09-11%20at%204.17.48%20PM%20(2).jpeg?raw=true">
            </q-avatar>

            <div class="col">
              <div class="text-h6">
                María Fernanda Gómez Reyes
              </div>

              <div class="text-subtitle1">
                Enfermera
              </div>

              <div class="q-mt-sm">
                ✉ Mafecita1118@gmail.com
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
                    +57 32114153995
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
    { dia: 'Lunes', hora: ['6:30AM - 10:30AM', '4:00PM - 8:00M']},
    { dia: 'Martes', hora: ['6:30AM - 10:30AM', '4:00PM - 8:00M']},
    { dia: 'Miercoles', hora: ['6:30AM - 10:30AM', '4:00PM - 8:00M']},
    { dia: 'Jueves', hora: ['6:30AM - 10:30AM', '4:00PM - 8:00M']},
    { dia: 'Viernes', hora: ['6:30AM - 10:30AM', '4:00PM - 8:00M']}
]
</script>

<style scoped>
.banner {
    margin: -24px -24px 0 -24px;
    width: calc(100% + 48px);
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.35);
}
</style>