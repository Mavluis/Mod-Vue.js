<template>
    <div>
        {{msg}} <br/>
        <velocimetro :velocidad="velocidad"></Velocimetro> <br/>
        <Pedal msg="Freno" @action="frenar()"></Pedal>
        <Pedal msg="Acelerador" @action="acelerar()"></Pedal>
    </div>
</template>
<script>
import Velocimetro from './Velocimetro.vue'
import Pedal from './Pedal.vue'
    export default {
        data() {
            return {
                velocidad : 0
            }
        },
        components : {
            Velocimetro,
            Pedal
        },
        props: {
            msg: String
        },
        methods : {
            acelerar (){
                this.velocidad++;
            },
            frenar (){
                this.velocidad--;
            }
        }
    }
</script>
