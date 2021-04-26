




Réserve de code

/*
.btn-coeur{
    @include padding_null;
    height: 20px;
    background: unset;
    border: unset;
    .far.fa-heart{
        font-size: 20px;
    }
    .fas.fa-heart{
        display: none;
        visibility: hidden;
    }
    &:hover{
        cursor: pointer;
    }
    &:active{
        .far.fa-heart{
            display: none;
        }
        .fas.fa-heart{
            display: unset;
            visibility: visible;
            font-size: 20px;
            color: transparent;
            background: linear-gradient($color-pri, $color-duo);
            background-clip: text;
        }
    }
}
*/

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
