---
id: bad87fee1348bd9aedb08845
title: Responsively Style Radio Buttons
required:
  - link: 'https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.2.0/css/font-awesome.css'
    raw: true
challengeType: 0
videoUrl: ''
localeTitle: Botones de radio de estilo responsivo
---

## Description
<section id="description"> ¡También puedes usar las clases <code>col-xs-*</code> en elementos de <code>form</code> ! De esta manera, nuestros botones de radio se distribuirán de manera uniforme en toda la página, independientemente de la resolución de la pantalla. Anida ambos botones de radio dentro de un elemento <code>&lt;div class=&quot;row&quot;&gt;</code> . Luego anida cada uno de ellos dentro de un elemento <code>&lt;div class=&quot;col-xs-6&quot;&gt;</code> . <strong>Nota:</strong> Como recordatorio, los botones de radio son elementos de <code>input</code> de tipo <code>radio</code> . </section>

## Instructions
<section id="instructions">
</section>

## Tests
<section id='tests'>

```yml
tests:
  - text: Anida todos los botones de radio dentro de un <code>div</code> con la <code>row</code> clase.
    testString: 'assert($("div.row:has(input[type=\"radio\"])").length > 0, "Nest all of your radio buttons inside one <code>div</code> with the class <code>row</code>.");'
  - text: Anida cada uno de sus botones de radio dentro de su propia <code>div</code> con la clase <code>col-xs-6</code> .
    testString: 'assert($("div.col-xs-6:has(input[type=\"radio\"])").length > 1, "Nest each of your radio buttons inside its own <code>div</code> with the class <code>col-xs-6</code>.");'
  - text: Asegúrese de que cada uno de sus elementos <code>div</code> tenga una etiqueta de cierre.
    testString: 'assert(code.match(/<\/div>/g) && code.match(/<div/g) && code.match(/<\/div>/g).length === code.match(/<div/g).length, "Make sure each of your <code>div</code> elements has a closing tag.");'

```

</section>

## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  h2 {
    font-family: Lobster, Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }
</style>

<div class="container-fluid">
  <div class="row">
    <div class="col-xs-8">
      <h2 class="text-primary text-center">CatPhotoApp</h2>
    </div>
    <div class="col-xs-4">
      <a href="#"><img class="img-responsive thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
    </div>
  </div>
  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <div class="row">
    <div class="col-xs-4">
      <button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info"><i class="fa fa-info-circle"></i> Info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger"><i class="fa fa-trash"></i> Delete</button>
    </div>
  </div>
  <p>Things cats <span class="text-danger">love:</span></p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>

```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
