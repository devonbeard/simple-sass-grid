simple-sass-grid
================
This is a super simple grid based system using sass.

To adjust the grid, all you need to do is change the pixel values in the variables below. You will have to do some math to find out what px. To change the column size change the *$total-column* variable to the number of columns needed:

    $max-width: 900px;
    $total-columns: 12;
    $column-width: percentage( 75px / $max-width );
    $gutter-width: percentage( 12px / $max-width );

## Types of Columns
There are two types of columns in this system. You have regular columns and then centered columns

### Columns
All columns need to be wrapped in a div with a class of row. Example below:

    <div class="row">
      <div class="col12">Here is some content</div>
    </div>

### Centered Columns
Centered columns do not need a row wrapper. Example below:

    <div class="col12-centered">Here is some content</div>
