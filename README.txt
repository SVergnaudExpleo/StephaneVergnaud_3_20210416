@media only screen 
  and (max-width: 3000px) {



/*test multi condition*/

$max-ecran: screen  ;

@function media-query($ecran){
    @if ($ecran ">=" 720px) {
        @return rgb(90, 84, 84);
    }
    @if ($ecran "<=" 1200px) {
        @return red;
    }
    @else{
        @return magenta;
    }
}

@mixin media-color ($color-query: media-query($max-ecran)){
    background: $color-query;
}
