<template>
    <q-page class="q-pa-lg">
        <div class="text-center q-mb-xl hero-title-box">
            <div class="text-h2 text-primary text-weight-bold">
                SENA - Centro Agroturistico
            </div>
            <p class="text-h6 text-grey-9">
                Conoce nuestros servicios y encuentra la información que necesitas.
            </p>
        </div>

        <div class="row q-col-gutter-lg">
            <div class="col-12 col-md-4">
                <q-card class="service-card info-card">
                    <q-card-section class="text-center">
                        <q-icon name="eco" color="primary" size="40px" />
                        <div class="text-h6 text-primary q-mt-sm">
                            ¿Quiénes somos?
                        </div>
                        <p class="text-body2 q-mt-sm text-left">
                            El Centro Agroturístico del SENA en San Gil es una sede
                            enfocada en la formación técnica y tecnológica en áreas
                            agropecuarias y turísticas. Aquí los aprendices desarrollan
                            competencias prácticas en un entorno rural, combinando el
                            aprendizaje académico con proyectos productivos reales.
                        </p>
                    </q-card-section>
                </q-card>
            </div>

            <div class="col-12 col-md-4">
                <q-card class="service-card info-card">
                    <q-card-section class="text-center">
                        <q-icon name="flag" color="primary" size="40px" />
                        <div class="text-h6 text-primary q-mt-sm">
                            Nuestra misión
                        </div>
                        <p class="text-body2 q-mt-sm text-left">
                            Formar aprendices íntegros y competitivos, con sólidos valores
                            éticos y un fuerte sentido de responsabilidad ambiental,
                            capaces de aportar al desarrollo agropecuario y turístico de
                            la región de Santander y del país.
                        </p>
                    </q-card-section>
                </q-card>
            </div>

            <div class="col-12 col-md-4">
                <q-card class="service-card info-card">
                    <q-card-section class="text-center">
                        <q-icon name="groups" color="primary" size="40px" />
                        <div class="text-h6 text-primary q-mt-sm">
                            Nuestra comunidad
                        </div>
                        <p class="text-body2 q-mt-sm text-left">
                            Contamos con áreas de bienestar, enfermería, biblioteca,
                            cafetería y coordinación académica, pensadas para acompañar
                            a nuestros aprendices durante todo su proceso de formación
                            dentro y fuera del aula.
                        </p>
                    </q-card-section>
                </q-card>
            </div>
        </div>
    </q-page>
</template>

<style scoped>
.service-card {
    height: 100%;
    border-radius: 15px;
}

.q-page {
    background-image: linear-gradient(rgba(255, 255, 255, 0.45), rgba(255, 255, 255, 0.45)), url('../assets/Sena_-sangil.jpg');
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
}

.hero-title-box {
    background: rgba(255, 255, 255, 0.92);
    border-radius: 16px;
    padding: 24px 32px;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.15);
}

.info-card .text-h6 {
    font-size: 1.25rem;
    font-weight: 600;
    margin-top: 10px;
    margin-bottom: 4px;
}

.info-card .text-body2 {
    font-size: 0.95rem;
    line-height: 1.65;
    color: #4a4a4a;
}

.hero-title-box .text-h2 {
    letter-spacing: -0.01em;
}

.hero-title-box .text-h6 {
    font-family: 'Inter', sans-serif;
    font-weight: 400;
    color: #555;
}
</style>