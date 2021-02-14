<template>
  <div id="app">
    <div class="vue-radio">
     <input type="radio" id="tab_1" value="1" v-model="tab" />
     <label for="tab_1">タブメニュー1</label>
     <input type="radio" id="tab_2" value="2" v-model="tab" />
     <label for="tab_2">タブメニュー2</label>
     <input type="radio" id="tab_3" value="3" v-model="tab" />
     <label for="tab_3">タブメニュー3</label>
    </div>

    <ul class="contents">
      <li v-if="tab === '1'">コンテンツ1コンテンツ1コンテンツ1コンテンツ1コンテンツ1コンテンツ1コンテンツ1コンテンツ1</li>
      <li v-if="tab === '2'">コンコンテンツ2テンツ2コンテンツ2コンテンツ2コンテンツ2コンテンツ2コンテンツ2コンテンツ2</li>
      <li v-if="tab === '3'">コンテンツ3コンテンツ3コンテンツ3コンテンツ3コンテンツ3コンテンツ3コンテンツ3コンテンツ3</li>
    </ul>
  </div>
</template>

<style>
  label{
    background: #000;
    color: #fff;
    text-decoration: none;
    padding: 3px 20px;
    margin-right: 2px;
    cursor: pointer;
  }

  input{
    display:none;
  }
  ul{
    margin-top: 2px;
    padding: 1em;
    border: 1px solid #ccc;
  }

  li{
    list-style: none;
  }
</style>

<script>
export default {
  data() {
    return {
      tab:"1"
    };
  },
};

</script>