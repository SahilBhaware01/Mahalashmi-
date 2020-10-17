<template>
  <div id="app">
  <!-- ///////////////header 1 -->
  <div class="sticky-top">
  <b-navbar toggleable="lg" type="dark" variant="info">
    

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
     
      <!--  -->
      
      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="Search"></b-form-input>
          <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
        </b-nav-form>

        

        <b-nav-item-dropdown right>
          <!-- Using 'button-content' slot -->
          <template v-slot:button-content>
            <em><b-avatar variant="primary" text="SB"></b-avatar></em>
          </template>
          <b-dropdown-item href="#"> Profile</b-dropdown-item>
          <b-dropdown-item href="#">Sign Out</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
  <div class="container2">
  <b-nav tabs align="center">
    <b-nav-item>Active</b-nav-item>
    <b-nav-item>Link</b-nav-item>
    <b-nav-item>Link with a long name </b-nav-item>
    <b-nav-item>link4</b-nav-item>
  </b-nav>
</div>
</div>

  <!-- /////////////// -->
   
  <!-- ///////////////header 2 -->

  <!-- /////////////// -->
  <!-- https://drive.google.com/file/d/1YT2DaxUj_hOBkWjtE36Mc90S9PO4QLra/view?usp=sharing -->
   <!-- //////////////////corosel -->
 <appHome></appHome>
  <!-- ////////////////////////////////////////////////////////////////////////////footer -->
  <div class="container3">
  <!-- Footer -->
  <mdb-footer color="indigo" class="font-small pt-0">
    <mdb-container>
      <mdb-row class="pt-5 mb-3 text-center d-flex justify-content-center">
        <mdb-col md="2" class="b-3">
          <h6 class="title font-weight-bold"><a href="#!">About us</a></h6>
        </mdb-col>
        <mdb-col md="2" class="b-3">
          <h6 class="title font-weight-bold"><a href="#!">Products</a></h6>
        </mdb-col>
        <mdb-col md="2" class="b-3">
          <h6 class="title font-weight-bold"><a href="#!">Awards</a></h6>
        </mdb-col>
        <mdb-col md="2" class="b-3">
          <h6 class="title font-weight-bold"><a href="#!">Help</a></h6>
        </mdb-col>
        <mdb-col md="2" class="b-3">
          <h6 class="title font-weight-bold"><a href="#!">Contact</a></h6>
        </mdb-col>
      </mdb-row>
      <hr class="rgba-white-light" style="margin: '0 15%'" />
      <mdb-row class="d-flex text-center justify-content-center mb-md-0 mb-4">
        <mdb-col md="8" sm="12" class="mt-5">
          <p style="lineHeight: '1.7rem'">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium
            doloremque laudantium</p>
        </mdb-col>
      </mdb-row>
      <hr class="clearfix d-md-none rgba-white-light" style="margin: '10% 15% 5%'" />
      <mdb-row class="pb-3">
        <mdb-col md="12">
          <div class="mb-5 flex-center">
            <a class="fb-ic"><i class="fab fa-facebook fa-lg white-text mr-md-4"> </i></a>
            <a class="tw-ic"><i class="fab fa-twitter fa-lg white-text mr-md-4"> </i></a>
            <a class="gplus-ic"><i class="fab fa-google-plus fa-lg white-text mr-md-4"> </i></a>
            <a class="li-ic"><i class="fab fa-linkedin-in fa-lg white-text mr-md-4"> </i></a>
            <a class="ins-ic"><i class="fab fa-instagram fa-lg white-text mr-md-4"> </i></a>
            <a class="pin-ic"><i class="fab fa-pinterest fa-lg white-text"> </i></a>
          </div>
        </mdb-col>
      </mdb-row>
    </mdb-container>
    
  </mdb-footer>
  <!-- Footer -->
  </div>
  <!-- //////////////////////////// -->
  ///////////////////////////////////////////////////////////////////////////////////////////////////////////
  <appHello></appHello>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Homepage from './components/homepage.vue'
import { mdbFooter, mdbContainer, mdbRow, mdbCol } from 'mdbvue';
export default {
  name: 'App',
  components: {
    appHello:HelloWorld,
    appHome:Homepage,
     mdbFooter,
      mdbContainer,
      mdbRow,
      mdbCol
  }
}
</script>

<style scoped>
  
  .container3{
   margin-top:40px;
   border:1em solid #17a2b8;
   border-left:3em solid #17a2b8;
   border-right:3em solid #17a2b8;
  }
  .container2{
    margin:3px;
    padding:1px;
    background-color:white;
    border-radius:5px;
    
  }
 
</style>
