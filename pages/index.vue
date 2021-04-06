<template>
  <div class="container">
    <div>
      <logo />
      <coverflow :coverList="coverList" :coverWidth="260" :index="2" :coverShadow="true"></coverflow>
    </div>
  </div>
  </div>
</template>
 
<script>
import Logo from '~/components/Logo.vue'
 
export default {
  name: 'Nuxttest',
  components: {
    Logo
  },
  data () {
    return {
      coverList: [
        {
          cover: 'https://cdn.pixabay.com/photo/2020/02/10/16/50/orchid-4837017_960_720.jpg',
          title: '蘭'
        }, {
          cover: 'https://cdn.pixabay.com/photo/2020/02/10/16/51/hyacinth-4837019_960_720.jpg',
          title: 'ヒヤシンス'
        }, {
          cover: 'https://cdn.pixabay.com/photo/2020/02/16/15/37/tulips-4853899_960_720.jpg',
          title: 'チューリップ'
        }, {
          cover: 'https://cdn.pixabay.com/photo/2020/02/17/20/26/nettled-iris-4857753_960_720.jpg',
          title: 'アイリス'
        }, {
          cover: 'https://cdn.pixabay.com/photo/2020/02/15/19/00/rose-yellow-4851780_960_720.jpg',
          title: 'バラ'
        }, {
          cover: 'https://cdn.pixabay.com/photo/2020/02/11/12/56/magnolia-4839469_960_720.jpg',
          title: 'マグノリア'
        }
      ]
    }
  }
}
</script>
<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>