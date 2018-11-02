<template>

  <p>

    <g2-line :charData="serverData" :id="'c1'" :weight="600" :height="400"></g2-line>

  </p>

</template>

<script>

import G2Line from './G2Line.vue'
export default {

  components: {

    G2Line

  },
  data () {
    return {
      serverData: ''
    }
  },
  created: function () {
    this.serverData =
        [{

          year: '2010',

          value: 3

        }, {

          year: '2011',

          value: 4

        }, {

          year: '2012',

          value: 3.5

        }, {

          year: '2013',

          value: 5

        }, {

          year: '2014',

          value: 4.9

        }, {

          year: '2015',

          value: 6

        }, {

          year: '2016',

          value: 7

        }, {

          year: '2017',

          value: 9

        }, {

          year: '2018',

          value: 13

        }]
  }

  // 此处省略从服务器获取数据并且赋值给this.serverData

  // 推荐使用axios请求接口

}

</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1, h2 {
    font-weight: normal;
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #42b983;
  }
</style>
