<template>
        <h1>Jobs </h1>
        <div v-for="job in jobs" :key="job.id" class="job"> 
            <router-link :to="{name:'JobDetails', params:{id:job.id}}"> <h2>{{ job.title }}</h2></router-link> 
         
         

        </div>

</template>

<script>
    export default {
        name: 'Jobs',
        data() {
            return {
                jobs: [
                    {id:1, details:'lorem',title:'Frontend Developer', company:'Google', location:'New York', type:'Full-time'},
                    {id:2, details:'lorem',title:'Backend Developer', company:'Facebook', location:'San Francisco', type:'Part-time'},
                    {id:3, details:'lorem',title:'Full Stack Developer', company:'Amazon', location:'Seattle', type:'Contract'},
                    {id:4, details:'lorem',title:'DevOps Engineer', company:'Microsoft', location:'Austin', type:'Full-time'},
                    {id:5, details:'lorem',title:'Data Scientist', company:'Apple', location:'Boston', type:'Internship'}

                ]
            }
        }
        
    }
</script>

<style scoped>

.job h2 {
    background: #f4f4f4;
    padding: 20px;
    border-radius: 10px;
    margin: 10px auto;
    max-width: 600px;
    cursor: pointer;
    color: #444;
  }

  .job h2:hover {
    background: #ddd;
  }

  .job a {
    text-decoration: none;
  }
</style>