# pnv_1606_aaFSA_SSver3_6Lin_eIc_on
Sassを勉強するためにTimebit会社で開発していました。

#ステップス
一目：せってい：Install　sass => search google (mac: sudo gem install ..)
に目：プロジェクトの中には：sass --watch input.scss:output.css. 

#.  sass --watch scss/layout.scss:css/layout.min.css --style compressed --scss

＃スタート
色　（color)
インポルト（import）
（MIXIN)
（CLASS DUNG CHUNG）
（EXTEND)　KETHUA
＆：。。。HOVER focus ,.


＃例：
footer {
    section {
        h5 {
            font-size: 14px;
            font-weight: bold;
        }
        p {}
        .demo__div {
            @include demo_mixin( 15px, $color_black, $color_w);
            h6 {
                @extend h5;
                text-transform: capitalize;
                &:hover {}
            }
        }
    }
}

＝＝＝＝＝＝＝＝＝＝＝＝＝＝

$color_background: #f0f0f0; // Color White
$color_w: #fff; // Color White



＝＝＝＝＝＝＝＝＝＝＝＝＝

@mixin title_main($font-size, $transform, $font-weight, $color) {
    font-size: $font-size;
    text-transform: $transform;
    font-weight: $font-weight;
    color: $color;
}

@mixin demo_mixin($font-size, $background-c, $color) {
    font-size: $font-size;
    background-color: $background-c;
    color: $color;
}




