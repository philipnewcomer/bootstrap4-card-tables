# Bootstrap4 Card Tables

*CSS for properly rendering tables inside of cards in Bootstrap 4*

While Bootstrap 3 supported tables inside of panels, tables are not supported in cards (the replacement for panels) in Bootstrap 4. Although the resulting visual glitches can be fixed using several helper classes on the card component and the table itself, this is something that would be nice if it would just work. Thus, this package provides the needed styles to use tables inside of cards in Bootstrap 4 without any additional helper classes.

## Installation

```
npm install --save-dev bootstrap4-card-tables
```

## Usage

Import the SASS source files into your app:

```scss
@import "~bootstrap4-card-tables/src/bootstrap4-card-tables";
```

Compiled (and optionally, minified) CSS is provided in the `dist` directory:

```
https://unpkg.com/bootstrap4-card-tables@1.2.0/dist/bootstrap4-card-tables.css
https://unpkg.com/bootstrap4-card-tables@1.2.0/dist/bootstrap4-card-tables.min.css
```

## Notes

- This package fixes the use cases I encountered when trying to use tables inside of cards in Bootstrap 4, but I do not consider this package to be comprehensive. If you encounter an edge case not covered by this package, feel free to [open an issue](https://github.com/philipnewcomer/bootstrap4-card-tables/issues/new) or submit a pull request.
- There is currently an [open issue](https://github.com/twbs/bootstrap/issues/17395) and a [pull request](https://github.com/twbs/bootstrap/pull/25193) on the Bootstrap project for adding native support for tables inside of cards to an upcoming release of Bootstrap 4. While progress has been slow, it would be worth checking if there have been any recent developments there before using this package.

## Screenshots

Given the markup below, this package fixes the visual glitches without requiring any additional classes to be added to the markup.

### Before

<img width="740" alt="before screenshot" src="https://user-images.githubusercontent.com/1446874/38529055-a4763f18-3c30-11e8-863f-e8e300a90fce.png">

### After

<img width="740" alt="after screenshot" src="https://user-images.githubusercontent.com/1446874/38529061-a9dcd71e-3c30-11e8-8b5b-c3020a7dff3c.png">

### HTML

```html
<div class="card">
    <div class="card-header">Card Header</div>

    <div class="card-body">
        <p class="mb-0">
            Credibly leverage other's team building action items with extensive methodologies. Enthusiastically conceptualize competitive e-services without mission-critical relationships. Dramatically reinvent quality interfaces after inexpensive convergence. Objectively incentivize an expanded array of metrics vis-a-vis timely materials. Energistically evisculate timely data through standardized ideas.
        </p>
    </div>

    <table class="table table-bordered">
        <thead>
            <tr>
                <th>Column 1</th>
                <th>Column 2</th>
                <th>Column 3</th>
            </tr>
        </thead>

        <tbody>
            <tr>
                <td>Row 1 Cell 1</td>
                <td>Row 1 Cell 2</td>
                <td>Row 1 Cell 3</td>
            </tr>

            <tr>
                <td>Row 2 Cell 1</td>
                <td>Row 2 Cell 2</td>
                <td>Row 2 Cell 3</td>
            </tr>

            <tr>
                <td>Row 3 Cell 1</td>
                <td>Row 3 Cell 2</td>
                <td>Row 3 Cell 3</td>
            </tr>
        </tbody>
    </table>

    <div class="card-footer">
        Card Footer
    </div>
</div>
```
