Mixins
=======

A collection of helpful Sass mixins. You can use this as an alternate to compass if you need a general set of mixins such as roundeder corners, opacity, shadows, etc. Full list below. 

All mixins generate the following prefixes automatically: 

* -webkit /* Safari and Chrome */
* -khtml /* IE 9 */
* -ms /* IE 9 */
* -moz /* Firefox */
* -o /* Opera */


Usage (Example)
========================
Simply import the mixin file and then use like any normal Sass mixin. 

`
@import 'mixins';

.overlay {
	@include opacity(0.5, ); 
	position: fixed; 
	top: 0px; 
	left: 0px; 
	right: 0px; 
	bottom: 0px; 
	z-index: 1000; 
}
`
**Produces**
.overlay {
	-webkit-opacity: 0.5; /* Safari and Chrome */
    -khtml-opacity: 0.5; /* IE 9 */
    -ms-opacity: 0.5; /* IE 9 */
    -moz-opacity: 0.5; /* Firefox */
    -o-opacity: 0.5; /* Opera */
    opacity: 0.5;
    filter: alpha(opacity = 0.5 * 100);
	position: fixed; 
	top: 0px; 
	left: 0px; 
	right: 0px; 
	bottom: 0px; 
	z-index: 1000; 
}
`

List of CSS Mixins w/ (Default Values)
=====================================
* **opacity**  opacity($trans: 0.75)
* **border-box** border-box()
* **border-radius** border-radius($radius: 4px) 
* **box-shadow** box-shadow($offset: 1px, $spread: 2px, $color: #999999) 
* **rotate** rotate($degree: 7deg) 