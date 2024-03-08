<template>
<div class="cover-container">
    <div class="title-n-sub-container">
        <span class="title-card">Interfaz Sencilla</span>
        <div>
            <span class="text-card">Todas las capacidades en la menor cantidad de pasos.</span>
        </div>
    </div>
    <div class="svg-div">
        <img :src="InterfaceSvg" alt="Interface" class="interface-svg"/>
    </div>
</div>
</template>
  
<script>
import InterfaceSvg from '../assets/Interface.svg';

export default {
name: 'InterfaceShow',
data() {
    return {
    InterfaceSvg // This makes diagramSvg available in the template
    }
},
};
</script>

  
<style scoped>
.cover-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 1em;
}

.title {
    font-size: 32px; /* Adjust the size as needed */
    color: #c6c6c6;
    margin-bottom: 20px; /* Space between title and image */
    font-family: 'IBM Plex Sans', Arial, sans-serif;
    text-align: center;
}

.svg-div {
    display: flex;
    justify-content: center;
    align-items: center;
}

.interface-svg {
    width: auto; /* Adjust the width as needed */
    height: 30em;
}

.text-card {
    font-family: 'IBM Plex Sans', sans-serif;
    font-weight: 200;
    font-size: 1.3em;
}

.title-card {
    font-size: 2em;
}

.title-n-sub-container {
    flex-direction: column;
    padding-left: 3em;
    padding-bottom: 2em;
    align-items: center;
    justify-items: center;
    text-align: center;
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

.interface-svg {
    height: 12em;
}


}
</style>
  