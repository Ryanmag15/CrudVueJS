<template>
    <div class="formulario">

        <div class="formulario-title">{{title}}</div><br>
        <label>Pasta </label><br>
        <input type="text" v-model="pasta"><br><br>   
        <label>CNJ </label><br>
        <input type="text" v-model="cnj"><br><br>   
        <label>Lista </label><br>
        <input type="text" v-model="lista"><br><br>   

        <button v-on:click="adicionarProcessos" type="submit" class="btn btn-primary">Enviar</button><br>

        <table class="table">
            <thead>
                <tr>
                  <th scope="col">id</th>
                  <th scope="col">Pasta</th>
                  <th scope="col">Numero CNJ</th>
                  <th scope="col">Lista Negativa</th>
                  <th scope="col">Acoes</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="(processo, index) in processos" :key="index">
                  <td>{{processo.index}}</td>
                  <td>{{processo.pasta}}</td>
                  <td>{{processo.cnj}}</td>
                  <td>{{processo.lista}}</td>
                  <td>
                  <td><button type="button" class="btn btn-warning">Editar</button></td>
                  <td><button v-on:click="removeProcessos(index)" type="submit" class="btn btn-danger">Deletar</button></td>
                  </td>
                </tr>
            </tbody>
        </table>

    </div>
</template>

<script>

export default {
    name: 'Formulario',
    props: {

    },
    data(){
        return {
            title: 'Formulario para adicionar processos',
            pasta: '',
            cnj: '',
            lista: '',
            processos: [] 
        }
    },
    methods: {
        adicionarProcessos () {
            this.processos.push({
                pasta: this.pasta,
                cnj: this.cnj,
                lista: this.lista
            })

            this.pasta = '',
            this.cnj = '',
            this.lista = ''
        },

        editarProcessos (index) {
           
        },

        removeProcessos (index) {
            this.processos.splice(index, 1)
        }
    }
}

</script>

<style>

</style>