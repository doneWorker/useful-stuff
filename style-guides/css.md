# CSS Code Style

## Colors

- Hex colors should be in lowercase:

  ```
  /* Bad */
  .selector {
    color: #EEE;
  }

  /* Good */
    .selector {
    color: #eee;
  }
  ```

- If hex color has alias, use it

```
    /* Bad */
    div {
        color: #000;
    }

    /* Good */
    div {
        color: black;
    }
```

## Properties ordering

- Group related css properties:

```
.selector {
    /* Positioning */
    position: absolute;
    z-index: 10;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;

    /* Display */
    display: inline-block;
    overflow: hidden;
    box-sizing: border-box;
    width: 100px;
    height: 100px;
    padding: 10px;
    margin: 10px;

    /* Fonts */
    font-family: sans-serif;
    font-size: 16px;
    text-align: right;

    /* Shadows, Borders */
    border: 10px solid #333;
    box-shadow: 0 0 2px red;


    /* Colors */
    background: #000;
    color: #fff;
}
```

- When dealing with pseudo-element always place `content` property on top:

```
    .selector:after {
        content: '';
    }
```

## Worth reading

idomatic CSS: https://github.com/necolas/idiomatic-css
