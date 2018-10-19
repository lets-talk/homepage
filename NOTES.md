https://github.com/middleman/middlemanapp.com/blob/master/source/stylesheets/base/_base.scss

https://github.com/twbs/bootstrap/blob/v4-dev/scss/_variables.scss


<%= link_to(
  "¿Quieres conocer mas sobre Let´s Talk?",
  "#about",
  target: "_blank"
) %>
>


<ol>
  <% data.home.benefits.each do |benefit| %>
  <li><%= benefit %></li>
  <% end %>
</ol>


<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 400 340" class="middleman-logo" aria-labelledby="middleman-logo__title" role="img">
  <title id="middleman-logo__title">Middleman</title>
  <path class="middleman-logo__top-left-bar" fill-opacity=".45" d="M0 40L200 0v30L0 60z"/>
  <path class="middleman-logo__top-right-bar" fill="#fff" d="M200 0l200 40v20L200 30z"/>
  <path class="middleman-logo__left-m" fill-opacity=".45" d="M0 78v184l45 5V152l45 83 47-83v129l53 7V52l-57 8-43 83-43-70z"/>
  <path class="middleman-logo__right-m" fill="#fff" d="M400 78v184l-45 5V152l-45 83-47-83v129l-53 7V52l57 8 43 83 43-70z"/>
  <path class="middleman-logo__bottom-left-bar" fill-opacity=".45" d="M0 300l200 40v-30L0 280z"/>
  <path class="middleman-logo__bottom-right-bar" fill="#fff" d="M200 340l200-40v-20l-200 30z"/>
</svg>


      name: Nombre
      email: Correo electrónico o teléfono
      subject: Que necesitas?
      message: Tu mensaje
      action: ENVIAR MENSAJE


<input type="<%= input.type %>" placeholder="<%= input.placeholder %><%= input.placeholder.blank ? input.placeholder : '' %>">

body {
  color: #333;
  font-family: -apple-system, BlinkMacSystemFont, "Avenir Next", "Avenir",
    "Segoe UI", "Lucida Grande", "Helvetica Neue", "Helvetica", "Fira Sans",
    "Roboto", "Noto", "Droid Sans", "Cantarell", "Oxygen", "Ubuntu",
    "Franklin Gothic Medium", "Century Gothic", "Liberation Sans", sans-serif;
  padding: 18vh 1rem;
  text-align: center;
}

