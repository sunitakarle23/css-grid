# css-grid
  reference-
	  https://cssgrid.io/
	  browser-sync:
		  watch html, js, css files & automatically reload the browser

#Grid lines
	The vertical and horizontal lines that divide the grid and separate the columns and rows.
#Grid cell
  A single unit of a CSS grid.
#Grid area
	Rectangular space surrounded by four grid lines. A grid area can contain any number of grid cells.
#Grid track
	The space between two grid lines. This space can be horizontal or vertical
#Grid row
	A horizontal track of a grid.
#Grid column
	A vertical track of a grid.
#Gutter
	The space between rows and columns in a grid.
#Grid container
	The container that holds the entire CSS grid. It will be the element that has the display: grid or display: inline-grid property on it.
#Grid item
	Any element that is a direct child of a grid container.
#Explicit/Implicit track
	when we set any grid coloumn or row width it is called explicit
		e.g-
			grid-template-cols: 200px 300px 600px;
				- when we does not set any grid coloumn or row width it is called implicit
			grid-template-cols: 200px 300px 600px;1

			grid-auto-rows:
				sets the property to row which have implicitly created
			grid-auto-coloumns:
				sets the property to column which have implicitly created

			grid-auto-flow: column
#sizing-track :
	free space/ fractional sets the same columns .
		e.g -  grid-template-columns: 1fr 2fr 1fr;
#grid-column :
	set number of column width
		e.g - grid-column: span 2;

#grid-row :
	set number of row width
		e.g - grid-row: span 2;

#auto-fill/auto-fit :
	fill or fit the coloumn in a given row.
	e.g -
		grid-template-column: repeat(auto-fit, 1fr);
		grid-template-column: repeat(auto-fill, 1fr);

#responsive grids:
	grid-template-column: repeat(auto-fit, minmax(150px, 1fr));

#grid-template-areas:
	set the layout areas using classnames
	e.g-
		grid-template-areas:
			"header header header"
			"sidebar content sidebar"
			"footer footer footer"
