<template>
 <div class="container">

  <div class="rightbox">
    <div class="rb-container">
      <ul class="rb">
        <li class="rb-item" v-for="(item,i) in historial" :key="i">
          <div class="timestamp">
            {{ item.fecha }} <br> {{ item.hora }}
          </div>
          <div class="item-title">{{ item.extracto }}</div>
        </li>
      </ul>

    </div>
  </div>
</div>
</template>

<script>

export default {
  name: 'TimeLine',
  data () {
    return{
      historial : [
        { fecha : '13 feb', hora : '5:00 PM', extracto : 'Fuimos informados que podiamos disfrutar del feriado largo de carnabal en agradecimiento al esfuerzo realizado en pandemia. Nunca antes en la historia de la empresa se detuvo la operacion por tantos dias.'},
        { fecha : '16 feb', hora : '4:00 PM', extracto : 'Se convoca reunion por Zoom. Se comunica que nuestras tareas ya no estan disponibles. La operacion es mudada a Escobar quedando a cargo de Transfarmaco'},
        { fecha : '16 feb', hora : '8:00 PM', extracto : 'Los trabajadores reunidos en asamblea decidimos defender nuestras fuentes de ingreso. Entendiendo que la empresa urdió esta maniobra – vaciando el deposito aprovechando el feriado de carnaval- para deshacerse de nosotros.'},
        { fecha : '17 feb', hora : '7:00 AM', extracto : ' Al presentarnos en Cavia 832, Lomas del Mirador, constatamos con tristeza que en la empresa ya no había nada. Se apersono el apoderado de la compañía ofreciendo reuniones personales, pero negando cualquier negociación colectiva aun en presencia del sindicato (SEOCA)'},
        { fecha : '23 feb', hora : '10:00 AM', extracto : 'Se presenta SEOCA (sindicato empleado de comercio zona oeste) en nuestro deposito indicando que había solicitado la conciliación obligatoria sin previa consulta con nosotros. El Ministerio accede al requerimiento dando plazo de inicio jueves 00:00HS.'},
        { fecha : '26 feb', hora : '1:00 PM', extracto : 'La compañía de manera fraudulenta, nuevamente, simula acatar la misma. Sin embargo, intenta cambiar nuestro horario de ingreso al mismo tiempo que no presenta tarea alguna para realizar.  Mucho menos las que cumplíamos de manera regular y habitual.'},
        { fecha : '1 mar', hora : '10:00 AM', extracto : 'Decidimos que la representación de nuestros derechos colectivos fuera realizada por el sindicato CIS (comercio, industria, servicio) nucleado en la CTA autónoma dado que las herramientas ofrecidas por SEOCA eran insuficientes, generando disconformidad en la asamblea de trabajadores. Ese mismo día denunciamos a Just por vaciamiento, lock out patronal, etc.'},
        { fecha : '4 mar', hora : '10:00 AM', extracto : 'Tomamos la iniciativa de realizar una caravana por los medios de comunicación más relevantes del país para denunciar nuestra situación, como complemento a lo realizado en las redes sociales. Con un balance positivo de la actividad'},
        { fecha : '8 mar', hora : '10:00 AM', extracto : 'La asamblea decide la participación en el día internacional de la mujer trabajadora.'},
        { fecha : '10 mar', hora : '7:00 AM', extracto : 'Realizamos una movilización junto a las organizaciones sociales, partidos políticos, y el sindicato CIS que nos representa a la planta de Just International Latam S.A – de Capitales suizos y socios estratégicos del Just Argentina- en General Rodríguez para seguir reclamando por nuestros puestos de trabajo dado que son solidariamente responsables. Dicha acción se combino con el sindicato UNIA de Suiza que se presento en la planta ubicada en la ciudad de Walsenhausen haciendo suyo nuestro reclamo'}
      ]
    }
  }
}
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=PT+Sans&display=swap");

body {
  background: #e8cbc0;
}

.container {
  background: #232931;
  width: 540px;
  margin: 0 auto;
  position: relative;
  margin-top: 10%;
  box-shadow: 2px 5px 20px rgba(119, 119, 119, 0.5);
}

.leftbox {
  top: -5%;
  left: 5%;
  position: absolute;
  width: 15%;
  height: 110%;
  background-color: #50d890;
  box-shadow: 3px 3px 15px rgba(119, 119, 119, 0.5);
}


.rightbox {
  padding: 0em 34rem 0em 0em;
  height: 100%;
}

.rb-container {
  font-family: "PT Sans", sans-serif;
  width: 50%;
  margin: auto;
  display: block;
  position: relative;
}

.rb-container ul.rb {
  margin: 2.5em 0;
  padding: 0;
  display: inline-block;
}

.rb-container ul.rb li {
  list-style: none;
  margin: auto;
  margin-left: 3em;
  min-height: 50px;
  border-left: 1px dashed #fff;
  padding: 0 0 50px 30px;
  position: relative;
}

.rb-container ul.rb li:last-child {
  border-left: 0;
}

.rb-container ul.rb li::before {
  position: absolute;
  left: -18px;
  top: -5px;
  content: " ";
  border: 8px solid rgba(255, 255, 255, 1);
  border-radius: 500%;
  background: #50d890;
  height: 20px;
  width: 20px;
  transition: all 500ms ease-in-out;
}

.rb-container ul.rb li:hover::before {
  border-color: #232931;
  transition: all 1000ms ease-in-out;
}

ul.rb li .timestamp {
  color: #50d890;
  position: relative;
  width: 300px;
  font-size: 12px;
}

.item-title {
  color: #fff;
}

.container-3 {
  width: 5em;
  vertical-align: right;
  white-space: nowrap;
  position: absolute;
}


</style>
