<template>
  <div class="background">
    <div class="strip left a1"></div>
    <div class="strip left a2"></div>
    <div class="strip left a3"></div>
    <div class="strip left a4"></div>
    <div class="strip left a5"></div>
    <div class="strip left a6"></div>
    <div class="strip left a7"></div>
    <div class="strip left a8"></div>
    <div class="strip right b1"></div>
    <div class="strip right b2"></div>
    <div class="strip right b3"></div>
    <div class="strip right b4"></div>
    <div class="strip right b5"></div>
    <div class="strip right b6"></div>
    <div class="strip right b7"></div>
    <div class="strip right b8"></div>

    
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import url(https://fonts.googleapis.com/css?family=Merriweather:400,700|Merriweather+Sans:400,700);





@keyframes fadeIn {
  from { opacity: 0; }
  to  { opacity: 1; }
}
.strip {
  position: fixed;
  width: 50%;
  height: 12.5%;
}

.left { left: 0; }
.right { right: 0; }

.a1, .b1 { top: 0%; }
.a2, .b2 { top: 12.5%; }
.a3, .b3 { top: 25%; }
.a4, .b4 { top: 37.5%; }
.a5, .b5 { top: 50%; }
.a6, .b6 { top: 62.5%; }
.a7, .b7 { top: 75%; }
.a8, .b8 { top: 87.5%; }



.a1 {
  background-color: #675CE0;
  animation: openA1 1.5s linear 0.5s forwards;
}

.a2 {
  background-color: #6470E0;
  animation: openA2 1.5s linear 0.5s forwards;
}
.a3 {
  background-color: #6284E0;  
  animation: openA3 1.5s linear 0.5s forwards;
}
.a4 {
  background-color: #5F97E0;
  animation: openA4 1.5s linear 0.5s forwards;
}
.a5 {
  background-color: #5CABE0;
  animation: openA5 1.5s linear 0.5s forwards;
}
.a6 {
  background-color: #5CB8DC;
  animation: openA6 1.5s linear 0.5s forwards;
}
.a7 {
  background-color: #5DC5D8;
  animation: openA7 1.5s linear 0.5s forwards;
}
.a8 {
  background-color: #5DDFD0;
  animation: openA8 1.5s linear 0.5s forwards;
}

@keyframes openA1 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 15%; }
}
@keyframes openA2 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 10%; }
}
@keyframes openA3 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 15%; }
}
@keyframes openA4 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 10%; }
}
@keyframes openA5 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 15%; }
}
@keyframes openA6 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 10%; }
}
@keyframes openA7 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 15%; }
}
@keyframes openA8 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 10%; }
}


.b1 {
  background-color: #675CE0;
  animation: openA1 1.5s linear 0.5s forwards;
}
.b2 {
  background-color: #6470E0;
  animation: openB2 1.5s linear 0.5s forwards;
}
.b3 {
  background-color: #6284E0;
  animation: openB3 1.5s linear 0.5s forwards;
}
.b4 {
  background-color: #5F97E0;
  animation: openB4 1.5s linear 0.5s forwards;
}
.b5 {
  background-color: #5CABE0;
  animation: openB5 1.5s linear 0.5s forwards;
}
.b6 {
  background-color: #5CB8DC;
  animation: openB6 1.5s linear 0.5s forwards;
}
.b7 {
  background-color: #5DC5D8;
  animation: openB7 1.5s linear 0.5s forwards;
}
.b8 {
  background-color: #5DDFD0;
  animation: openB8 1.5s linear 0.5s forwards;
}

@keyframes openB1 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 15%; }
}
@keyframes openB2 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 10%; }
}
@keyframes openB3 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 15%; }
}
@keyframes openB4 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 10%; }
}
@keyframes openB5 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 15%; }
}
@keyframes openB6 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 10%; }
}
@keyframes openB7 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 15%; }
}
@keyframes openB8 { 
  from { width: 50%; }
  75%  { width: 15%; }
  to   { width: 10%; }
}




</style>
