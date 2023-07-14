
<div class="container">
<slot/>
</div>
<style>
.container {
  width: 100vw;
  height: 100vh;
@media screen and (min-width: 500px){
  width: 375px;
  height: 667px;
  border: 5px solid grey;
  border-radius: 20px;
}
}
</style>
