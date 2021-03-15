<template>
<div class = "dropdown">
    <span>Redes</span>
       
        <div class = 'dropdown-content'>
            <p><a href = 'https:\\www.instagram.com' class = 'button fondo squareLayer'></a></p>
            <p><a href = 'https:\\www.facebook.com' class = 'button fondo' >f</a></p>
        </div>
</div>
</template>


<script>
export default {
    name : 'Redes',
    data: {
        
            instagram  : 'https:\\www.instagram.com',
            facebook : 'https:\\www.facebook.com'
        
    }
}
</script>

<style scoped>

.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  padding: 12px 16px;
  z-index: 1;
}

.dropdown:hover .dropdown-content {
  display: block;
}
.container {
  display: flex;                  
  flex-direction: column;
  justify-content: center;            
}
.container > div {
  width: 100px;
  height: 100px;
  border: 2px dashed red;
}

.button{
  background-color:#fff; /* white */
  border-radius: 8px;
  color: rgb(0, 0, 0);
  text-align: center;
  font-family: sans-serif;
  font-weight: bold;
  font-size: 40px;
  text-decoration: none;
  display: inline-block;
  top:0%
}
.button:hover{
    background-color: #50d890;
}

.fondo {
    width: 3rem;
    height: 3rem;
    background:transparent;
    border-radius: 1rem;
    margin: auto;

}
.squareLayer{
    width: 2rem;
    height: 2rem;
    border: 0.3rem solid rgb(0, 0, 0);
    background-color: transparent;
    border-radius: 0.5rem solid rgb(196, 31, 31);
    border-radius: 0.6rem;
    position: relative;
    top:0.1rem;
    left: 0.2rem;
}
.squareLayer::before{
    content: "";
    width: 0.9rem;
    height: 0.9rem;
    border: 0.2rem solid rgb(0, 0, 0);
    background-color: transparent;
    border-radius: 1rem solid rgb(0, 0, 0);
    border-radius: 50%;
    position: absolute;
    left: 0.35rem;
    top: 0.36rem;

}
.squareLayer::after{
    content: "";
    width: 0.4rem;
    height: 0.4rem;
    background-color: #000;
    border-radius: 1rem solid #000;
    border-radius: 80%;
    position: absolute;
    right: 0.1rem;
    top: 0.15rem;
}
.ftop{
    width: 1.3rem;
    height:3rem;
    left:0.9rem;
    top:0.1rem;
    background: #000;
    position: relative;
    border-top-left-radius:1rem;
}
.fshaper{
    background: #fff;
    width: 0.8rem;
    height:2.3rem;
    top:0.7rem;
    left: 0.7rem;
    position: relative;
    border-top-left-radius: 0.5rem;
}
.fline{
    background: #000;
    width: 1.5rem;
    height: 0.6rem;
    position: relative;
    left: 0.5rem;
    bottom: 1.5rem;

}

</style>