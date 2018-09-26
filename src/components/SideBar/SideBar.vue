<template lang="html">

  <div id="parentx">

    <vs-button @click="active=!active" vs-color="danger" vs-type="filled">Mostrar a Barra Lateral</vs-button>
    <vs-sidebar parent="body" default-index="1"  color="primary" class="sidebarx" spacer v-model="active">

      <div class="header-sidebar" slot="header">
        <vs-avatar  size="100px" src="https://abrilveja.files.wordpress.com/2018/08/img201604161637545987481.jpg"/>

        <h4>
          Cabo Daciolo
          <vs-button vs-color="primary" vs-icon="more_horiz" vs-type="flat"></vs-button>
        </h4>

      </div>


      <!-- <vs-sidebar-item index="1" icon="question_answer">
        Dashboard
      </vs-sidebar-item>

      <vs-sidebar-item index="2" icon="gavel">
        History
      </vs-sidebar-item>

      <vs-divider icon="person" position="left">
        User
      </vs-divider>

      <vs-sidebar-item index="3" icon="verified_user">
        Configurations
      </vs-sidebar-item>
      <vs-sidebar-item index="4" icon="account_box">
        Perfile
      </vs-sidebar-item> -->

      <vs-sidebar-item index="5" >
       <vs-input vs-label="Título da Página" vs-placeholder="Digite o título" v-model="titulo"/>
        <vs-input type="password" vs-label="Password" vs-placeholder="Disabled" v-model="pw"/>
      </vs-sidebar-item>

      <vs-sidebar-item index="6">
        <vs-button vs-color="success" vs-type="gradient">Salvar</vs-button>
      </vs-sidebar-item>

      

      <div class="footer-sidebar" slot="footer">
        <vs-button vs-icon="reply" vs-color="danger" vs-type="flat">log out</vs-button>
        <vs-button vs-icon="settings" vs-color="primary" vs-type="border"></vs-button>
      </div>

    </vs-sidebar>
  </div>

</template>

<script>
export default {
  name: 'SideBar',  
  data:()=>({
    active:false,
  })
}
</script>

<style lang="stylus">
.header-sidebar
  display flex
  align-items center
  justify-content center
  flex-direction column
  width 100%
  h4
    display flex
    align-items center
    justify-content center
    width 100%
    > button
      margin-left 10px
.footer-sidebar
  display flex
  align-items center
  justify-content space-between
  width 100%
  > button
      border 0px solid rgba(0,0,0,0) !important
      border-left 1px solid rgba(0,0,0,.07) !important
      border-radius 0px !important
</style>