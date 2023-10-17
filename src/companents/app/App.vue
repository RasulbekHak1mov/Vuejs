<template>
  <div class="app t-uppercase">
    <div class="content">
      <div class="app-info">
        <appInfo />
      </div>
      <div class="sreach-panel">
        <sreachPanel />
      </div>
      <div>
        <movieList />
      </div>
      <div>
        <movieAddList />
      </div>
    </div>
  </div>
</template>


<script>
import sreachPanel from '../sreach-panel/sreachPanel.vue'
import movieList from '../movie-list/movieList.vue'
import appInfo from '../app-info/appInfo.vue'
import movieAddList from '../movie-add-list/movieAddList.vue'
export default {
  components: {
    sreachPanel,
    movieList,
    appInfo,
    movieAddList,
  },
}
</script>


<style>
.app {
  height: 100vh;
  color: #000;
}

.content {
  width: 1000px;
  min-height: 700px;
  background: #fff;
  margin: 0 auto;
  padding: 1.5rem 0;
}

.sreach-panel {
  margin-top: 2rem;
  padding: 1.5rem;
  background-color: #fcfaf5;
  border-radius: 4px;
  box-shadow: 15px 15px 15px rgba(0, 0, 0, 0.15);
}
</style>