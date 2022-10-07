## CSS repo

Use firefox for debuggin css(has more usefull tools for that)

download firefox extension then run:

Windows

"C:\Program Files\Mozilla Firefox\firefox.exe" -start-debugger-server

(This syntax is for a regular command prompt (cmd.exe), not PowerShell!)

OS X

/Applications/Firefox.app/Contents/MacOS/firefox -start-debugger-server

Linux

firefox -start-debugger-server

### cut text depends on width size

```html
  <div class="box">
    <div class="text-cut">Legnica Love</div>
  </div>
```

```css
.text-cut{
  width: 70px;
  height: 20px;
  overflow: hidden;
}

@media only screen and (min-width: 600px) {
  .text-cut{
    width: 100%;
  }
}
```

second css solution:

```css
.text-cut{
  width: clamp(70px,10vw,400px);
  height: 20px;
  overflow: hidden;
}
```


