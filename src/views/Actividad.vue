<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
  
      #Actividad                
        <Actividad :cuestionario="cuestionario"/>
  
  </template>

<script>
import Actividad from 'ecored-pkg-fliz/plugin/components/actividad/Actividad.vue'
export default {
  name: 'ActividadDidactica',
  components: {
    Actividad,
  },
  data: () => ({
    cuestionario: {
      tema: 'Ajustes y cierre del periodo contable según normativa NIIF',
      titulo: 'Cuestionario',
      introduccion:
        '<b>Objetivo:</b> Identificar los conceptos clave relacionados con los ajustes contables y el cierre del ciclo contable conforme a la normativa financiera vigente, especialmente las NIIF.',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!..',
      titulo_reprobado: 'VUELVA A INTENTARLO..',
      preguntas: [
        {
          id: 1,
          texto: '¿Cuál es el objetivo principal de los asientos de ajuste?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Reflejar el costo de los activos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Revisar el balance de prueba.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Corregir errores u omisiones contables.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Verificar el arqueo de caja.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 2,
          texto:
            '¿Qué norma se aplica para el deterioro del valor de los activos?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'NIC 21.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'NIC 2.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'NIC 36.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'NIIF 9.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 3,
          texto:
            'Según la NIC 36, ¿qué debe hacerse si el valor en libros excede el importe recuperable?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Actualizar el valor residual.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Reconocer una pérdida por deterioro.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Aumentar la vida útil del activo.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Realizar una revaluación fiscal.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 4,
          texto:
            '¿Cuál de las siguientes cuentas representa un gasto pagado por anticipado?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Arrendamientos.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Proveedores.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Depreciación acumulada.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Ingresos ordinarios.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 5,
          texto:
            '¿Qué método de depreciación genera un mayor gasto en los primeros años?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Método de depreciación acelerada.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Método de línea recta.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Método de unidades de producción.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Método de valor residual.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 6,
          texto:
            '¿Qué elemento se utiliza para calcular la depreciación bajo el método de línea recta?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Tasa del mercado.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Vida útil del activo.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Tasa de inflación.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Tasa de descuento.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 7,
          texto:
            '¿Cuál es el tratamiento contable de un faltante injustificado en caja?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Se registra como cuenta por cobrar al trabajador.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Se considera ingreso no operativo.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Se elimina del balance.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Se amortiza como gasto financiero.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 8,
          texto:
            'En la conciliación bancaria, ¿qué representa una nota débito por GMF?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Un gasto financiero.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Un ingreso por intereses.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Una diferencia en cambio.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Una provisión para deterioro.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 9,
          texto:
            '¿Cuál de las siguientes cuentas debe cerrarse al final del periodo contable?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Gastos financieros.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Bancos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Proveedores.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Clientes.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 10,
          texto:
            '¿Qué documento recopila los ajustes, balances y estados financieros en un solo lugar?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Balance de prueba.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Estado de situación financiera.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Hoja de trabajo.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Notas a los estados financieros.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 11,
          texto:
            'El balance de prueba ajustado se elabora antes del comprobante de ajustes.',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Falso.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Verdadero.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 12,
          texto: 'La amortización se aplica únicamente a activos tangibles.',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Falso.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Verdadero.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 13,
          texto:
            'Un aumento en la tasa de cambio puede generar una diferencia en cambio negativa.',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Falso.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Verdadero.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 14,
          texto:
            'El valor residual es considerado en el cálculo de la depreciación.',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Falso.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Verdadero.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 15,
          texto:
            'Los activos intangibles con vida útil indefinida no se amortizan.',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Falso.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Verdadero.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
