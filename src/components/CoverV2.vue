<template>
    <div class="cover-container">
        <div class="title-n-sub-container">
            <span class="title-card">
                Analiza cualquiera cosa, en cualquier archivo, en segundos.
            </span>
            <p>
                Identifica patrones, encuentra información, sintetiza datos, resuelve problemas.
            </p>
        </div>

        <div class="svg-div">
            <img :src="DiagramSvg" alt="Diagram" class="diagram-svg"/>
        </div>

    </div>
  </template>
  
  <script>
  import DiagramSvg from '../assets/CoFlow.svg';
  
  export default {
    name: 'CoverComponent',
    data() {
      return {
        DiagramSvg // This makes DiagramSvg available in the template
      }
    },
  };
  </script>
  
<style scoped>
.cover-container {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: 1em 4em;
}

.title {
    font-size: 32px; /* Adjust the size as needed */
    color: #c6c6c6;
    margin-bottom: 20px; /* Space between title and image */
    font-family: 'IBM Plex Sans', Arial, sans-serif;
    text-align: start;
}

.svg-div {
    display: flex;
    justify-content: center;
    align-items: center;
}

.diagram-svg {
    width: auto; /* Adjust the width as needed */
    height: 20em;
}

.title-card {
    font-size: 2em;
    color: #fff;
}

.title-n-sub-container {
    flex-direction: column;
    padding-left: 3em;
}



@media (max-width: 768px) { /* For mid-sized screens */
.diagram-svg {
    height: 8em;
}

.cover-container {
    flex-direction: column;
    padding: 1em 1em;
}

.title-n-sub-container {
    padding-left: 0em;
}

}
</style>
  