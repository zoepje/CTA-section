<script>
  import {Arrow, Card} from "$lib/index.js"
</script>

<section>
  <div>
    <p class="label">Label</p>
    <h1>Mandatory title about the <span>call-to-action</span> here</h1>
  </div>

  <p class="body-copy">Optional body copy goes here.</p>

  <a href="/">Optional button 
    <Arrow />
  </a>
</section>

<ul>
  <li>
    <Card />
  </li>
  <li>
    <Card />
  </li>
</ul>


<style>
  section{
    display: grid;
    justify-items: center;
    gap: 16px;
    margin-bottom: 32px;
    max-width: 864px;
    margin-inline: auto;
  }

  div {
    display: grid;
    justify-items: center;
    gap: 8px;
  }

  p {
    font-weight: 450;
  }

  .label{
    color: #39494D;
    font-size: 14px;
    line-height: 16px;
    letter-spacing: 0.02em;
  }

  h1 {
    text-align: center;
    font-weight: 575;
    font-size: 36px;
    line-height: 40px;
    color: #212121;
    letter-spacing: -0.02em;

    & span {
      font-family: 'GT Alpina';
      font-weight: 300;
      font-size: 38px;
      letter-spacing: -0.03em;
    }
  }

  .body-copy {
    color: #4B5050;
    font-size: 17px;
    line-height: 24px;
  }

  a {
    display: flex;
    align-items: center;
    gap: 4px;
    font-weight: 450;
    font-size: 17px;
    line-height: 24px;
    color: #BF564D;
    text-decoration: none;

    & svg {
      padding: 5px;
    }

    & path {
      stroke: #BF564D;
    }
  }

  ul {
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-inline: auto;
  }

  li {
    flex: 1 1 335px;
  }

  @media only screen and (min-width: 768px){
    section {
      margin-bottom: 48px;
      gap: 24px;
    }

    div {
      max-width: 597px;
    }

    .label {
      font-size: 15px;
    }

    h1 {
      font-size: 40px;
      line-height: 48px;
      letter-spacing: -0.03em;
    }

    h1 span {
      font-size: 42px;
    }

    .body-copy {
      font-size: 19px;
    }

    a {
      font-size: 19px;
    }
  }

  @media only screen and (min-width: 1440px){
    section {
      margin-bottom: 80px;
    }
    
    div {
      max-width: 642px;
    }

    ul {
      gap: 24px;
    }
  }
</style>