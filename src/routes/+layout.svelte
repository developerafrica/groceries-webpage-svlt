<script>
  import "../app.scss";
</script>
<div class="layout">
  <div class="lay-out">
    <header>
      <div class="brand">
        <div class="logo">
          <img src="/logo.png" alt="logo">
        </div>
        <div class="text">
          <h1>
            DEVELOPER AFRICA MW
          </h1>
        </div>
      </div>
    </header>
    <main>
      <slot />
    </main>
    <footer>
      <div class="ft"><a href="https://grocerylistmw.netlify.app">LAUNCH APP</a></div>
    </footer>
  </div>
</div>
<style lang="scss">
  @mixin fnt ($c,$s,$w) {
    font-size: $s;
    color: $c;
    font-weight: $w;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;  
}
  
  .layout{
    .lay-out{
      header{
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        z-index: 10;
        background: var(--gn);
        .brand{
          display: flex;
          align-items: center;
          justify-content: space-between;
          padding: 10px 10px          
        }
        .logo{
          img{
            width: 30px;
          }
        }
        .text{
          h1{
            @include fnt(var(--wt), 0.8rem, 500)
          }
        }
      }
      footer{
        text-align: center;
        position: fixed;
        bottom: 0;
        left: 0;
        width: 100%;
        .ft{
          padding: 10px;
          a{
            background: var(--gn);
            border-radius: 5px;
            padding: 15px 0;
            display: block;
            @include fnt(var(--wt), 1rem, 450);
            text-decoration: none;
          }
        }
      }
    }
  }
</style>
