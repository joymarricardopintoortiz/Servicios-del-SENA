<template>
  <q-page class="q-pa-md">

    <q-img
      src="https://github.com/joymarricardopintoortiz/fotos/blob/main/WhatsApp%20Image%202026-09-07%20at%2012.35.10%20PM.jpeg?raw=true"
      class="banner"
      :ratio="30/9"
      fit="cover"
    />

    <div class="q-mt-lg">
      <div class="text-h3 text-primary text-weight-bold">
        Coordinación
      </div>

      <p class="text-body1 q-mt-md">
        La Coordinación Académica del Centro Agrotrístico del SENA cumple
        un rol fundamental en la gestión, orientación y aseguramiento de la calidad de
        los procesos formativos institucionalizados. Entre sus labores principales destaca
        el acompañamiento permanente a la plantilla de instructores, garantizando la correcta
        ejecución de los diseños curriculares vigentes y el seguimiento al desarrollo integral
        de los aprendices. Asimismo, gestiona la programación de los ambientes de aprendizaje,
        administra los recursos e insumos requeridos para la práctica técnica y supervisa el
        cumplimiento estricto de los calendarios académicos. Es la instancia encargada de
        atender peticiones, evaluar el desempeño de las actividades formativas, articular
        las etapas lectiva y productiva, y velar por el cumplimiento del reglamento del aprendiz.
        Su gestión objetiva asegura la continuidad institucional, promoviendo la excelencia,
        el respeto a la normatividad y el impacto positivo de la formación en la región.
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
              <img src="https://github.com/joymarricardopintoortiz/CENTROAGROTURISTICO/blob/main/WhatsApp%20Image%202026-09-11%20at%204.17.47%20PM%20(1).jpeg?raw=true">
            </q-avatar>

            <div class="col">
              <div class="text-h6">
                Luis Carlos Reina
              </div>

              <div class="text-subtitle1">
                Coordinador Académico
              </div>

              <div class="q-mt-sm">
                ✉ lreinas@sena.edu.com
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
                    +57 3166783027
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
    { dia: 'Lunes', hora: '7:30AM - 12:00PM'},
    { dia: 'Martes', hora: '7:30AM - 12:00PM'},
    { dia: 'Miercoles', hora: '7:30AM - 12:00PM'},
    { dia: 'Jueves', hora: '7:30AM - 12:00PM'},
    { dia: 'Viernes', hora: '7:30AM - 12:00PM'}
]
</script>

<style scoped>
.banner {
    margin: -24px -24px 0 -24px;
    width: calc(100% + 48px);
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.35);
}
</style>