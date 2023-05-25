<template>
    <div class="main-container">
        <div class="project-card" v-for="(items, index) in projectData.ProjectsArray" v-bind:key="items">
            <h2>{{projectData.ProjectsArray[index].Title}}</h2>
            <img :src="projectData.ProjectsArray[index].Image" alt="">
            <p>{{projectData.ProjectsArray[index].About}}</p>
        </div>
    </div>

</template>

<script>
import jsonData from "/projects.json"
export default {
    name: "ProjectsCard",
    data() {
        return{
            projectData: jsonData
        }
    }
}
</script>

<style scoped>
  .main-container{
      display: flex;
      justify-content: center;
      align-items: center;
      flex-wrap: wrap;
  }
  .project-card{
      margin: 10px;
      width: 30rem;
      padding: 10px;
      flex-wrap: 0 0 40%;
      background-color: #fff;
      border-radius: 25px;
      box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  }
  .project-card img {
      height: 10rem;
      width: 23rem;
  }

  .project-card:hover{
      transform: scale(1.3);
      transition: 0.8s;


  }
</style>