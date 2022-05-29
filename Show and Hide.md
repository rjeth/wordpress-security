<script>
var divs
var btn1 = document.getElementById("btn1");
var btn2 = document.getElementById("btn2");
var btn3 = document.getElementById("btn3");
var btn4 = document.getElementById("btn4");
var btn5 = document.getElementById("btn5");
var btn6 = document.getElementById("btn6");
btn1.onclick = function(event){
    event.preventDefault();
    toggleDivs("sect1");
};
btn2.onclick = function(event){
    event.preventDefault();
    toggleDivs("sect2");
};
btn3.onclick = function(event){
    event.preventDefault();
    toggleDivs("sect3");
};
btn4.onclick = function(event){
    event.preventDefault();
    toggleDivs("sect4");
};
btn5.onclick = function(event){
    event.preventDefault();
    toggleDivs("sect5");
};
btn6.onclick = function(event){
    event.preventDefault();
    toggleDivs("sect6");
};
function toggleDivs(s){

    //reset
    document.getElementById("sect1").classList.remove("shown");
    document.getElementById("sect2").classList.remove("shown");
    document.getElementById("sect3").classList.remove("shown");
    document.getElementById("sect4").classList.remove("shown");
    document.getElementById("sect5").classList.remove("shown");
    document.getElementById("sect6").classList.remove("shown");
    //show
    document.getElementById(s).classList.add("shown");
}
//force button1 state initialise, if required
//btn1.focus();
//btn1.click();
</script>
<style>

    .elementor-editor-active .hidden{
        display:block;
    }
    .hidden{
        display:none;
    }
    .shown{
        display: block !important;
         -webkit-transition: transform 0.34s ease;
transition : transform 0.34s ease;
    }
    .align{
        text-align: center;
    }
    .text-white{
       color: white; 
    }

</style>
