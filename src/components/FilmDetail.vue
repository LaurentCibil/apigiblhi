<style>
body {
  display: flex;
  align-items: center;
  justify-content: center;
}
#containerDetail {
  overflow: hidden;
  box-shadow: 10px 5px 5px;
  border-radius: 15px;
  border: solid;
  align-self: center;
  max-width: 1200px;
  display: flex;
  flex-direction: column;
}
#imgDetail {
  overflow: hidden;
  border-radius: 35px;
  padding: 20px;
  max-width: 400px;
}
#header {
  overflow: hidden;
  flex-wrap: wrap;
  border-top-right-radius: 15px;
  border-top-left-radius: 15px;
  background-color: antiquewhite;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
#banner {
  overflow: hidden;
  padding: 20px;
  justify-content: center;
  background-color: antiquewhite;
  display: flex;
  flex-direction: row;
}
#bannerDetail {
  border-radius: 1%;
  object-fit: fill;
  width: 300%;
}
#resumeDetail {
  overflow: hidden;
  border-bottom-left-radius: 15px;
  border-bottom-right-radius: 15px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: antiquewhite;
  padding: 20px;
}
#pResume,
#h2Resume {
  overflow: hidden;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 600px;
}
</style>

<template>
  <div id="containerDetail">
    <div id="header">
      <!-- ici on met:
        sur la partie gauche 
            l'affiche du film en plus grand a gauche
        sur la partie droite
            le titre
      what else??? :o-->
      <div id="afficheDetail">
        <img
          id="imgDetail"
          alt="Castle in the sky"
          src="https://image.tmdb.org/t/p/w600_and_h900_bestv2/npOnzAbLh6VOIu3naU5QaEcTepo.jpg"
        />
      </div>
      <div id="titreEtinfosDetail">
        <h1>
          <!-- Le titre et l'année dans le h1 -->
          Castle in the Sky
        </h1>
        <p id="titreOriginal">
          Titre original : 天空の城ラピュタ
          <span id="titreOriginalRomanised">(Tenkū no shiro Rapyuta)</span>
        </p>
        <p id="directeur">
          <span>Directeur :</span>
          <span style="font">Hayao Miyazaki</span>
        </p>
        <p id="producteur">
          <span>Producteur :</span>
          <span>Isao Takahata</span>
        </p>
        <p id="anneeSortie">
          <span>Année de sortie</span>
          <span>1986</span>
        </p>
        <p id="dureeFilm">
          <span>Durée du film :</span>
          <span>126 minutes</span>
        </p>
        <p id="rtScore">
          <span>RT score :</span>
          <span>95</span>
        </p>
      </div>
    </div>
    <div id="banner">
      <!-- ici on met la bannier du film -->
      <img
        id="bannerDetail"
        src="https://image.tmdb.org/t/p/w533_and_h300_bestv2/3cyjYtLWCBE1uvWINHFsFnE8LUK.jpg"
        alt="baniere film castle in the sky"
      />
    </div>
    <div id="resumeDetail">
      <!-- ici le resumé -->
      <h2 id="h2Resume">Résumé</h2>
      <p id="pResume">
        The orphan Sheeta inherited a mysterious crystal that links her to the
        mythical sky-kingdom of Laputa. With the help of resourceful Pazu and a
        rollicking band of sky pirates, she makes her way to the ruins of the
        once-great civilization. Sheeta and Pazu must outwit the evil Muska, who
        plans to use Laputa's science to make himself ruler of the world.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "FilmDetail",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style lang="scss" scoped></style>
