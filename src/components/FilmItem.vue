<style>
h1 {
  letter-spacing: 3px;
  font-family:Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
  align-items: center;
}
#container {
  opacity: 60%;
  justify-content: center;
  margin: 50px;
  max-width: 600px;
  border-radius: 15px;
  border: solid;
  box-shadow: 10px 5px 5px;
  background-color: antiquewhite;
  border-block-color: rgb(0, 0, 0);
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  transition: 0.1s;
}
#container:hover {
  opacity: 100%;
  transition: all 0.4s ease;
  transform: scale(1.05);
}

#affiche{
  margin: 10;
}
#img {  
  transition: .7s;
  margin-right: 15px;
  border-radius: 10px;
  margin: 18px;
  height: auto;
  width: auto;
  max-height: 300px;
  max-width: 300px;
}
#img:hover {  
  transform: scale(1.1);
}
#titreEtResume {
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin-left: 15px;
  margin-bottom: 15px;
  max-width: 300px;
}
</style>

<template>
  <!-- container -->
  <div id="container">
    <!-- affiche du film -->
    <div id="affiche">
      <img
        id="img"
        alt="Castle in the sky"
        src="https://image.tmdb.org/t/p/w600_and_h900_bestv2/npOnzAbLh6VOIu3naU5QaEcTepo.jpg"
      />
    </div>
    <!-- la on met le titre et le resumé du film a droite de l'affiche -->
    <div id="titreEtResume">
      <h1>
        <!-- Le titre et l'année dans le h1 -->
        Castle in the Sky
        <span style="font-size : 15px">(1987)</span>
      </h1>
      <!-- et tout de suite apres le h1, un span pour le resume -->
      <p>The orphan Sheeta inherited a mysterious crystal that links her to the mythical sky-kingdom of Laputa. With the help of resourceful Pazu and a rollicking band of sky pirates, she makes her way to the ruins of the once-great civilization. Sheeta and Pazu must outwit the evil Muska, who plans to use Laputa's science to make himself ruler of the world.</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "FilmItem",
  created() { },
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style lang="scss" scoped>
</style>