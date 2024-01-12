# underline hover effect on navigation
```css
.navbar-nav li a {
	text-transform: uppercase;
	letter-spacing: 1.5px;
	position: relative;
	transition: all 0.3s ease-in-out;
}

 /* Navbar Underline Animation / Transition */
.navbar-nav li a:before {                            
	content: "";
	position: absolute;
	top: 90%;
	width: 0%;
	height: 3px;
	background: #0165ba;
	transition: all 0.3s ease-in-out;
}
```

# Breakpoints
```css
@media screen and (min-width: 576px) {
	.navbar-nav li a:hover::before {
		width: 80%;
	}
}

@media only screen and (max-width: 576px) {
	.navbar-nav li a:hover::before {
		width: 40%;
	}
}
```
