<template>
    <img
      :src= "image.image" 
      class="profile"
      alt="profile"
    />
</template>
<script>
export default{
    props:{ 
        image: {
            type: Object,
            default:{
                
                    image: "https://img.freepik.com/foto-gratis/adorable-perro-basenji-marron-blanco-sonriendo-dando-maximo-cinco-aislado-blanco_346278-1657.jpg?w=996&t=st=1672255558~exp=1672256158~hmac=04d6604fd843762169374f41b8b5e79e461f0ec0b6ca2a49aa3242aa45e04c55"
                
            }                       
        }
    }
}
</script>