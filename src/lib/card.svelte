<script>
  import {Arrow} from "$lib/index.js"
</script>

<article>
  <div class="gradient">
    <div class="container-text">
      <div>
        <h2>Title</h2>
        <p>Supporting text about the call-to-action goes here.</p>
      </div>
      <button><Arrow /></button>
    </div>
  </div>
</article>

<style>
  article {
    display: grid;
    position: relative;
    min-width: 335px;
    min-height: 257px;
    border-radius: 4px;
    background-color: #FFDFB2;
    background-image: url(/images/hero-image.png);
    background-position: center;
    background-size: cover;
  }

  .gradient {
    width: 100%;
    height: 50%;
    position: absolute;
    bottom: 0;
    border-radius: 4px;
    background: linear-gradient(rgba(20, 20, 20, 0), rgb(20, 20, 20));
  }

  .container-text {
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    position: absolute;
    bottom: 0;
    margin: 23px 16px;

    & div {
      display: grid;
      gap: 8px;
      width: 80%;
    }
  }

  h2 {
    font-weight: 600;
    font-size: 22px;
    line-height: 24px;
    letter-spacing: -0.01em;
    color: #FFFFFF;
  }

  p {
    font-weight: 450;
    font-size: 17px;
    line-height: 24px;
    color: #FAFAFA94;
  }

  button {
    width: 48px;
    height: 48px;
    border-radius: 4px;
    border: solid 2px #FFFFFF4D;
    background-color: transparent;

    & path {
      stroke: #FFFFFF;
    } 
  }
</style>
