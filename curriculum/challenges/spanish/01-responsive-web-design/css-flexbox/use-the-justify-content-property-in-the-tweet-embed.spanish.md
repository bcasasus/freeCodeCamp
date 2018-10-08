---
id: 587d78ac367417b2b2512af7
title: Use the justify-content Property in the Tweet Embed
localeTitle: Use la propiedad justify-content en el Tweet Insertar
challengeType: 0
videoUrl: ''
---

## Description
<section id='description'> 
El último desafío mostró un ejemplo de la propiedad <code>justify-content</code> . Para la inserción de tweets, esta propiedad se puede aplicar para alinear los elementos en el elemento <code>.profile-name</code> . 
</section>

## Instructions
<section id='instructions'> 
Añadir la propiedad CSS <code>justify-content</code> de la cabecera del <code>.profile-name</code> del elemento y establezca el valor en cualquiera de las opciones desde el último desafío. 
</section>

## Tests
<section id='tests'>

```yml
tests:
  - text: &#39;El elemento <code>.profile-name</code> debe tener la propiedad <code>.profile-name</code> <code>justify-content</code> establecida en cualquiera de estos valores: centro, inicio flexible, extremo flexible, espacio intermedio o espacio-alrededor.&#39;
    testString: 'assert(code.match(/header\s.profile-name\s*{\s*?.*?\s*?.*?\s*?\s*?.*?\s*?justify-content\s*:\s*(center|flex-start|flex-end|space-between|space-around)\s*;/g), "The <code>.profile-name</code> element should have the <code>justify-content</code> property set to any of these values: center, flex-start, flex-end, space-between, or space-around.");'

```

</section>

## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style>
  body {
    font-family: Arial, sans-serif;
  }
  header, footer {
    display: flex;
    flex-direction: row;
  }
  header .profile-thumbnail {
    width: 50px;
    height: 50px;
    border-radius: 4px;
  }
  header .profile-name {
    display: flex;
    flex-direction: column;

    margin-left: 10px;
  }
  header .follow-btn {
    display: flex;
    margin: 0 0 0 auto;
  }
  header .follow-btn button {
    border: 0;
    border-radius: 3px;
    padding: 5px;
  }
  header h3, header h4 {
    display: flex;
    margin: 0;
  }
  #inner p {
    margin-bottom: 10px;
    font-size: 20px;
  }
  #inner hr {
    margin: 20px 0;
    border-style: solid;
    opacity: 0.1;
  }
  footer .stats {
    display: flex;
    font-size: 15px;
  }
  footer .stats strong {
    font-size: 18px;
  }
  footer .stats .likes {
    margin-left: 10px;
  }
  footer .cta {
    margin-left: auto;
  }
  footer .cta button {
    border: 0;
    background: transparent;
  }
</style>
<header>
  <img src="https://pbs.twimg.com/profile_images/378800000147359764/54dc9a5c34e912f34db8662d53d16a39_400x400.png" alt="Quincy Larson's profile picture" class="profile-thumbnail">
  <div class="profile-name">
    <h3>Quincy Larson</h3>
    <h4>@ossia</h4>
  </div>
  <div class="follow-btn">
    <button>Follow</button>
  </div>
</header>
<div id="inner">
  <p>I meet so many people who are in search of that one trick that will help them work smart. Even if you work smart, you still have to work hard.</p>
  <span class="date">1:32 PM - 12 Jan 2018</span>
  <hr>
</div>
<footer>
  <div class="stats">
    <div class="Retweets">
      <strong>107</strong> Retweets
    </div>
    <div class="likes">
      <strong>431</strong> Likes
    </div>
  </div>
  <div class="cta">
    <button class="share-btn">Share</button>
    <button class="retweet-btn">Retweet</button>
    <button class="like-btn">Like</button>
  </div>
</footer>
```

</div>



</section>

## Solution
<section id='solution'>


```js
var code = "header .profile-name {display: flex; flex-direction: column; justify-content: center; margin-left: 10px;}"
```

</section>