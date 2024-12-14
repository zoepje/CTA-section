<script>
  import {Arrow} from "$lib/index.js"
</script>

<a href="/">
  <article>
    <div class="gradient">
      <div class="container-text">
        <div class="text">
          <h2>Title</h2>
          <p>Supporting text about the call-to-action goes here.</p>
        </div>
        <div class="button"><Arrow /></div>
      </div>
    </div>
  </article>
</a>

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
    display: grid;
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
    margin: 24px 16px;

    & .text {
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

  .button {
    width: 48px;
    height: 48px;
    border-radius: 4px;
    border: solid 2px #FFFFFF4D;
    background-color: transparent;
    cursor: pointer;

    & svg {
      padding: 17px;
    }

    & path {
      stroke: #FFFFFF;
    } 
  }

  a:hover .button{
    border: solid 2px #ffffff76;
  }

  @media only screen and (min-width: 768px){
    article {
      height: 45vh;
    }

    .container-text {
      margin: 32px 24px;
    }

    h2 {
      font-size: 28px;
      line-height: 32px;
      letter-spacing: -0.02em;
    }

    p {
      font-size: 19px;
    }

    button {
      width: 56px;
      height: 56px;
    }
  }

  @media only screen and (min-width: 1440px){
    article {
      height: 55vh;
    }
  }
</style>
