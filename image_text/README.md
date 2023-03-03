# How to use the Image and Text sections for webpages

## Add the CSS

```
<style>
    .container {
        width: 100%;
        max-width: 1280px;
        margin: 0 auto;
        padding: 20px;
        box-sizing: border-box;
    }
    .text-with-image{
        display: grid;
        grid-template-columns: 1fr;
    }
    .text-with-image img{
        width: 100%;
    }
@media only screen and (min-width: 700px){
    .text-with-image{
        grid-template-columns: minmax(350px, 1fr) 2fr;
        gap: 20px;
    }
    .text-with-image__reverse{
        grid-template-columns: 2fr minmax(350px, 1fr) ;
    }
}
</style>
```




```
<section class="text-with-image container">
    <img src="[IMAGE_URL_HERE]"
        alt="">
    <div class="text-with-image__content">
        <h2>TITLE HERE</h2>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ducimus earum assumenda deleniti. Asperiores,
            repellat officiis! Vel distinctio, dolorum vero dignissimos sapiente laborum beatae quasi itaque! Impedit
            distinctio corporis voluptate reiciendis fugit maxime quasi, sequi autem quas sapiente voluptatem repellat
            odio quidem excepturi voluptates iste magnam cumque explicabo ea minus ab.</p>
    </div>
</section>
```