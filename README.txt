




Réserve de code

/* ce code fonctionne
.btn-coeur{
    position:sticky;
    @include padding_null;
    @include btn-style-null;
    height: 20px;
    .far.fa-heart{
        position: absolute;
        z-index: 1;
        font-size: 20px;
    }
    .fas.fa-heart{
        position: relative;
        z-index: 2;
        font-size: 20px;
        visibility: hidden;
        color: transparent;
        background: linear-gradient(white, white);
        @include background-clip;
        opacity: 0%;
    }
    &:hover{
        cursor: pointer;
    }
    &:focus{
        .fas.fa-heart{
            visibility: visible;
            background: linear-gradient($color-pri, $color-duo);
            @include background-clip;
            opacity: 100%;
            transition: all 0.5s;
        }
    }
}
*/