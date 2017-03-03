# Subtle Grid

This is a grid that I build on top of flexbox so I can save time whenever I just want a simple layout done fast.

## Notes

- Each of these containers scale to 100% of the parent container.
- They are mobile responsive, with pre-defined layout on smaller screens.
- The gutters (spacing between columns) are predefined but can be customized.
- You can use the css as is otherwise you can customize or add on top of this by modifying the scss and use a scss processor like [Scout](http://scout-app.io/classic/) to compile.

## To Start

Just download or copy the scss/css to your project and it'll work!


## Usage

Use `.row` if you want to stack content horizontally

```
<div class="row">
	<div class="content"></div>
	<div class="content"></div>
	<div class="content"></div>
</div>
```

Use `.col` if you want to stack content vertically

```
<div class="col">
	<div class="content"></div>
	<div class="content"></div>
	<div class="content"></div>
</div>
```

You can combine both of them

```
<!-- 3 columns inside a row container -->
<div class="row">
	<div class="col">
		<div class="content"></div>
		<div class="content"></div>
		<div class="content"></div>
	</div>	
	<div class="col">
		<div class="content"></div>
		<div class="content"></div>
		<div class="content"></div>
	</div>
	<div class="col">
		<div class="content"></div>
		<div class="content"></div>
		<div class="content"></div>
	</div>
</div>

```

Use pre-defined containers

```
<!-- Half class -->
<div class="row">
	<div class="half">
		<div class="content"></div>
	</div>
	<div class="half">
		<div class="content"></div>
	</div>
</div>


<!-- Class for 1/3 containers-->
<div class="row">
	<div class="one-third">
		<div class="content">.one-third</div>
	</div>
	<div class="one-third">
		<div class="content">.one-third</div>
	</div>
	<div class="one-third">
		<div class="content">.one-third</div>
	</div>
</div>


<!-- Class for 1/4 containers-->
<div class="row">
	<div class="one-quarter">
		<div class="content"></div>
	</div>
	<div class="one-quarter">
		<div class="content"></div>
	</div>
	<div class="one-quarter">
		<div class="content"></div>
	</div>
	<div class="one-quarter">
		<div class="content"></div>
	</div>
</div>
<!-- Continue for one-fifth and one-sixth-->

```

There are containers for Sidebar and main content

```
<!-- Sidebar and main Content -->
<div class="row">
	<div class="one-third">
		<div class="content"></div>
	</div>
	<div class="auto">
		<div class="content"></div>
	</div>
</div>


<div class="row">
	<div class="one-quarter">
		<div class="content"></div>
	</div>
	<div class="col-auto">
		<div class="content"></div>
	</div>
</div>


<div class="row">
	<div class="one-fifth">
		<div class="content"></div>
	</div>
	<div class="auto">
		<div class="content"></div>
	</div>
</div>


<div class="row">
	<div class="one-sixth">
		<div class="content"></div>
	</div>
	<div class="auto">
		<div class="content"></div>
	</div>
</div>
```


You can nest them however you like

```
<div class="row">
	<div class="half">
		<div class="row">
			<div class="half">
				<div class="auto">
					<div class="content"></div>
				</div>
			</div>
			<div class="half">
				<div class="auto">
					<div class="content"></div>
				</div>
			</div>
		</div>
		<div class="row">
			<div class="auto">
				<div class="content"></div>
			</div>
		</div>
	</div> <!-- end 1st half-->
	<div class="half">
		<div class="col">
			<div class="content"></div>
			<div class="content"></div>
			<div class="content"></div>
		</div>
	</div>
</div> <!-- end 2nd half -->
```

Last but not least you can move things to left, right or center

```
<ul class="row left">
	<li><a href="">Home</a></li>
	<li><a href="">About</a></li>
	<li><a href="">Blog</a></li>
	<li><a href="">Contact</a></li>
</ul>

<ul class="row center">
	<li><a href="">Home</a></li>
	<li><a href="">About</a></li>
	<li><a href="">Blog</a></li>
	<li><a href="">Contact</a></li>
</ul>


<ul class="row right">
	<li><a href="">Home</a></li>
	<li><a href="">About</a></li>
	<li><a href="">Blog</a></li>
	<li><a href="">Contact</a></li>
</ul>
```


