<script>
	// logic goes here
</script>
<div class="sticky-header">
	<nav>
		<ul>
			<li><a href="/">Home</a></li>
			<li><a href="/login">Login</a></li>
			<li><a href="/">Blog</a></li>
		</ul>
	</nav>
</div>

<style>
.sticky-header {
  background-color: #333;
  color: #fff;
  position: sticky; /* Apply the sticky positioning */
  top: 0; /* Stick the element to the top of the viewport */
  z-index: 100; /* Ensure the navbar is above other content */
}


a:link, a:hover, a:visited, a:visited:hover, a:active {
	color: blue;
}

.sticky-header nav {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 0px 20px;
}

.sticky-header ul {
  list-style: none;
  margin: 0;
  padding: 0.7em;
  display: flex;
}

.sticky-header li {
  margin-right: 20px;
}

.sticky-header a {
  text-decoration: none;
  color: salmon;
}

nav {
	align-content: center;
}
ul {
	list-style: none;
}
</style>
