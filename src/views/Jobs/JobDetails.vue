<template>
        <h1>Job Details</h1>
        <!-- Job details would be dynamically loaded based on job ID -->
        <!-- For demonstration, using static content -->
    <p>job id is {{ $route.params.id }}</p>
     <!-- <div>
        <h2>{{ job.title }}</h2>
         
            <p>{{ job.company }} - {{ job.location }}</p>
            <p>Type: {{ job.type }}</p>
            <p>{{ job.details }}</p>
            <hr/>
            </div> -->
</template>

<script>
    export default {
        name: 'JobDetails',
        props: ['id'],
        // data() {
        //     return {
        //         job: {
        //             id:this.$route.params.id,
                  
        //         },

        //     }
        // }


    }
</script>

<style scoped>



</style>