a {
  color: rgba(#000, 0.7);

  &:focus,
  &:hover {
    color: rgba(#000, 0.6);
  }
}

.middleman-logo {
  margin-bottom: 1rem;
  width: 10rem;
}











// Variables
//
// Variables should follow the `$component-state-property-size` formula for
// consistent naming. Ex: $nav-link-disabled-color and $modal-content-box-shadow-xs.


// Color system

$white:    #fff !default;
$black:    #000 !default;


$primary:       $blue !default;
$secondary:     $gray-600 !default;
$success:       $green !default;
$info:          $cyan !default;
$warning:       $yellow !default;
$danger:        $red !default;
$light:         $gray-100 !default;
$dark:          $gray-800 !default;


// Body
//
// Settings for the `<body>` element.

$body-bg:                   $white !default;
$body-color:                $gray-900 !default;


// Links
//
// Style anchor elements.

$link-color:                theme-color("primary") !default;
$link-decoration:           none !default;
$link-hover-color:          darken($link-color, 15%) !default;
$link-hover-decoration:     underline !default;


// Paragraphs
//
// Style p element.

$paragraph-margin-bottom:   1rem !default


// Grid breakpoints
//
// Define the minimum dimensions at which your layout will change,
// adapting to different screen sizes, for use in media queries.

$grid-breakpoints: (
  xs: 0,
  sm: 576px,
  md: 768px,
  lg: 992px,
  xl: 1200px
) !default;


// Grid containers
//
// Define the maximum width of `.container` for different screen sizes.

$container-max-widths: (
  sm: 540px,
  md: 720px,
  lg: 960px,
  xl: 1140px
) !default;


// Grid columns
//
// Set the number of columns and specify the width of the gutters.

$grid-columns:                12 !default;
$grid-gutter-width:           30px !default;

// Fonts
//
// Font, line-height, and color for body text, headings, and more.

// stylelint-disable value-keyword-case
$font-family-sans-serif:      -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji" !default;
$font-family-monospace:       SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace !default;
$font-family-base:            $font-family-sans-serif !default;
// stylelint-enable value-keyword-case

$font-size-base:              1rem !default; // Assumes the browser default, typically `16px`
$font-size-lg:                ($font-size-base * 1.25) !default;
$font-size-sm:                ($font-size-base * .875) !default;



font-family: Montserrat-Bold;
font-size: 44px;
color: #000000;
letter-spacing: -0.73px;
line-height: 56px;

/* Typography
–––––––––––––––––––––––––––––––––––––––––––––––––– */
h1, h2, h3, h4, h5, h6 {
  margin-top: 0;
  margin-bottom: 2rem;
  font-weight: 300;
}

h1 { font-size: 4.0rem; line-height: 1.2;  letter-spacing: -.1rem;}
h2 { font-size: 3.6rem; line-height: 1.25; letter-spacing: -.1rem; }
h3 { font-size: 3.0rem; line-height: 1.3;  letter-spacing: -.1rem; }
h4 { font-size: 2.4rem; line-height: 1.35; letter-spacing: -.08rem; }
h5 { font-size: 1.8rem; line-height: 1.5;  letter-spacing: -.05rem; }
h6 { font-size: 1.5rem; line-height: 1.6;  letter-spacing: 0; }

/* Larger than phablet */
@media (min-width: 550px) {
  h1 { font-size: 5.0rem; }
  h2 { font-size: 4.2rem; }
  h3 { font-size: 3.6rem; }
  h4 { font-size: 3.0rem; }
  h5 { font-size: 2.4rem; }
  h6 { font-size: 1.5rem; }
}



font-family: OpenSans-Regular;
font-size: 32px;
color: #000000;
letter-spacing: -0.53px;
line-height: 48px;



$spacers: (
  0:      0,
  xxs:    $space-xxs,
  xs:     $space-xs,
  sm:     $space-sm,
  md:     $space-md,
  lg:     $space-lg,
  xl:     $space-xl,
  xxl:    $space-xxl,

  small:  $space-small,
  medium: $space-medium,
  large:  $space-large,
  xlarge: $space-xlarge
);

$space-xxs:           $unit * 0.5;   //   4px
$space-xs:            $unit * 1;     //   8px
$space-sm:            $unit * 1.5;   //  12px
$space-md:            $unit * 2;     //  16px
$space-lg:            $unit * 3;     //  24px
$space-xl:            $unit * 4;     //  32px
$space-xxl:           $unit * 5;     //  40px

$space-small:         $unit * 10;    //  80px
$space-medium:        $unit * 15;    // 120px
$space-large:         $unit * 20;    // 160px
$space-xlarge:        $unit * 30;    // 240px

$spacers: (
  0:      0,
  x0_5:   $space-xxs,
  x1:     $space-xs,
  x1_5:   $space-sm,
  x2:     $space-md,
  x3:     $space-lg,
  x4:     $space-xl,
  x5:     $space-xxl,

  x10:    $space-small,
  x15:    $space-medium,
  x20:    $space-large,
  x30:    $space-xlarge
);

















input[type="email"],
input[type="number"],
input[type="search"],
input[type="text"],
input[type="tel"],
input[type="url"],
input[type="password"],
textarea,
select {
  height: 32px;
  padding: 6px 8px; // The 6px vertically centers text on FF, ignored by Webkit
  background-color: #fff;
  border: 1px solid #D1D1D1;
  border-radius: 4px;
  box-shadow: none;
  box-sizing: border-box;
}

// Removes awkward default styles on some inputs for iOS
input[type="email"],
input[type="number"],
input[type="search"],
input[type="text"],
input[type="tel"],
input[type="url"],
input[type="password"],
textarea {
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
}

textarea {
  min-height: 65px;
  padding-top: 6px;
  padding-bottom: 6px;
}

input[type="email"]:focus,
input[type="number"]:focus,
input[type="search"]:focus,
input[type="text"]:focus,
input[type="tel"]:focus,
input[type="url"]:focus,
input[type="password"]:focus,
textarea:focus,
select:focus {
  border: 1px solid #33C3F0;
  outline: 0;
}