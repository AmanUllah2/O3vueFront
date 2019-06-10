<template>
<!-- Text and Text Field -->
<div class = "field">
<div class="text">
<div class="textsize">
<h2>Group "Name"</h2>
</div>
</div>
<div class="text">
<h3>Welcome "user name"</h3>
</div>
<div class="ex1">
    <form>
    <input type="checkbox" name="vehicle1" value="Bike">I have a <br>
    <input type="checkbox" name="vehicle2" value="Car"> I have a car<br>
    <input type="checkbox" name="vehicle3" value="Boat" checked> I have a boat<br><br>
    </form>
</div>

<!-- my availabilty section -->
<div class="ava">
    <h2> My Availability </h2>
</div>

<div class="selectors">
    <mainDay></mainDay>
</div>

<!-- End of Main Div -->
</div>
</template>

<script>
import mainDay from './mainDay'

export default {
    
    components: { mainDay}
}
</script>

<style>
.ava{
    margin-top: 50px;
    font-size: 25px;
}
.textsize{
    font-size: 70px;
}
.text{
    font-size: 50px;
    margin-top: 30px;
    margin-bottom: 30px;
}

div.ex1 {
  margin-left: 280px;
  margin-right: 240px;
  background-color: lightblue;
  width: 110px;
  height: 110px;
  overflow: scroll;
  width: 1240px;
  height: 420px;
}

.selectors{
    margin-left: 170px;
    margin-top: 50px;
    height: 40px;
    margin-right: 170px;
}
</style>